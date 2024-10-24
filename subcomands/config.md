# Config

конфигурационные файлы

- .git/config (--local)
- ~/.gitconfig (--global)
- /etc/gitconfig (--system)

```bash
# установки имени и e-mail пользователя
$ git config --global user.name "..."
$ git config --global user.email "..."
# вывод всех переменных
$ git config --list
$ git config -l
$ git config --list --show-origin
$ git config --list --global
$ cat ~/.gitconfig
# удаления настройки
$ git config --unset --global user.email
```

## Настройка псевдонимов

```bash
$ git config --global alias.show-graph 'log --graph --abbrev-commit --pretty=oneline'
```
