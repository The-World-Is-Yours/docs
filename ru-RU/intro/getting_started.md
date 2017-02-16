---
name: Начало работы
---

# Начало работы

Давайте создадим свой первый Peach-проект!

По соглашению, каждый проект Peach должен быть назван в формате `* .peach`, для примера выберем` my.peach`

В этом примере, мы собираемся разместить наш Peach-проект в каталоге `Downloads`:

```sh
$ cd ~/Downloads
```

Затем нужно выполнить установку по умолчанию (предполагается, что `$GOPATH/bin` был добавлен к вашему` $ PATH`):

```sh
$ peach new -target=my.peach
➜  Creating 'my.peach'...
➜  Creating 'templates'...
➜  Creating 'public'...
Do you want to use custom templates?[Y/n] n
✓  Done!
```

Давайте рассмотрим, как организован наш проект:

```sh
$ cd my.peach
$ tree -L 2
.
├── conf
│   ├── app.ini
│   └── locale
├── public
│   ├── css
│   ├── fonts
│   ├── img
│   └── js
└── templates
    ├── 404.html
    ├── base.html
    ├── disqus.html
    ├── docs.html
    ├── duoshuo.html
    ├── footer.html
    ├── home.html
    ├── navbar.html
    └── search.html
```

Great! We've got almost everything we need, except one thing: custom configuration.

To quickly get started with, we are going to use the one Peach uses, it is [open sourced on GitHub](https://github.com/peachdocs/peach.peach). :heart_eyes:

So... how do we use that?

Right, we clone it to local system, and name the directory to `custom` which Peach uses it to load all custom things.

```sh
git clone https://github.com/peachdocs/peach.peach.git custom
```

Very well! You can't wait to try it out, can you?

Why don't you now start a Peach server in current directory (in this case, it is `~/Downloads/my.peach`):

```sh
$ peach web
```

OK, Peach is now running and you should see log on your terminal:

```
[Peach] 15-10-06 19:58:44 [ INFO] Peach 0.8.0.1025
[Peach] 15-10-06 19:58:44 [ INFO] Peach Server Listen on 0.0.0.0:5556
```

Based on the log, Peach is customized itself to listen on `0.0.0.0:5556` (default is `5555`), and if you open your browser and visit http://localhost:5556/, miracle happens!

If you curious about what is in Peach's custom configuration, let me briefly explain in the `custom/app.ini` file:

```ini
# Change listen port
HTTP_PORT = 5556

[docs]
# Set documentation to a remote Git source adrress
TYPE = remote
# URL to remote Git source
TARGET = https://github.com/Unknwon/peach-docs.git
```

This should explain why we didn't do anything with documentation but we can view it automatically.

Well, let's moving forward: [Setup your documentation repository](../howto/documentation).
