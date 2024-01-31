# FFmpeg/avconv not found hatası

Hatayı alma sebebiniz:

- Projenizde ve bilgisayarnızda FFmpeg yüklü olmaması.

Hatayı nasıl çözersiniz:

- Proje ve bilgisayar kapsamlı iki çözümden birini seçebilirsiniz.

1. Proje kapsamlı:
   - **npm i ffmpeg-static** ile projenize FFmpeg kurabilirsiniz.
   - Eğer başında **ERR** yazan uzunca hatalar alıyorsanız [buraya](./buildTools.md) bakınız.
2. Bilgisayar kapsamlı:
   - [FFmpeg](https://www.gyan.dev/ffmpeg/builds/ffmpeg-release-full.7z)'in son sürümünü indirin.
   - İçindeki klasörü C diskine atın ve ismini **ffmpeg** olarak değiştirin.
   - Windows'un arama çubuğuna **değişken** yazıp **Sistem ortam değişkenlerini düzenleyin** sonucuna tıklayın.
   - Açılan pencerede aşağıda **Ortam Değişkenleri** yazısına tıklayın.
   - **(Kullanıcı adı) için kullanıcı değişkenleri** tablosunda **Path** yazısına iki kez tıklayın.
   - Açılan pencerede boş bir satıra iki kez tıklayıp **C:\ffmpeg\bin** yazın ve enter tuşuna basın.
   - Pencereleri **Tamam** deyip kapatın. (**Uygula** yazısı aktifse en son pencerede ona tıklayın)
   - Terminali kapatıp tekrar açın ve konsola **ffmpeg** yazın. Eğer uzunca gri/beyaz yazılar çıkıyorsa indirme başarılıdır.
