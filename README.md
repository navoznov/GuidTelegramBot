# GuidTelegramBot

Telegram-бот, который генерирует GUID. На любое сообщение он отвечает новым GUID, на `help` или `/help` — короткой подсказкой.

## Состав

Решение `GuidTelegramBot.sln` для .NET Framework 4.5.1 и Windows, четыре проекта:

- `GuidTelegramBot.Core` — сам бот: опрашивает Telegram раз в секунду и отвечает на сообщения.
- `GuidTelegramBot.Console` — консольное приложение, пишет входящие сообщения в консоль.
- `GuidTelegramBot.WinApp` — приложение Windows Forms с кнопками «Старт» и «Стоп» и логом сообщений, сворачивается в трей.
- `GuidTelegramBot.WindowsService` — бот в виде службы Windows.

Бот использует [Telegram.Bot](https://github.com/TelegramBots/Telegram.Bot) 9.0.

## Запуск

1. Создайте бота у [@BotFather](https://t.me/BotFather) и получите токен.
2. Пропишите токен в ключе `apiToken` в `app.config` (или `App.config`) того приложения, которое будете запускать.
3. Откройте `GuidTelegramBot.sln` в Visual Studio, восстановите NuGet-пакеты и запустите нужный проект.

## Лицензия

[MIT](LICENSE)
