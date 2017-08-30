# Frequently asked questions (Microsoft Teams developer platform)

## Setting up

### What technology should I use to build my bot or tab?

Because tabs are web content that you build and deploy, you can use any technology you want.  

As bots must be built with the Bot Framework, we recommend you use one of the languages supported by the SDKs provided by the framework:  .NET/C# or Node.js. Although the Bot Framework also provides REST APIs usable by any language you choose, the SDKs provide additional functionality and helper functions to make the development process easier.

### Where do I sign up to start building Teams apps?

There are no prerequisites or additional development accounts to start building apps for Microsoft Teams. Although you must have access to Microsoft Teams via an Office 365 subscription, no other sign-up or program access is required. You do need to create accounts for the Bot Framework if you build a bot and create a Dev Center account if you submit your app for publication.

## Bots

### How can my bot access or listen to all messages in a channel?

Bots in channels only receive messages when they are explicitly @mentioned. There is no way to grant your bot access to conversations in which they are not mentioned.

## Distribution

### How can I distribute my Microsoft Teams app?

Microsoft Teams apps can be distributed to end users via the Office Store and the in-product app-discovery system. For more information, see [Publish your Microsoft Teams app to the Office Store](submission.md).

Microsoft Teams app packages can be manually distributed to your colleagues or other end users and sideloaded by them via the [sideloading process](sideload.md). Please note that apps distributed in this format are not tested, validated, or trusted by Microsoft.

### What account do I use to create an Office Store or Dev Center account?

A Microsoft Store developer account is based on a [Microsoft account](https://account.microsoft.com/account), so you should use an existing Microsoft account or create one for this purpose.

If you already have a Windows Store developer account, you must use the original owner Microsoft account for the Seller Dashboard experience. Although the Windows Store portal allows Azure Active Directory association, the Seller Dashboard is a separate system that works only with your original Microsoft account.

---

>Not seeing your question?  Submit your own; we listen to the developer community across [several channels](feedback.md).
