# CMD FUNCTIONAL COMMANDS

**winsat formal : Sistemde stres testi yapar ve değerlendirir.**<br>

**powercfg /? : Bilgisayarın güç ile ilgili sorunlarına yardım eder.**<br>

**powercfg /energy : Enerji ile ilgili sorunları 60 saniye içerisinde gösterir.**<br>

**powercfg /hibernate, /h : Ram üzerindeki bilgileri hdd'ye kaydeder ve bir dahaki açılışta aynı kaldığı yerden devam eder.**<br>

**systeminfo : Bilgisayar ile ilgili tüm detayları görürüz.**<br>

**dx diag : Bilgisayar hakkında bilgi verir ve Gerçek/Sanal Makine olup olmadığını anlarız.**<br>

**mrt : Windows'un şüpheli uygulamaları bulup tespit etme programıdır.**<br>

**mmc : Kullandığınız programlar ile bir konsol oluşturursunuz.**<br>

**tasklist /v : Verbos komutudur detay verir.**<br>

**tasklist /svc : Çalışan servisleri gösterir.**<br>

**taskkill /f /im calculator.exe : Çalışan servisleri gösterir.**<br>

**ipconfig /release : IP Adresini bırakır.**<br>

**ipconfig /renew : DHCP IP Alma işlemini başlatır.**<br>

**ipconfig /flushdns : DNS Ön belleğini temizler.**<br>

**tracert 8.8.8.8 : IP Adresine giderken yolumuzu belirler.**<br>

**pathping 8.8.8.8 : Tracert komutunun daha iyisidir.**<br>

**net share : Paylaşılanları gösterir.**<br>

**netsh wlan show profile name="NetworkName" key=clear : Ağın Şifresini Gösterir.**<br>

**net share admin$ /d : paylaşılanlardan Admini siler (c veya d yazarsanız c yi siler) Fakat her bilgisayar açıldığında tekrar paylaşılır bat ile otomasyon yapabilirsiniz.**<br>

**telnet 8.8.8.8 53 : IP Adresinin portunu yoklayabilirsiniz. (Önce yüklemeniz gerekir : )**<br>
*Denetim Masası > Programlar > Programlar ve Özellikler > Windows Özellikerini aç veya kapat > Telnet İşlemcisini açın. > Tamam'a basıp indirin.*<br>
*Port açıksa ekran siyah kalır değilse "Connecting to 8.8.8.8..." Yazar*<br>

**attrib +s +h C:\Users\fazzt\Desktop\Accounts\ : Klasör veya dosyayı gizler**<br>
*-s -h yazarsanız gizliden görünür hale gelir*<br>

**dir /s /b /A:DH : Bulunduğunuz konumdaki gizli klasörleri gösterir Not: DH'ı Silerseniz direkt tüm gizli öğeleri gösterir**<br>

**dir /s /b /A:DH : Bulunduğunuz konumdaki gizli klasörleri gösterir Not: DH'ı Silerseniz direkt tüm gizli öğeleri gösterir**<br>

**fsutil file createnew text.txt 30000 : 30 KB'lik içi boş bir TXT Dosyası oluşturur.**<br>

<hr>

nslookup.exe:Gerçek bağlantı kurduğunuz yerin IP adresini bulun.

shrpubw.exe:Paylaşılan klasör oluşturmak için.

syskey.exe:Windows şifreleme (not şifreyi bir kez girerseniz bir daha devre dışı bırakamazsınız)

C:\\WINDOWS\\system32\\tsshutdn.exe:Sistemi 60 saniyede kapatır.

C:\\WINDOWS\\system32\\webfldrs:Sistemdeki diyalogları siler kurar.

C:\\WINDOWS\\system32\\attrib.exe:Sistemdeki .dll .exe .inf vs. uzantılı

dosyaları listeler.

netstat -n: Adresleri ve Bağlantı Noktalarının Numaralarını Sayısal Biçimde Gösterir
netstat -an: Dosya Alırken Karşıdakinin IP adresini Gösterir.

netstat -a: Tüm Bağlantıları ve Dinleme Bağlantı Noktalarını Gösterir.

netstat -b: Her Bağlantı veya Dinleme Bağlantı Noktası İle İlişkili Çalıştırılabilir Dosyayı Gösterir.

netstat -e: Ethernet İstatistiklerini Gösterir.

netstat -o: Her Bağlantıyla İlişkili Sahip İşlem Kimliğini Gösterir.

netstat -p: İletişim Kuralının Bağlantılarını Gösterir.

netstat -r: Yönlendirme Tablosunu Gösterir.

netstat -s: her İletişim Kuralları İçin İstatistikleri Gösterir.

compmgmt.msc - Bilgisyar Yöneticisi

devmgmt.msc - Aygıt Yöneticisi

diskmgmt.msc - Disk Yöneticisi

dfrg.msc - Disk birleştirme

eventvwr.msc - Olay Görüntülüyicisi

fsmgmt.msc - Paylasilan Dosyalar

gpedit.msc - Grup Poliçeleri

lusrmgr.msc - Yerel Kullanicilar ve Gruplar

perfmon.msc - Performans Monitörü

rsop.msc - Poliçe Sonuçarini Ortaya koymak

secpol.msc - Yerel Güvenlik Ayarlari

services.msc - Çesitli Servisler

msconfig - Sytem Bilgisi Hizmetleri

regedit - - Kayit Defteri Editörü

msinfo32 - Sistem bilgisi

sysedit - Sistem sekli Editörü

win.ini - Windows Yükleme Bilgisi

winver - su anki Windows Sürümünü Görüntüle
alicisi Görüntüle

cmd - Komut satirini çalistir

Program Ekle Kaldir / control appwiz.cpl

Tarih Saat özellikleri /control timedate.cpl

Ekran özellikleri / control desk.cpl

Hizli bul / control findfast.cpl

Fontlar / control fonts

Internet Özellikleri /control inetcpl.cpl

Klavye özellikleri /control main.cpl keyboard

Mouse Özellikleri / control main.cpl

Multimedya Özellikler /control mmsys.cpl

Ag Özellikleri / control netcpl.cpl

Şifre özellikleri / control password.cpl

Printer /control printers

Ses Özellikleri / control mmsys.cpl sounds

Sistem Özellikleri /control sysdm.cpl

ing ip ===> ip deki diger bilgisayara ufak veri paketleri gönderip, alarak baglantiyi test eder

ping -a -n ip ===> -n parametresinin yanindaki deger kadar veri paketleri gönderilirilerek test edilir.

pathping ===> bu komut sayesinde routerlar üzeriden geçen verinin kayba uğayıp uğamadığı kontrol edilir.

ipconfig ===> bilgisayarin agdaki ip adresini gösterir.

ipconfig /all ===> bilgisayarin agdaki ip adresini ve bir çok ekstrayi gösterir.

ipconfig /all >egemen.txt ===> dökülen tüm bilgiyi egemen.txt dosyası içine atar.

ipconfig /release ===> bilgisayarin agdaki ipsini birakir

ipconfig /renew ===> bilgisayarin agdaki ipsini yeniler. yenileme islemi sirasinda ilk önce ?release? , sonra ?renew? islemi uygulanir

ipconfig /registerdns ===> bilgisayarı adını ve ipsini DNS e kaydetmek için kullanılır.

ipconfig /flushdns ===> Dns clientların cache belleklerinde tuttukları isim ve ip adres eşleşmelerine ait bilgileri siler,Cache belleği boşaltır.(Sorun Çözmek için kullanılır)

ipconfig /displaydns ===> Eğer kullandığınız bilgisayar aynı zamanda bir DNS clientâ?ı ise, DNS Cache belleğinde bulunan IP adresleri ve onlara ait olan DNS isimlerinin gösterilmesini sağlar.

arp -a ===> cache deki ip çözümlesini gösterir. cache eger 2 dk içinde yeni bir ip çözümlemesi olmazsa kendini temizler. eger 2 dk içinde yenilenirse 10 dk daha tutulur.

arp -s 192.168.0.2 00-02-44-12-24-ad ===> ip çözümlemesi içinde, ip si verilen bilgisayarin ?mac? adresini sabitler. cache de sürekli kalir, silinmez


net use ===> bilgisayardaki map leri gösterir.

net use h: \\\\client98\\c ===> client 98 bilgisayarin C sini H olarak map eder.

net use h: \\\\192.168.0.2\\c$ ===> ipsi verilen bilgisayarin gizli admin sharini h olarak map eder.

net use /delete h: ===> h mapped drive i siler.

net use lpt1: \\\\server\\ibm /persistent ===> kalıcı printer bağlantısı sağlar.

netstat ===> bilgisayara yapilan baglantilari gösterir.

nbtstat ===> TCP/IP üzerinde NetBIOS API ile ilgili verilerin gösterilmesini sağlar.Netbios isim tablosunun hem kullandığınız(local) bilgisayar için hemde network üstündeki diğer bilgisayarlar(remote) için gösterilmesini sağlar.

<hr>

calc.exe Hesap makinesini açar.

diskmgmt.msc Disk yönetimini açar.

devmgmt.msc Aygıt yöneticisini açar.

dfrg.msc Disk birleştiriciyi açar.

eudcedit.exe Karakter imal edebilirsiniz.

appwiz.cpl Program ekle kaldırı açar.

access.cpl Erişebilirlik seçeneklerini açar.

accwiz.exe Erişebilirlik sihirbazını açar.

desk.cpl Görüntü özelliklerini açar.

eventvwr.exe Olay görüntüleyicisini açar.

freecell.exe İskambil oyununu açar.

fsmgmt.msc Paylaşılan klasörler menüsünü açar.

hdwwiz.cpl Donanım ekleme sihirbazını açar.

iexpress.exe Setup programını açar.

inetcpl.cpl İnternet özelliklerini açar.

intl.cpl Bölge ve dil ayarlarını açar.

joy.cpl Oyun kontrollerini açar.

magnify.exe Büyüteçi açar.

main.cpl Fare özelliklerini açar.

mmsys.cpl Ses ayarlarını açar.

mspaint.exe Paint programını açar.

narrator.exe İngilizce ekran okuyucusunu açar.

ntbackup.exe Yedekleme sihirbazını açar.

nusrmgr.cpl Kullanıcı hesaplarını açar.

osk.exe Ekran klavyesi açar.

telnet.exe Telnet'i açar.

spider.exe Kağıt oyunu açar.

gpedit.msc Grup poliçesi açar.

msconfig.exe Sistem ayarlarını açar.

verifier.exe Sürücü monitörünü açar.

drwtsn32.exe Sorun tanıma aracını açar.

dxdiag.exe DirectX sürümünüzü öğrenmenizi sağlar.

mobsync.exe Senkronizasyon sağlar.

mplay32.exe Media Player'ın çok basit bir halini açar.

odbcad32.exe Database işleme sağlar.

packager.exe Obje paketleyiciyi açar.

perfmon.exe Sistem monitörünü açar.

progman.exe Masaüstü yöneticisini açar.

rasphone.exe Erişim defterini açar.

shrpubw.exe Network paylaşımı bilgisini açar.

sigverif.exe İmza denetleyicisini açar.

sysedit.exe Sistem yöneticisini açar.

syskey.exe Şifre databaseni açar.

sndrec32.exe Ses kaydedicisini açar.

timedate.cpl Tarih ayarlama penceresini açar.

tourstart.exe Windows XP turu başlatır.

winchat.exe Windows içinde bulunan chat programını açar.

winmine.exe Mayın Tarlası oyununu açar.

write.exe WordPad'i açar.

wupdmgr.exe Windows güncelleştirme penceresini açar.

explorer.exe Windows Gezgini?ni açar.

powercfg.cpl Güç seçeneklerini açar.

rasphone.exe Ağ bağlantılarını açar.

regedt32.exe Windows Kayıt Düzenleyicisi'ni açar.

regedit.exe Windows Kayıt Düzenleyicisi'ni açar.

sndvol32.exe Ses ayarlarını yapmanızı sağlar.

notepad.exe Not defterini açar.

taskmgr.exe Görev yöneticisini açar

compmgmt.msc Bilgisayar yönetimini açar.

clipbrd.exe Pano işlemcisini açar.

cleanmgr.exe Disk temizleyiciyi açar.

ciadv.msc Dizin yöneticisini açar.

charmap.exe Karakterleri ayarlamanızı sağlar

appwiz.cpl....Add/Remove Programs

desk.cpl......Display Properties

hdwwiz.cpl....Add Hardware Control Panel Applet

inetcpl.cpl...Internet Control Panel

main.cpl......Mouse Properties

mmsys.cpl.....Sound and Audio

powercfg.cpl..Power Options

sysdm.cpl.....System Properties

timedate.cpl..Time and Date Properties

wuaucpl.cpl...Automatic Updates Control Panel

<hr>

**Append : Append komutu, programlar tarafından başka bir dizindeki dosyaları geçerli dizinde bulunuyormuş gibi açmak için kullanılabilir. Append komutu, MS-DOS'ta ve Windows'un tüm 32 bit sürümlerinde kullanılabilir. Append komutu, Windows'un 64 bit sürümlerinde kullanılamaz.**

**Arp : arp komutu, ARP önbelleğindeki girdileri görüntülemek veya değiştirmek için kullanılır. arp komutu Windows'un tüm sürümlerinde kullanılabilir.**

**Assoc : assoc komutu, belirli bir dosya uzantısıyla ilişkili dosya türünü görüntülemek veya değiştirmek için kullanılır. İlişkili komut Windows 10, Windows 8, Windows 7, Windows Vista ve Windows XP'de kullanılabilir.**

**At : at komutu, komutları ve diğer programları belirli bir tarih ve saatte çalışacak şekilde zamanlamak için kullanılır. at komutu Windows 7, Windows Vista ve Windows XP'de kullanılabilir. Windows 8'den başlayarak, komut satırı görev zamanlaması bunun yerine schtasks komutuyla tamamlanmalıdır.**

**Atmadm : Atmadm komutu, sistemdeki zaman uyumsuz aktarım modu (ATM) bağlantılarıyla ilgili bilgileri görüntülemek için kullanılır. Atmadm komutu Windows XP'de kullanılabilir. ATM desteği, Windows Vista'dan itibaren kaldırılarak atmadm komutu gereksiz hale getirildi.**

**Attrib : Attrib komutu, tek bir dosyanın veya dizinin özniteliklerini değiştirmek için kullanılır. Attrib komutu, Windows'un tüm sürümlerinde ve MS-DOS'ta kullanılabilir.**
