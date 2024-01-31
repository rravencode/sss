# Check /app/package.json: command not found hatası

Hatayı alma sebebiniz:

- Glitch veya Replit gibi bir ortamlarda botu başlatmak için varsayılan olarak **npm start** kullanılır ve package.json dosyanızda bu komut çalıştırılınca ne yapılacağınız yazmazsanız botu başlatamaz.
- **Not**: Genellikle kendiniz bir proje oluştururken **npm init** kullandıysanız veya hazır altyapı aldıysanız start komutu bulunur.

Hatayı nasıl çözersiniz:

- package.json dosyanıza aşağıdakini ekleyin. **Eklenecek yerden önceki satırın sonuna örnekteki gibi virgül koymayı unutmayın!**

```json
"scripts": {
  "start": "node ."
}
```

- Örnek package.json:

```json
{
  "name": "bot",
  "version": "1.0.0",
  "main": "./index.js",
  "scripts": {
    "start": "node ."
  },
  "license": "MIT",
  "dependencies": {
    "discord.js": "^14.14.1"
  }
}
```
