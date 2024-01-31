# CLIENT_MISSING_INTENTS veya ClientMissingIntents hatası

Hata örneği:

![Örnek](./images/missingIntents.jpg)

Hatayı alma sebebiniz:

```js
const { Client } = require("discord.js");
const client = new Client(); // Burasının bu şekilde bırakılması
```

Örnek çözüm:

```js
const { Client, GatewayIntentBits } = require("discord.js");
const INTENTS = Object.values(GatewayIntentBits); // Tüm intentleri açar

const client = new Client({ intents: INTENTS });
```
