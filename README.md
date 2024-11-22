# Noveks txAdmin Logs & Discord Integration Script

**Version:** 3.1.0  
**Developer:** Novek  
**Discord:** [Discord](https://discord.gg/8q8BnmgXq2)  

---

## 📄 Overview

The **Noveks Admin Logs Script** allows server administrators to log all admin activities and events directly to a Discord channel. It helps to monitor server administration, quickly identify issues, and maintain control.

## ⚙️ Installation

1. **Download the script** and place it in the **`resources`** folder of your server.
2. **Add the script to `server.cfg`**:
    ```lua
    start Noveks_AdminLogs
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

-- Webhook URL (Discord)
Noveks_CFG.txAdminWebhook = 'YOUR_DISCORD_WEBHOOK_URL'

-- Bot Settings
Noveks_CFG.Username = 'TxAdminLogs'
Noveks_CFG.Logo = 'https://your-bot-logo-link.png'

-- Filter Announcements (true = only show admin announcements)
Noveks_CFG.FilterAnnouncements = true

-- Language Settings
Noveks_CFG.locale = 'en' -- or 'de' for German
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

---

## 📑 License

This script is open-source and can be freely used and modified as long as you adhere to the license terms.  
Please respect the usage guidelines and only use the script on your own server.

---

**Enjoy your new admin log system!** ✨
