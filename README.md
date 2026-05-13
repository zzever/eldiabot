# 📰 ElDiaBot

Bot de Telegram que publica automáticamente las noticias del periódico **La Opinión de Tenerife** a través de un canal RSS.

📢 Canal de Telegram: [@eldia_laopiniondetenerife](https://t.me/eldia_laopiniondetenerife)

---

## ¿Qué hace?

ElDiaBot es un bot automatizado que:

- Monitoriza el feed RSS de La Opinión de Tenerife
- Publica automáticamente las nuevas noticias en el canal de Telegram
- Evita duplicados comprobando las noticias ya publicadas
- Funciona de forma continua en segundo plano

---

## 🛠️ Tecnologías

- **Node.js** — entorno de ejecución
- **Telegraf** o `node-telegram-bot-api` — integración con la API de Telegram
- **RSS Parser** — lectura del feed RSS
- **Cron / setInterval** — ejecución periódica

---

## 🚀 Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/zzever/Eldiabot.git
   cd Eldiabot
   ```

2. Instala las dependencias:
   ```bash
   npm install
   ```

3. Crea un archivo `.env` con tu token de bot de Telegram:
   ```env
   BOT_TOKEN=tu_token_aqui
   CHANNEL_ID=@eldia_laopiniondetenerife
   ```

4. Inicia el bot:
   ```bash
   node index.js
   ```

---

## ⚙️ Configuración

| Variable        | Descripción                              |
|-----------------|------------------------------------------|
| `BOT_TOKEN`     | Token del bot obtenido desde @BotFather  |
| `CHANNEL_ID`    | ID o username del canal de Telegram      |
| `RSS_URL`       | URL del feed RSS a monitorizar           |
| `INTERVAL`      | Intervalo de comprobación (en minutos)   |

---

## 📄 Licencia

MIT © [zzever](https://github.com/zzever)
