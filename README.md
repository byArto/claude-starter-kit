# Стартер-кит byArto для Claude Code

8 моих команд для Claude Code на русском. Ставятся один раз и работают во всех проектах.

## Установка

В Claude Code выполнить по очереди:

```
/plugin marketplace add byArto/claude-starter-kit
/plugin install byarto@byarto-kit
```

Команды вызываются с префиксом, например: `/byarto:plan сделать страницу с отзывами`.

## Команды

| Команда | Что делает |
|---|---|
| `/byarto:start` | Создаёт CLAUDE.md по шаблону |
| `/byarto:plan` | Задаёт вопросы и предлагает план, ничего не меняет до «ок» |
| `/byarto:fix` | Находит причину ошибки, чинит минимальной правкой и проверяет |
| `/byarto:explain` | Объясняет код или последние изменения простыми словами |
| `/byarto:design` | Делает интерфейс «сочным» и проверяет его на телефоне |
| `/byarto:check` | Строгое ревью: баги, безопасность, лишняя сложность |
| `/byarto:save` | Проверяет проект, делает git-коммит и заметку в NOTES.md |
| `/byarto:ship` | Готовит выкладку: сборка, переменные окружения, инструкция |

Команды запускаешь только ты — сам Claude их не вызывает. Ревью называется `check`, а не `review`: у Claude Code уже есть встроенный `/review`.

## Без плагина

Скопируй папки из `plugins/byarto/skills/` в `~/.claude/skills/`. Тогда команды будут без префикса: `/plan`, `/fix` и так далее.

```bash
git clone https://github.com/byArto/claude-starter-kit.git
mkdir -p ~/.claude/skills
cp -R claude-starter-kit/plugins/byarto/skills/* ~/.claude/skills/
```

Шаблон CLAUDE.md лежит отдельно в [`templates/CLAUDE.md`](templates/CLAUDE.md) — его можно скопировать в проект и без команд.

## Откуда это

- 🎁 Полный стартер-пак по Claude Code — гайд из 7 шагов, 12 промптов и шпаргалки — в моём Telegram-боте: [@byartoai_bot](https://t.me/byartoai_bot?start=pack__github)
- 📢 Канал [@byarto1](https://t.me/byarto1) — разборы новых фич Claude и дневник моей MMO RPG
- 📸 Instagram [@by.arto](https://www.instagram.com/by.arto/)

## Лицензия

[MIT](LICENSE)
