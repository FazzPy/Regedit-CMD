# İstemci İşletim Sistemleri | Windows

<h3>Sürüm Farklılıkları</h3>


<img src="https://github.com/FazzPy/System-Network/blob/main/documents/img/version1.PNG">

<img src="https://github.com/FazzPy/System-Network/blob/main/documents/img/version2.PNG">

<img src="https://github.com/FazzPy/System-Network/blob/main/documents/img/version3.PNG">

<img src="https://github.com/FazzPy/System-Network/blob/main/documents/img/version4.PNG">

<h3>Not :</h3>

Command Prompt & Regedit Notları ;

https://github.com/FazzPy/Regedit-CMD

Batch Scripting Notları ;

https://github.com/FazzPy/BatchScripting

<h3> Task Scheduler Nedir ? </h3>
  
Windows işletim sistemleri ve üçüncü parti uygulamaların görevlerini ve başlatma zamanlarını vs. ayarlayabileceğiniz bir görev zamanlayıcısıdır.
  
<h3> Event Viewer Nedir ? </h3>
  
**Event Viewer**, Windows'ta tüm olayları log olarak kaydeden ve bizlere uyarılar sunan bir hizmettir.

<h3> SMB Protokolü </h3>

**Paylaşım Yönetimi (Sharing Management)**

- Bilgisayar üzerindeki objeler (klasör, dosya, disk, yazıcı, uygulama vs.) paylaştırılabilirdir.
- Paylaşılan bilgisayar ve kullanıcılar, paylaştırılan objeyi izinler dahilinde kullanabilir.
- Paylaşımlar, SMB (Server Message Block) protokolü üzerinden sağlanırlar.
- Dosya paylaşım protokolü olan SMB; UDP 137-139 ve TCP 445 portlarında çalışır.
- SMB, iki adet ters slaş ( \\ ) ile ifade edilir.
- Paylaşılan objelere ve diğer bilgisayarlara 2 adet ters slaş ( \\ ) ile erişilebilir.

Örn; \\192.168.1.15\AbcKlasörü

- SMB (Server Message Block) protokülünün birden fazla versiyonu vardır.
- En yaygın kullanılan 2 tanesi şunlardır:

1) CIFS (Common Internet File System):
Windows ve SMB destekli diğer aygıtlar (NAS gibi) arasında kullanılır.

2) Samba:
Diğer işletim sistemlerinin Windows ile SMB bağlantısı kurabilmesi için kullanılır.

<h3> Regedit Nedir? </h3>

- İşletim sistemi, uygulama ve donanımların ayarlarını barındıran bir veritabanıdır.
- Bilgiler, ayarlar, seçenekler ve diğer değerleri içerir.
- İşletim sistemi ve bileşenleri, nasıl davranması gerektiğini buradan okur.
- Bu veritabanının dosyaları C:\Windows\System32\Config klasörü altında tutulur.
- Run (Çalıştır)’da veya CMD (Komut İstemcisi)’de Regedit yazılarak başlatılabilir.
- Değişiklikler kalıcı hasara yol oçabileceği için yedek (backup) alınarak çalışılması gerekir.
- Registry dosyaları .reg uzantılıdır.

Registry 5 bölümden oluşur.

1) HKEY_CLASSES_ROOT: Burada dosya türleri ve OLE (Object Linking and Embedding) bilgileri saklanır.
Dosya türleri için OLE kullanan uygulamalar, bilgileri buradan okur.

2) HKEY_CURRENT_USER: O an için oturum açmış kullanıcıya ait ayar ve seçenek bilgileri burada tutulur.

3) HKEY_LOCAL_MACHINE: Bilgisayara ait ayar ve seçenekler burada tutulur.

4) HKEY_USERS: Kullanıcıların geneline ait ayar ve seçenekler burada tutulur.

5) HKEY_CURRENT_CONFIG: O an için oturum açmış kullanıcıya özel donanım ayar ve seçenekleri burada tutulur.

Registry’de 2 tür veri tipi vardır:

1) Key (Anahtar): Değerleri barındıran ve çalıştıran ana konumlardır.
(Değerlerin klasörleri denebilir.)

2) Value (Değer): Değerlerdir. Key’lerin altında bulunurlar.
Üçe ayrılırlar.

a) String: Dizgi şeklindeki değerlerdir. Karakterlerden oluşur, metinseldir.

b) Binary: İkilik (Binary) gösterimli sayısal değerlerdir.

c) DWORD/QWORD Ondalık (decimal) ve onaltılık (hexadecimal) gösterimli değerlerdir.

DWORD, 32 bit’lik bir decimal veya hexadecimal değerdir.

QWORD, 64 bit’lik bir decimal veya hexadecimal değerdir.

Bir Registry dosyasının içeri şöyledir:

[Topluluk (Hive) Adı\Key Adı\Alt (Sub) Key Adı]

Değer (Value) Adı=Değer Tipi:Değer Verisi
