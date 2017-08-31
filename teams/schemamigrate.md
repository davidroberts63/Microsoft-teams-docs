# Migrate your v0.4 manifest to v1.0 in Microsoft Teams

To support Microsoft Teams apps, we made significant changes in our manifest. If you've already built your app on the [v0.4 manifest](schemav0.4.md), here are a few tips to help in conversion:

|v0.4 object| v1.0 object| comments|
|---|---|---|
| `id`, `tabs:id`, or `bot.mri` | `id` | Use a Microsoft app ID. You'll already have one if you registerd a bot with the Bot Framework, or if your tab's web app signs in with Microsoft. Otherwise, generate a new ID at the [Microsoft App registration portal](https://apps.dev.microsoft.com). This ID uniquely represents your app moving forward and may not change once published. |
| `tabs` | `configurableTabs` | In v0.4, all `tabs` were channel/configurable tabs. In v1.0, this distinction is called out to distinguish from `staticTabs` |
| `tabs:id` | `id` | This field was deprecated in v1.0. Your GUID should migrate to the overall app `id` in v1.0. |
| `tabs:name` | `name:short`, `name:long` | Use your existing name. |
| `tabs:description` | `description` | Use your existing tab description or create new ones to represent your entire app experience. |
| `tabs:description` | `description` | Use your existing tab description or create new ones to represent your entire app experience. |
| `tabs:icons` | `icons` | Icons have been promoted to a top-level object. Note that [icons have been changed in v1.0](createpackage.md#icons) and must be included as part of the package. URLs to hosted icons are not allowed. |
| `tabs:accentColor` | `accentColor` | Accent color has been promoted to a top-level object. |
| `tabs:configUrl` | `tabs:configurationUrl` | The configurable tab's config.html file. |
| `bots:mri` | `bots:id` | Same value, the bot's Microsoft app ID as registered with the Bot Framework. |
| `bots:pinnedTabs` | `staticTabs` | Static tabs are top level objects, not children of the bot object. |
| `bots:pinnedTabs:id`, `bots:pinnedTabs:definitionId` | `staticTabs:entityId` | Static tab IDs have been collapsed into a single ID used for deep link reference. |
| `bots:pinnedTabs:displayName` | `staticTabs:name` | The static tab name in the UI. |
| `bots:pinnedTabs:url` | `staticTabs:contentUrl` | The tab content URL. |
| `needsIdentity` | `permissions: ["identity"]` | Permissions object is an array, of which `identity` is one of the values. |
