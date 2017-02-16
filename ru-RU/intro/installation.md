---
name: Установка
---

# Установка

## Установочные пакеты

Вы можете скачать установочные пакеты последней версии с [GitHub](https://github.com/peachdocs/peach/releases).

## Из исходного кода

Установка из исходного кода требует наличия языка программирования [Go] (https://golang.org/) и правильно настроенной переменной среды окружения `$GOPATH`.

Проверить можно с помощью команд:

```sh
$ go version
go version go1.5.1 darwin/amd64
$ echo $GOPATH
~unknwon/go
```
Для Windows:

```sh
$ echo %GOPATH%
~unknwon/go
```
Минимальная версия Go **1.3**.

После этого можно установить Peach, выполнив следующую команду:

```sh
go get github.com/peachdocs/peach
```

Для обновления Peach используется флаг `-u`:

```sh
go get -u github.com/peachdocs/peach
```

Для проверки установленной версии Peach используйте команду (при условии, что `$GOPATH/bin` был добавлен в `$PATH`):

```sh
$ peach -v
Peach version 0.9.2.1214
```
