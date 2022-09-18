# Fazz | Registry Giriş

**Kayıt Defteri Yönetimi (Registry Management)**

* İşletim sistemi, uygulama ve donanımların ayarlarını barındıran bir veritabanıdır.
* Bilgiler, ayarlar, seçenekler ve diğer değerleri içerir.
* İşletim sistemi ve bileşenleri, nasıl davranması gerektiğini buradan okur.
* Bu veritabanının dosyaları C:\Windows\System32\Config klasörü altında tutulur.
* Run (Çalıştır)’da veya CMD (Komut İstemcisi)’de Regedit yazılarak başlatılabilir.
* Değişiklikler kalıcı hasara yol açabileceği için yedek (backup) alınarak çalışılması gerekir.
* Registry dosyaları .reg uzantılıdır.

**Registry 5 bölümden oluşur.**

1) HKEY_CLASSES_ROOT: Burada dosya türleri ve OLE (Object Linking and Embedding) bilgileri saklanır.
Dosya türleri için OLE kullanan uygulamalar, bilgileri buradan okur.
2) HKEY_CURRENT_USER: O an için oturum açmış kullanıcıya ait ayar ve seçenek bilgileri burada tutulur.
3) HKEY_LOCAL_MACHINE: Bilgisayara ait ayar ve seçenekler burada tutulur.
4) HKEY_USERS: Kullanıcıların geneline ait ayar ve seçenekler burada tutulur.
5) HKEY_CURRENT_CONFIG: O an için oturum açmış kullanıcıya özel donanım ayar ve seçenekleri burada tutulur.

**Registry'de 2 tip *veri* tipi vardır.**

1) Key (Anahtar): Değerleri barındıran ve çalıştıran ana konumlardır.
(Değerlerin klasörleri denebilir.)
2) Value (Değer): Değerlerdir. Key’lerin altında bulunurlar.
Üçe ayrılırlar.

* String : Dizgi şeklindeki değerlerdir. Karakterlerden oluşur, metinseldir
* Binary: İkilik (Binary) gösterimli sayısal değerlerdir.
* DWORD/QWORD Ondalık (decimal) ve onaltılık (hexadecimal) gösterimli değerlerdir.
DWORD, 32 bit’lik bir decimal veya hexadecimal değerdir.
QWORD, 64 bit’lik bir decimal veya hexadecimal değerdir.

**Bir Registry dosyasının içeri şöyledir:**

*Windows Registry Editor Version 5.00*

[Topluluk (Hive) Adı\Key Adı\Alt (Sub) Key Adı]

*   Değer (Value) Adı=Değer Tipi:Değer Verisi

<h2> Menü </h3>

| Notes  |
| ------------- |
| [Server Systems](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/ServerSystems.md) |
| [Network](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/network.md) |
| [Windows](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/windows.md) |
| [DNS](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/DNS.md) |
| [CMD](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/CMD.md) |
| [Regedit-Anonim](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/Anonim-Settings.md) |
| [Regedit-Performance](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/Performance-Settings.md) |
| [Regedit-Clean](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/Registry-Clear.md) |
| [Regedit-Startup](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/Startup-Program.md) |
| [Tor-Hosting](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/TorHosting.md) |
| [Usb-Ignore](https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/Usb-Ignore.md) |
