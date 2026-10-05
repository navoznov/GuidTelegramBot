# GuidTelegramBot

A Telegram bot that generates GUIDs. It replies to any message with a new GUID, and to `help` or `/help` with a short hint.

## Projects

The `GuidTelegramBot.sln` solution targets .NET Framework 4.5.1 on Windows and has four projects:

- `GuidTelegramBot.Core`: the bot itself. It polls Telegram once a second and replies to messages.
- `GuidTelegramBot.Console`: a console app that prints incoming messages.
- `GuidTelegramBot.WinApp`: a Windows Forms app with Start and Stop buttons and a message log. It minimizes to the tray.
- `GuidTelegramBot.WindowsService`: the bot as a Windows service.

The bot uses [Telegram.Bot](https://github.com/TelegramBots/Telegram.Bot) 9.0.

## Running

1. Create a bot with [@BotFather](https://t.me/BotFather) and get its token.
2. Put the token into the `apiToken` key in the `app.config` (or `App.config`) of the app you're going to run.
3. Open `GuidTelegramBot.sln` in Visual Studio, restore the NuGet packages and run the project you need.

## License

[MIT](LICENSE)
