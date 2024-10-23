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
