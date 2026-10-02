# gleboboss

Скилл для Codex и Claude Code. Агент начинает разговаривать по-пацански:
коротко, уверенно, с матерком. Работает он так же, как раньше, меняется
только манера речи.

## Установка в Codex

Открыть Терминал и вставить:

```
mkdir -p ~/.codex/skills && curl -L https://github.com/an-mnfctr/gleboboss/archive/refs/heads/main.tar.gz | tar -xz -C ~/.codex/skills --strip-components=1 gleboboss-main/gleboboss
```

Перезапустить Codex. В чате написать `$gleboboss`.

Другой способ: попросить сам Codex

```
$skill-installer установи https://github.com/an-mnfctr/gleboboss/tree/main/gleboboss
```

## Установка в Claude Code

```
mkdir -p ~/.claude/skills && curl -L https://github.com/an-mnfctr/gleboboss/archive/refs/heads/main.tar.gz | tar -xz -C ~/.claude/skills --strip-components=1 gleboboss-main/gleboboss
```

Перезапустить Claude Code. В чате написать `/gleboboss`.

## Установка вручную

1. Нажать зелёную кнопку **Code** → **Download ZIP**, распаковать.
2. Скопировать папку `gleboboss` (ту, где лежит `SKILL.md`) в:
   - Codex: `~/.codex/skills/`
   - Claude Code: `~/.claude/skills/`
3. Перезапустить программу.

Должно получиться `~/.codex/skills/gleboboss/SKILL.md` (или то же самое в `~/.claude`).

Папки `.codex` и `.claude` скрытые. В Finder их видно после Cmd + Shift + точка.
На Windows это `C:\Users\<имя>\.codex\skills\` и `C:\Users\<имя>\.claude\skills\`.

## Как выключить

Написать «хорош» или «нормально говори». Ещё можно просто начать новый чат.

## Обновление

Повторить команду установки, файл перезапишется.

## Удаление

```
rm -rf ~/.codex/skills/gleboboss ~/.claude/skills/gleboboss
```

## Настроить под себя

Весь характер описан в одном файле `gleboboss/SKILL.md`, это обычный текст.
Поправить, сохранить, перезапустить программу.

Имя папки и строка `name:` в начале `SKILL.md` должны совпадать.
