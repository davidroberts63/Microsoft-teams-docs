# Create a bot for Microsoft Teams

All bots created using the Microsoft Bot Framework are configured and ready to work in Microsoft Teams.

See the [Bot Framework Documentation](https://docs.botframework.com/en-us/) for more information about the following:

1. Register the bot with the [Bot Framework](https://dev.botframework.com/), being sure to add Microsoft Teams as a channel and that you re-use any Microsoft app ID you generated if you've already created your app package/manifest.

   ![Bot Framework registration page](images/Bot/BFRegister.PNG)

2. Build the bot using the [Microsoft.Bot.Connector.Teams](https://www.nuget.org/packages/Microsoft.Bot.Connector.Teams) NuGet package, the [botbuilder-teams](https://www.npmjs.com/package/botbuilder-teams) npm package, or the [Bot Connector API](https://docs.microsoft.com/en-us/bot-framework/rest-api/bot-framework-rest-connector-api-reference).

3. Test the bot using the [Bot Framework Emulator](https://docs.microsoft.com/en-us/bot-framework/debug-bots-emulator).

4. Deploy the bot to a cloud service, such as [Microsoft Azure](https://azure.microsoft.com/).

To make your bot experience Teams-ready:

1. [Create a sideloadable bot package](createpackage.md) and [sideload it to a team](sideload.md) to test it in action.
2. Add [tabs](tabs.md) or [other capabilities](index.md) to make your experience shine in Teams.
3. [Submit your final app package](submission.md) for publication in the Office Store.
