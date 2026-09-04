---
type: feature
project: uMontage
series: umontage
title: uMontage Control v1 — единый центр управления разработкой
version: 0.3.0-alpha.10.1
queued_at: 2026-09-04T09:31:00Z
repo_url: https://github.com/sunpole/uMontage-releases
image: 2026-09-04-umontage-control-v1-update.png
image_origin: real
---

В uMontage появился единый Control v1 для рабочего цикла разработки.

Что сделано:
— GitHub Sync выполняется одной командой;
— все safety-тесты запускаются из одного меню;
— Release package, PlanOnly и Safe release rehearsal собраны в одну цепочку;
— короткий ChatGPT report заменяет огромные консольные логи;
— временные отчёты получают уникальные имена до миллисекунд и не блокируют меню.

Статус:
Control v1 уже проверен на рабочем Windows/CorelDRAW окружении: sync, тесты,
сборка alpha.10-пакета и PlanOnly проходят успешно.

Короткий текст для Telegram:

Обновление uMontage: Control v1 объединяет GitHub Sync, тесты, сборку пакета,
PlanOnly и короткий диагностический отчёт в одном меню. Теперь рабочий цикл
можно запускать без копирования длинных PowerShell-команд.
