# Git процесс ЛР1

Проект выполняется индивидуально. Исправление первой версии оформлено через [issue #1](https://github.com/bee-crypt/confmanager/issues/1), ветку lr1-fixes, восемь коммитов и [PR #2](https://github.com/bee-crypt/confmanager/pull/2). PR проверен самостоятельно и принят в main. Тег [v0.1.0](https://github.com/bee-crypt/confmanager/tree/v0.1.0) указывает на 491d654.

Текущее упрощение оформляется отдельно через [issue #3](https://github.com/bee-crypt/confmanager/issues/3) и ветку lr1-simple. Автотесты и инструменты качества перенесены в план ЛР3; для ЛР1 остаются команды и ручные сценарии из README.

## Конфликт слияния

Ветки lr1-fixes и demo/local-checks разошлись от 312a24f. В demo/local-checks коммит b6de3f6 изменил строку проверки README на Make; в lr1-fixes коммит c59d6df изменил ту же строку на команду Python. Слияние остановилось:

```text
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.
UU README.md
```

Конфликт разрешён объединением обеих инструкций. Создан настоящий merge-коммит 75d0d5265fae0fa05a8fe867f0f288b3cd8791a4 с двумя родителями. Проверить историю можно командами:

```bash
git show --format=fuller --no-patch 75d0d52
git log --graph --oneline --all
```

Сам конфликт и его разрешение сохранены в истории, даже если текущая инструкция проверки изменяется.

## Даты

Даты коммитов вручную установлены на 8–10 сентября 2026 года по запросу владельца; issue и PR сохраняют реальные даты. Исходная история и опубликованный тег не переписываются.
