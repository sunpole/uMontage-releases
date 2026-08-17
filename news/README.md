# Заметки для uNews

`sunpole/uNews` автоматически сканирует этот публичный репозиторий. Для
каждого подтверждённого публичного релиза uMontage добавляйте одну заметку и
один проверенный визуальный материал. Не создавайте датированную заметку для
внутреннего checkpoint, полевого кандидата или неопубликованной сборки.

## Обязательная пара файлов

```text
news/YYYY-MM-DD-umontage-vX-Y-Z-short-title.md
news/YYYY-MM-DD-umontage-vX-Y-Z-short-title.png
```

Имя должно быть на латинице; основа имени Markdown-файла и картинки должна
совпадать. Установочный ZIP остаётся в GitHub Releases. Не добавляйте сюда
GMS, исходный код, CDR/PDF клиентов, credentials или локальные backup.

## Обязательный YAML

```yaml
---
type: release
project: uMontage
series: umontage
title: Краткое русское описание подтверждённого релиза
version: 0.3.0
queued_at: 2026-08-17T12:00:00Z
repo_url: https://github.com/sunpole/uMontage-releases
image: YYYY-MM-DD-umontage-v0-3-0-short-title.png
---
```

`queued_at` ставится в реальное UTC-время создания публичной заметки. Описывайте
только фактически выпущенные изменения. Не вставляйте в текст URL и хештеги:
единую ссылку и footer добавляет policy uNews. В Telegram отправляет только
GitHub Actions из uNews, а не локальный компьютер.

## Порядок публикации

1. Опубликовать проверенный GitHub Release с manifest и checksums.
2. Добавить сюда соответствующие заметку и PNG.
3. Запустить в uNews dry-run (`Publish all project news`, `dry_run=true`).
4. Запуск с `dry_run=false` выполняется только когда заметка готова к отправке
   в Telegram.
