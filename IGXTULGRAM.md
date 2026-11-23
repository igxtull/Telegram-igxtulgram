# igxtulGram build

Этот форк официального Telegram Android с интегрированным модом
[igxtulGram](https://github.com/igxtull/igxtulgram).

## Что добавлено

- Исходники мода: `TMessagesProj/src/main/java/com/igxtul/gram/`
- Инициализация в `LaunchActivity.onCreate()`
- Кнопка **iGX** в правом верхнем углу — открывает настройки мода
- Тонировка пузырей в `ChatMessageCell.drawBackground()`
- `ModSettingsActivity` зарегистрирован в манифесте
- Workflow `.github/workflows/build-igxtulgram.yml` собирает debug APK

## Сборка

Нажмите **Actions → Build igxtulGram Telegram → Run workflow**, либо сделайте
push в `master`. APK появится в артефактах запуска как `igxtulgram-telegram-apk`.

Сборка использует официальный исходник, SDK 36, NDK 27.2.12479018 и все
сабмодули. Первый запуск занимает длительное время из-за нативной части.

Мод не читает и не отправляет сообщения — только меняет внешний вид.
Не используйте официальное название и логотип Telegram при публикации.
