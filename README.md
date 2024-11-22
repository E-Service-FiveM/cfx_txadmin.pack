# Noveks txAdmin Logs & Discord Integration Script

**Version:** 3.1.0  
**Entwickler:** Novek 
**Discord:** [Discord](https://discord.gg/8q8BnmgXq2)  

---

## 📄 Überblick

Das **Noveks Admin Logs Script** ermöglicht es Server-Administratoren, alle Administrator-Aktivitäten und Ereignisse direkt in einem Discord-Channel zu protokollieren. Es hilft dabei, die Server-Administration zu überwachen, Probleme schnell zu erkennen und die Kontrolle zu behalten.

## ⚙️ Installation

1. **Lade das Script herunter** und platziere es im **`resources`**-Ordner deines Servers.
2. **Füge das Script in der `server.cfg`** hinzu:
    ```lua
    start Noveks_AdminLogs
    ```
3. **Webhook URL einfügen**: 
   - Gehe zu deinem Discord-Server und erstelle einen Webhook in einem gewünschten Channel.
   - Kopiere die Webhook-URL und füge sie in die **`Noveks_CFG.txAdminWebhook`**-Einstellung ein.

## 🛠️ Konfiguration

Die Konfiguration erfolgt über die **`Noveks_CFG`** Tabelle im Skript. Du kannst folgende Einstellungen anpassen:

- **Webhook URL**: Die URL des Discord-Webhooks für den Log-Channel.
- **Bot Name**: Der Name des Bots, der die Logs sendet.
- **Bot Logo**: Das Logo, das der Bot beim Senden der Logs anzeigt.
- **Filter Announcements**: Schalte die Anzeige von Admin-Ankündigungen ein oder aus.
- **Sprache (locale)**: Stelle die Sprache des Skripts auf Englisch (en) oder Deutsch (de) um.

### Beispiel-Konfiguration:

```lua
Noveks_CFG = {}

-- Webhook URL (Discord)
Noveks_CFG.txAdminWebhook = 'DEIN_DISCORD_WEBHOOK_URL'

-- Bot Einstellungen
Noveks_CFG.Username = 'TxAdminLogs'
Noveks_CFG.Logo = 'https://dein-bot-logo-link.png'

-- Filter Announcements (true = nur Admin-Ankündigungen anzeigen)
Noveks_CFG.FilterAnnouncements = true

-- Spracheinstellungen
Noveks_CFG.locale = 'en' -- oder 'de' für Deutsch
```

## 🌍 Sprachen

Aktuell wird das Skript in folgenden Sprachen unterstützt:
- Englisch (`en`)
- Deutsch (`de`)

## 📢 Weitere Features

- **Echtzeit-Logs**: Alle Admin-Aktionen werden direkt an den Discord-Channel gesendet.
- **Benutzerdefinierbare Einstellungen**: Lege den Namen und das Logo des Bots fest, um es deinem Server-Stil anzupassen.
- **Admin-Filter**: Filtere, welche Admin-Aktivitäten und Ankündigungen angezeigt werden sollen.

## 🚀 Wie funktioniert es?

1. Das Skript überwacht alle Admin-Aktionen auf deinem Server.
2. Bei einer Admin-Aktion wird eine Nachricht mit den Details der Aktion an den Discord-Webhook gesendet.
3. Du kannst die Art der Informationen und den Bot, der diese Nachrichten sendet, nach deinen Wünschen konfigurieren.

## 💬 Hilfe & Support

Wenn du Unterstützung benötigst oder Fragen hast, kannst du uns jederzeit über unseren **Discord-Server** kontaktieren:  
[Noveks Support-Discord](https://discord.gg/8q8BnmgXq2).

---

## 📑 Lizenz

Dieses Skript ist Open-Source und darf frei verwendet und angepasst werden, solange du die Lizenzbedingungen einhältst.  
Bitte respektiere die Nutzungsbedingungen und verwende das Skript nur auf deinem eigenen Server.

---

**Viel Spaß mit deinem neuen Admin-Log-System!** ✨
