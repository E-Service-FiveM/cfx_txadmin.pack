# Noveks txAdmin Logs & Discord Integration Script

**Version:** 3.2.2 
**Developer:** Novek  
**Discord:** [Discord](https://discord.gg/8q8BnmgXq2)  
**Tebex-Store** [Buy-Here](https://noveks-workspace.tebex.io/package/6551861)
---

## 📄 Overview

The **Noveks Admin Logs Script** allows server administrators to log all admin activities and events directly to a Discord channel. It helps to monitor server administration, quickly identify issues, and maintain control.

## ⚙️ Installation

1. **Download the script** and place it in the **`resources`** folder of your server.
2. **Add the script to `server.cfg`**:
    ```lua
    ensure Noveks_AdminLogs
    ```
3. **Insert Webhook URL**:
   - Go to your Discord server and create a webhook in a desired channel.
   - Copy the webhook URL and paste it into the **`Noveks_CFG.txAdminWebhook`** setting.

## 🛠️ Configuration

Configuration is done via the **`Noveks_CFG`** table in the script. You can adjust the following settings:

- **Webhook URL**: The Discord webhook URL for the log channel.
- **Bot Name**: The name of the bot that sends the logs.
- **Bot Logo**: The logo that appears when the bot sends logs.
- **Filter Announcements**: Enable or disable the display of admin announcements.
- **Language (locale)**: Set the script language to English (en) or German (de).

### Example Configuration:

```lua
Noveks_CFG = {}

-- ================================================ =========================
-- Webhook URL (Discord)
Noveks_CFG.txAdminWebhook = 'YOUR_DISCORD_WEBHOOK_URL' -- <-- Insert webhook here

-- ================================================ =========================
-- Bot settings
Noveks_CFG.Username = 'TxAdminLogs' -- Name of the Bot on your Discord Server
Noveks_CFG.Logo = 'https://your-bot-logo-link.png' -- <-- URL for the server logo

-- ================================================ =========================
-- Filter Announcements: true = show only admin announcements
Noveks_CFG.FilterAnnouncements = true -- true/false to filter announcements
-- ================================================ =========================
-- Language settings
Noveks_CFG.locale = 'en' -- [en]for English -/- [de] for German
```

## 🌍 Languages

Currently, the script supports the following languages:
- English (`en`)
- German (`de`)

## 📢 Additional Features

- **Real-time Logs**: All admin actions are sent directly to the Discord channel.
- **Customizable Settings**: Set the bot's name and logo to match your server's style.
- **Admin Filter**: Filter which admin activities and announcements are displayed.

## 🚀 How it Works

1. The script monitors all admin actions on your server.
2. When an admin action occurs, a message with the action details is sent to the Discord webhook.
3. You can customize the type of information and the bot sending the messages according to your preferences.

## 💬 Help & Support

If you need assistance or have questions, feel free to contact us anytime via our **Discord server**:  
[Noveks Support Discord](https://discord.gg/8q8BnmgXq2).


### 📑 License

This script is **not open-source** and may only be used under the following conditions:

- **Usage**: You may only use the script on your own server. Redistribution, resale, or distribution on other servers is prohibited unless explicitly authorized by the developer.
- **Modifications**: You are not permitted to modify or distribute the script unless explicitly granted permission by the developer.
- **Escrow**: If the script is part of an escrow service (such as Tebex), usage and licensing terms may be governed by the rules of the escrow platform. Ensure that you comply with all relevant terms and conditions.
- **Commercial Use**: The script may not be used for commercial purposes without express consent from the developer. Any resale or redistribution is subject to the developer’s licensing terms.
  
Please respect the license terms and ensure the script is only used on your own server as permitted.

This reflects the idea that the script is not open-source and imposes more restrictions on use and modification. If you'd like to make any more adjustments or need further information, let me know!

**Enjoy your new admin log system!** ✨
