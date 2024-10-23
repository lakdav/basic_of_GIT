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
