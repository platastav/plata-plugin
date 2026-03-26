# Plata Plugin for Claude Code

Операционная система ювелирной мастерской Plata — 10 скиллов для работы с клиентами, производством, контентом и автоматизацией.

## Установка

```bash
/plugin install plata@local --plugin-dir /var/www/plata-plugin
```

Или для тестирования:

```bash
claude --plugin-dir /var/www/plata-plugin
```

## Скиллы

| Команда | Что делает |
|---------|-----------|
| `/plata:plata-brief` | ТЗ для мастера из запроса клиента |
| `/plata:plata-offer` | Коммерческое предложение клиенту |
| `/plata:plata-reply` | Ответ на жалобу / сложную ситуацию |
| `/plata:plata-price` | Расчёт стоимости изделия |
| `/plata:plata-post` | Пост для Instagram / Telegram |
| `/plata:plata-collection` | Концепция новой коллекции |
| `/plata:plata-bizletter` | Деловое письмо партнёру |
| `/plata:plata-decide` | Анализ бизнес-решения |
| `/plata:plata-debrief` | Разбор рабочего дня |
| `/plata:plata-n8n` | Воркфлоу для автоматизации |

## Примеры

```
/plata:plata-brief кольцо из золота 585 с бриллиантом, размер 17
/plata:plata-price серьги Au585 3г + 2 бриллианта 0.1кт каждый
/plata:plata-reply клиент жалуется что заказ задержали уже на неделю
/plata:plata-post новые серьги с опалом, ig
```

## Структура

```
plata-plugin/
├── .claude-plugin/
│   └── plugin.json
└── skills/
    ├── plata-brief/SKILL.md
    ├── plata-offer/SKILL.md
    ├── plata-reply/SKILL.md
    ├── plata-price/SKILL.md
    ├── plata-post/SKILL.md
    ├── plata-collection/SKILL.md
    ├── plata-bizletter/SKILL.md
    ├── plata-decide/SKILL.md
    ├── plata-debrief/SKILL.md
    └── plata-n8n/SKILL.md
```
