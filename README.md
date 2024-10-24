# GIT

## установка

```bash
 $ sudo apt install git
 $ sudo apt install git git-doc gitweb
 $ sudo apt install git gitk
```

```bash
# Получение исходного кода http://git.kernel.org в каталоге pub/software/scm
# 1
$ cd git-2.3
# 2
$ ./configure
$ ./configure --prefix=/usr/local
# 3
$ make all
$ make all doc
# 4
$ make install
$ sudo make install install-doc
```

## Создание начального репозитария

```bash
# 1
$ mkdir ~/public_html
# 2
$ cd ~/public_html
# 3
$ echo "hello git" > index.html
# 4
$ git init
```

## Добавление файлов в ваш репозитарий

```bash
# 1
$ git add index.html
# Чтоби добавить в репозитарий все фаайлы в каталоге о во всех подкаталогах
$ git add .
# 2
$ git status
# 3
$ git commit -m "...."
# 4
$ git status
```

## Настройка автора коммита(фиксации)

```bash
# 1
$ git config --global user.name "..."
$ git config --global user.email "..."
# 2
```

```bash
# Вы также можете сообщить Git свое имя и свой e-mail, установив перемен­ные окружения
$ export GIТ_AUTHOR_NAME=...
$ export GIТ_AUTHOR_EMAIL=...
```

## Теги

объект тега назначает человекочитаемое имя определенному объек­ту, обычно фиксации

- Легковесный тег - это просто ссылка на объект фиксации и обычно он част­
  ный для репозитария. Эти теги не создают постоянный объект в хранилище
  объектов.
- Аннотированный тег

```bash
$ git tag -m "version 1.0" V1.0 4876jg
```

```bash
# Увидеть объект тега
# 1
$ git rev-parse V1.0
786532kjd
# 2
$ git cat-file -p 786532kjd
```

Git может удалить файл только из индекса или одновременно из индекса и
рабочего каталога. Git не может удалить файл только из рабочего каталога,
для этого используется команда операционной системы
