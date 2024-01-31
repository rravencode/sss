# ...cannot be loaded because running scripts... hatası

Hatayı alma sebebiniz:

- Windows varsayılan olarak internetten indirilen PowerShell scriptlerini çalıştırmayı engeller. Bu ayar npx veya npm gibi bazı programların rahatça çalışmasını engeller.

Hatayı nasıl çözersiniz:

- Arama kısmından **PowerShell**'i aratıp yönetici olarak çalıştırın.
- Konsola **Set-ExecutionPolicy -ExecutionPolicy RemoteSigned** yazıp entera basın.
- Çıkan mesaja **y** yazıp entera basın ve pencereyi kapatın.
