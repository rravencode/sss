# @discordjs/voice paketi ile müzik oynatırken ses kesilme hatası

Hatayı nasıl çözersiniz:

- Botunuzun olduğu klasörün içindeki **node_modules** klasörünün içine girin.
- Sırayla **@discordjs**, **voice**, **dist** klasörlerine girip **index.js**'nin içine girin.

```js
addStatePacket(packet) { // Bu isimle başlayan bir fonksiyon olacak
  this.packets.state = packet;
  this.configureNetworking(); // Bu satırı ekle
  if (packet.self_deaf !== void 0)
    this.joinConfig.selfDeaf = packet.self_deaf;
  if (packet.self_mute !== void 0)
    this.joinConfig.selfMute = packet.self_mute;
  if (packet.channel_id)
    this.joinConfig.channelId = packet.channel_id;
}
```

- Üstte gösterildiği gibi değişiklikleri yapıp kaydedin ve botu yeniden başlatın.
