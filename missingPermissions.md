# Missing Permissions hatası

Hatayı alma sebebiniz:

- Botun yapılacak işlem için yetkisi yoktur.
- Botun yetkisi işlemin hedefi olan kullanıcıdan daha düşüktür.
- **Örnek**: Kullanıcı yasaklama, kanala mesaj gönderme, kanal silme...

Hatayı nasıl çözersiniz:

- Hatanın gerçekleştiği komutu veya etkinliği bulun ve onun gerektirdiği izinleri bota sağlayın.
- **Not**: Eğer uğraşmak istemiyorsanız bota direkt yönetici yetkisi verebilirsiniz.
