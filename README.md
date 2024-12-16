# Cara membuat Bot Discord menggunakan Javascript ([Discord.Js](https://github.com/discordjs/discord.js/releases))

🧾Note: **This documentation will use Indonesian language**
___

## Rekomendasi setting

- Telah mengaktifkan `Developer Mode`
Hal ini akan berguna ketika kita membutuhkan sebuah ID: (Pengguna, Channel, Threads, Server) dan lain sebagainya secara cepat.
- Telah login pada website [Discord Developer Portal](https://discord.com/developers).

## Langkah 1 - Membuat Bot

Buka website **[Discord Developer Portal](https://discord.com/developers)** dan pilih **New Aplication**
- Masuk pada Aplication/Bot
- Pilih menu **Bot**
- Cari bagian **"Privileged Gateway Intents"**
- Nyalakan beberapa Intents dibawah ini:

> 1. **Presence Intent**<br>
Required for your bot to receive [Presence Update](https://discord.com/developers/docs/events/gateway#presence-update) events.

NOTE: Once your bot reaches 100 or more servers, this will require verification and approval. [**Read more here**](https://support-dev.discord.com/hc/en-us/articles/6205754771351)

>2. **Server Members Intent**<br>
Required for your bot to receive events listed under [GUILD_MEMBERS](https://discord.com/developers/docs/events/gateway#list-of-intents).

NOTE: Once your bot reaches 100 or more servers, this will require verification and approval. [**Read more here**](https://support-dev.discord.com/hc/en-us/articles/6205754771351)

>3. **Message Content Intent**<br>
Required for your bot to receive [message content](https://support-dev.discord.com/hc/en-us/articles/4404772028055) in most messages.

NOTE: Once your bot reaches 100 or more servers, this will require verification and approval. [**Read more here**](https://support-dev.discord.com/hc/en-us/articles/6205754771351)

<br>

Invite Bot ke server:

- Masuk ke-Menu **Installation** <br>
Installation Contexts
Select the installation contexts your app supports. Apps can be installed to both users and guilds.

- Pilih **Guild Install** <br>
Install Link
Use our provided install link or register a custom one. If you choose a custom link, users who add your app will be redirected to your URL instead of the Add App flow in Discord.

- Pilih **Discord Provided Link**

- Pilih **Scopes**: `aplications.commands`, `bot` - lalu **Permissions**: `Administrator` mencakup semua izin yang ada.
- Salin link yang sudah di sediakan dan masukkan Bot ke server.


## Langkah 2 - Memprogram Bot
