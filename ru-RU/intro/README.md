---
name: Введение
---

# Peach

Peach — веб-сервер мультиязычной документации с возможностью поиска и синхронизации в реальном времени.

## Обоснование

Существует достаточное количество инструментов для создания веб-документации, но в течение долгого времени ни один из этих инструментов не удовлетворил мою потребность в размещении мультипроектной докуентации на веб-сайте. Я искал общее и настраиваемое решение. Это и послужило причиной создания Peach.

В приведенной ниже таблице показаны основные различия между Peach и другими существующими инструментами (концепции могут отличаться от того, что я понимаю):

| Название | Размещение на своем хостинге | Мультиязычность | Синхронизация в реальном времени | Статический HTML | Контроль версий|
|:--:|:---------:|:------------:|:------------:|:---------:|:---------:|
|Peach|✅|✅|✅|✅(Кэшируемый)|[Дорожная карта](/docs/intro/roadmap)|
|Mkdocs|✅|❌|❌|✅|❌|
|Read The Docs|❌|✅|✅|✅|✅|


Кроме того, Peach также поддерживает следующие функции:

- Синхронизация в режие реального времени из любых исходников, размещенных в Git;
- Полнотекстовый поиск на предподчтительном языке;
- Использование Markdown разметки;
- Highly configurable without touching a single bit of Git history;
- Встроенная поддержка интеграции Disqus.


## Статус разработки

Peach is currently still in development, but can be used in production with some notes:

- Things are subject to change,
- ... but if you don't upgrade, it will keep working until the end of the world. :100:
- If you do want to upgrade, just read the documentation. :joy:

## Примеры

- [Peach Docs](http://peachdocs.org/): [peach.peach](https://github.com/peachdocs/peach.peach)
- [Gogs Docs](http://gogs.io/): [gogsweb.peach](https://github.com/gogits/gogsweb.peach)
- [Macaron Docs](http://go-macaron.com/): [macaron.peach](https://github.com/macaron-contrib/macaron.peach)
- [Blade Docs](http://bladejava.com/): [blade.peach](https://github.com/bladejava/blade.peach)
