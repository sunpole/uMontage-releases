---
type: release
project: uMontage
series: umontage
title: uMontage v1.0.0 — первый стабильный релиз
version: 1.0.0
queued_at: 2026-09-07T16:22:00Z
repo_url: https://github.com/sunpole/uMontage-releases
image: 2026-09-07-umontage-v1-0-0-release.png
image_origin: real
---

uMontage дошёл до v1.0.0 после большой серии разработки и полевых проверок
непосредственно в CorelDRAW.

Что вошло:
— новая Docker/VBA-архитектура и bridge API 11;
— создание и управляемое обновление монтажной формы;
— геометрия формы, листа, захвата и направляющих;
— реальные CMYK, Spot и Pantone-краски и сканирование красок документа;
— производственные кресты, шкалы, подписи, образцы и МБР;
— диагностика соединения Docker ↔ VBA;
— безопасная установка с backup, SHA-256 и rollback;
— uMontage Control, тесты, release rehearsal и GitHub-first процесс.

Финальный релиз собирался один раз. Один и тот же ZIP без пересборки прошёл
установку и холодный запуск на CorelDRAW 2024 (major 25) и CorelDRAW 2026
(major 27).

v1.0.0 зафиксирован отдельным tag и frozen release-branch. Следующие изменения,
включая миграцию режимов слоёв и укрепление release publisher, уже вынесены
в v1.1.0.

Короткий текст для Telegram:

uMontage v1.0.0 выпущен. Первый стабильный релиз новой Docker/VBA-архитектуры
прошёл полевую проверку на CorelDRAW 2024 и 2026 одним и тем же релизным ZIP.
Внутри — формы, геометрия, реальные Spot/Pantone-краски, производственные
метки, диагностика и безопасная установка с проверкой SHA-256 и rollback.
