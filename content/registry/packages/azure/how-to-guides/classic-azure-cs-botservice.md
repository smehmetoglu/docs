---
title: "Azure Bot Service with Application Insights | C#"
h1: "Azure Bot Service with Application Insights"
linktitle: "Azure Bot Service with Application Insights"
no_edit_this_page: true
cloud: classic-azure
language: cs
layout: how-to-guide
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/mktutorial. -->

<p class="mb-4 flex">
    <a class="flex flex-wrap items-center rounded text-xs text-white bg-blue-600 border-2 border-blue-600 px-2 mr-2 whitespace-no-wrap hover:text-white" style="height: 32px" href="https://github.com/pulumi/examples/tree/master/classic-azure-cs-botservice" target="_blank">
        <span><i class="fab fa-github pr-2"></i> View Code</span>
    </a>
    <a href="https://app.pulumi.com/new?template=https://github.com/pulumi/examples/tree/master/classic-azure-cs-botservice" target="_blank">
        <img src="https://get.pulumi.com/new/button.svg" alt="Deploy">
    </a>
</p>


Starting point for building Azure Bot Service hosted in Azure App Service.

Provisions Azure Bot Service, Azure Bot Channel registration and Azure Application Insights to be used in combination
with App Service - registering Azure AD Microsoft Application with secret.  

This will deploy the echo bot code within the ~/bot directory - you can tweak the contents or replace the contents with your own bot.  Please ensure you publish the bot first to the ~/bot/publish subfolder - following the instructions for `Publish Bot Steps`.

## Deploying the App

To deploy your infrastructure, follow the below steps.

### Prerequisites

* [Install Pulumi](https://www.pulumi.com/docs/get-started/install/)
* [Install .NET Core 3.0+](https://dotnet.microsoft.com/download)

### Publish Bot Steps

1.  Within the **/bot** subfolder, publish the bot to subfolder called publish:

    ```bash
    $ dotnet publish -o publish
    ```

### Pulumi Steps

1.  Within the **azure-cs-botservice** folder, create a new stack:

    ```bash
    $ pulumi stack init dev
    ```

2.  Login to Azure CLI (you will be prompted to do this during deployment if you forget this step):

    ```bash
    $ az login
    ```

3.  Configure the location to deploy the resources to:

    ```bash
    $ pulumi config set azure:location "North Europe"
    ```

4.  Configure the Bot Name:

    ```bash
    $ pulumi config set botName PulumiBot1
    ```

5.  Run `pulumi up` to preview and deploy changes:

    ```bash
    $ pulumi up
    Previewing changes:
    ...

    Performing changes:
    ...
    info: 14 changes performed:
        + 14 resources created
    Update duration: 1m22s
    ```

6.  Check the deployed bot using either:
  
   * Azure Portal Azure Bot Service - [Test in Webchat feature](https://docs.microsoft.com/en-us/azure/bot-service/abs-quickstart?view=azure-bot-service-4.0#test-the-bot)
   * [Bot Framework Emulator](https://github.com/Microsoft/BotFramework-Emulator) pointing to the output bot endpoint and Microsoft Application Id and the secret you supplied:

      ```bash
      $ BotEndpoint: "https://app8asdf.azurewebsites.net/api/messages"
      $ MicrosoftAppId: "b5e65403-923c-4568-z2f6-a6f41b258azz"
      $ MicrosoftAppPassword: "<secret>"    
      ```

7.  Once you've finished, you can tear down your stack's resources by destroying and removing it:

    ```bash
    $ pulumi destroy -y
    $ pulumi stack rm -y
    ```

