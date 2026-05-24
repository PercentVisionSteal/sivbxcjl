# Калькулятор (Android)

Простое Android-приложение — обёртка-WebView над HTML-калькулятором.

## Возможности
- +, −, ×, ÷, %
- Тёмная тема, тач-кнопки, аккуратный UI
- `assets/calculator.html` — собственно калькулятор

## Сборка APK

APK собирается автоматически в GitHub Actions при пуше в `main`.

- Воркфлоу: `.github/workflows/build.yml`
- Готовый файл публикуется в **Release `latest`**:
  https://github.com/PercentVisionSteal/sivbxcjl/releases/tag/latest
- Также доступен как артефакт `calculator-apk` в Actions.

### Локальная сборка
```bash
gradle wrapper --gradle-version 8.7
./gradlew :app:assembleDebug
# APK: app/build/outputs/apk/debug/app-debug.apk
```

## Установка APK на телефоне
1. Скачать `calculator-debug.apk` из релиза.
2. Включить «Установка из неизвестных источников» в настройках браузера/файлового менеджера.
3. Открыть `.apk` и установить.
