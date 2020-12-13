# TeamsBotSSO

Bot Framework v4 Teams bot single sign on (SSO) authentication sample.

This bot has been created using [Bot Framework](https://dev.botframework.com), it shows how to add the [Single Sign On (SSO)](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-concept-sso?view=azure-bot-service-4.0) authentication for Microsoft Teams.

The sample uses the bot authentication capabilities in [Azure Bot Service](https://docs.botframework.com), providing SSO feature to make it easier to develop a bot that authenticates users. Currently, only the [Azure AD v2](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-concept-identity-providers?view=azure-bot-service-4.0&tabs=adv1%2Cga2#azure-active-directory-identity-provider) identity provider is supported.

> IMPORTANT: The manifest file in this app adds "token.botframework.com" to the list of `validDomains`. This must be included in any bot that uses the Bot Framework OAuth flow.

## Prerequisites

- [.NET Core SDK](https://dotnet.microsoft.com/download) version 3.1

 ```bash
  # determine dotnet version
  dotnet --version
  ```
## To try this sample

- Clone the repository

    ```bash
    git clone https://github.com/Mallipriya-MSFT/TeamsSSOBot.git
    ```

- Deploy your bot to Azure, see [Deploy your bot to Azure](https://aka.ms/azuredeployment)

- [Add Single sign on to your bot via Azure Bot Service](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-authentication-sso?view=azure-bot-service-4.0&tabs=csharp)

After Authentication has been configured via Azure Bot Service, you can test the bot.

- Run the bot from a terminal or from Visual Studio:

  A) In a terminal, navigate to `TeamsBotSSO`

    ```bash
    # change into project folder
    cd TeamsBotSSO    
    # run the bot
  dotnet run
  ```

  B) Or from Visual Studio

  - Launch Visual Studio
  - File -> Open -> Project/Solution
  - Navigate to `TeamsBotSSO` folder
  - Select `TeamsBotSSO.csproj` file
  - Press `F5` to run the project

## Testing the bot using Bot Framework Emulator

[Bot Framework Emulator](https://github.com/microsoft/botframework-emulator) is a desktop application that allows bot developers to test and debug their bots on localhost or running remotely through a tunnel.

- Install the latest Bot Framework Emulator version 4.3.0 or greater from [here](https://github.com/Microsoft/BotFramework-Emulator/releases)

### Connect to the bot using Bot Framework Emulator

- Launch Bot Framework Emulator
- File -> Open Bot
- Enter a Bot URL of `http://localhost:3978/api/messages`

## Interacting with the bot

This sample uses bot authentication capabilities in Azure Bot Service, providing features to make it easier to develop a bot that authenticates users to various identity providers such as Azure AD (Azure Active Directory), GitHub, Uber, etc. These updates also take steps towards an improved user experience by eliminating the magic code verification for some clients.

## Deploy the bot to Azure

To learn more about deploying a bot to Azure, see [Deploy your bot to Azure](https://aka.ms/azuredeployment) for a complete list of deployment instructions.

## Further reading

- [Bot Framework Documentation](https://docs.botframework.com)
- [Bot Basics](https://docs.microsoft.com/azure/bot-service/bot-builder-basics?view=azure-bot-service-4.0)
- [Azure Portal](https://portal.azure.com)
- [Add Authentication to Your Bot Via Azure Bot Service](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-authentication?view=azure-bot-service-4.0&tabs=csharp)
- [Activity processing](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-concept-activity-processing?view=azure-bot-service-4.0)
- [Azure Bot Service Introduction](https://docs.microsoft.com/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-4.0)
- [Azure Bot Service Documentation](https://docs.microsoft.com/azure/bot-service/?view=azure-bot-service-4.0)
- [.NET Core CLI tools](https://docs.microsoft.com/en-us/dotnet/core/tools/?tabs=netcore2x)
- [Azure CLI](https://docs.microsoft.com/cli/azure/?view=azure-cli-latest)
- [Azure Portal](https://portal.azure.com)
- [Language Understanding using LUIS](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/)
- [Channels and Bot Connector Service](https://docs.microsoft.com/en-us/azure/bot-service/bot-concepts?view=azure-bot-service-4.0)
