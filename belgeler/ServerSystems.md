# Fazz | Sunucu Sistemleri

<h3>Sunucular (Servers)</h3>

- Donanımsal ve yazılımsal olarak anılırlar.
- Birden fazla işlemi en az sürede yapabilmek için performans odaklı donanım ve işletim sistemleridir.
- Mimarileri, işlemler sırasındaki darboğazı (bottleneck) en aza indirgemek ve yüksek erişirlik amaçlıdır.
- Rack-Mount, Tower, Blade gibi boyutsal türleri vardır.
- Isı, sıvı ve nem değerleri kontrollü ortamlarda, kabinetler içerisinde tutulurlar.
- Yüksekliklerinden U (Unit) olarak bahsedilir. 1U, 2U, 4U, 12U gibi. 1U=4.4 cm’dir.

Boyut Tipleri:

Rack-Mount:

- Yatay tiplidir; kabinetlerin içine yatay olarak konulurlar.
- Genelikle 2U olurlar. 1U olanları da vardır.

Tower:

- Dikey tiplidir; kabinetlere uygun değildir.
- Rack tipi sunucular kadar verimli ve güvenli değillerdir.

Blade:

- Birden fazla sunucunun bir şaşede görev yaptığı sunucudur.
- Performans ve depolama odaklı kullanılırlar.
- Genellikle 10U olurlar.

Parçalar:

1 HDD’ler 2 Ön LED’ler 3 Disk Slotları 4 Kapasitör 5 Fanlar 6 Anakart 7 İşlemci ve soğutucusu 8 Batarya/Pil 9 Dahili USB Sürücüsü
10 Hava Bölmesi
11 Üst Kapak
12 Dahili M2 SSD Sürücü
13 PCI-E Kart
14 RAID Kontrolcüsü
15 PCI-E Kart
16 PCI-E Kart
17 PCI-E Basamakları

<h3>Kabinetler (Cabinets)</h3>

- Minimum alana maksimum sunucu sığdırma amaçlı dolaplardır.
- Sunucular için güvenli ve düzenli alan sağlarlar.
- Üzerilerinde ısı, sıvı, nem sensörleri; soğutma fanları; elektrik prizleri ve kilitler mevcuttur.
- Çalışma ergonomisi için sunucu kızakları ve hareket için altında tekerlekleri mevcuttur.
- Yükseklikleri U (Unit) birimiyle adlandırılır. Yükseklikleri 4U ila 48U arasında değişir.
- Network cihazları için duvar tipi olanları da vardır. Genellikle 4U’dur.

Kabinet Parçaları:

Güç Dağıtım Birimi
Power Distribution Unit (PDU)

Fan Kontrolcüsü
Fan Controller

Sunucu Kızağı
Slider / Rail

Kablo Düzenleyici
Cable Organizer

<h3>Çok İşlemcili Sunucular</h3>

**(Multiprocessor Servers)**

- İçinde 1’den fazla CPU olabilen sunuculardır.
- Model numarası içinde veya ilişiğinde veya özelliklerinde ‘P’ harfiyle temsil edilirler. Örn; 4P.
- Bu sunucularda iş yükünün paylaşımında 2 metot vardır.
1) Asymmetric Multiprocessing (AMP)
2) Symmetric Multiprocessing (SMP)

1) Asymmetric Multiprocessing (AMP):
- Her görevin, işlemin, uygulamanın kendine özel ayrı CPU’su vardır.
- Her durumda verimli olmayabilir.
- CPU çoklamak fayda etmeyebilir.

2) Symmetric Multiprocessing (SMP)
- Her görev, işlem, uygulama; boşta olan herhangi bir CPU’da işlenebilir.
- Her durumda yük dengelemesi sağlanabilir.
- CPU çoklamak fayda eder.

- Verilen işler birden fazla CPU’da işlendiği için RAM kullanımının 2 metodu vardır.

1) Tightly Coupled (Sıkı Bağımlı):
- Tüm bellekler ortak kullanılır.
- Belleklerde meydana gelen sorun tüm CPU’ları etkiler.

2) Loosely Coupled (Gevşek Bağımlı):
- Bellekler bölüştürülmüştür. Her CPU’nun ayrı bellek grubu vardır.
- Kendi belleklerini diğer CPU’lar ile paylaşmazlar.
- Her CPU kendi arasında ortaklaşa çalışabilir.
- Eklenen her CPU’ya ayrı RAM de eklemek gerekir; bu yüzden maliyetlidir.

<h3>x86 ve x64 Kavramları<h3>
  
  **x86 (32-bit)**
 
- 32 bitlik sayılar için bir kısaltmadır.
- Bu sayı 0 ve 1’lerden oluşur ve binary dizimi olarak adlandırılır. Örn; 01101110…
- 32 bitte, sayı 1 ve 0’lardan oluşacağı için toplam kombinasyon adedi 2^32 kadardır.
- 2^32=4,294.967.296 farklı kombinasyon eder.
- 32 bit bellek adresyebilen bir işlemci, 4,294.967.296 bitlik bellek alanı işleyebilir.
- Her 8 bit’e, 1 byte adreslenebildiği için, bu da 32-bit işlemcinin maksimum 4 GB veri adresleyebildiği anlamına gelir.
- 32 bit’lik işletim sistemleri bu yüzden en fazla 4GB RAM destekler. Fazla fiziksel RAM’inizin olması, durumu değiştirmez.
- İşlemci, işlem parçalarını en fazla 32’şer bitler halinde işleyebildiği için, 64 bit’lik işlemciye göre yavaştır.
- PAE (Physical Addressing Extensions) teknolojisi ile Windows’ta görünen 3~ GB RAM kullanımı, 4 GB’a çıkarılabilir.
  
  **Neden x32 değil de; x86 ?**
  
- Intel’in en başarılı, ilk göz ağrı olan işlemcilerinin mimarisidir.
- Intel’in ilk işlemcilerinin son 2 rakamı daima 86 ile biterdi.
- 1980 ve 1990’lar arasında çıkan i286, i386, i486 gibi.
- Bu işletim sistemlerinin hepsi 32 bit’lik mimarideydi.
- Bu yüzden 32 bitlik mimarinin adı, bu eski işlemcilere atıfta bulunarak terminolojiye x86 olarak geçti.
- x86 teriminin isim babası Intel’dir.

**x64 (64-bit)**
  
- 1 ve 0’ların 32 bit mimaride en fazla 2^32 kadar kombinasyonu olduğu gibi, 64 bit için de bu sayı, 2^64’tür.
- Bu sayı (16 EB) günümüz ve yakın gelecek için çok fazla olduğu için şimdilik 2^48 ile sınırlandırılmıştır.
- 2^48 bitlik bir işlemci 256 TB veri adresleyebilir.
- PAE (Physical Addressing Extensions) teknolojisi ile bu adres alanı 2^64’e çıkarılabilir. Fakat teoridedir…
- İşlemci, işlem parçalarını 64’er bitler halinde işleyebildiği için, 32 bit’lik işlemciye göre daha hızlıdır.
- 64 bit’lik veri adreslenebilmesi (işlenebilmesi) için, işletim sistemi ve uygulamaların da x64’ü desteklemesi gerekir.
- x64 işlemciler ve işletim sistemleri x86 uyumludur; 32 bit’lik adresleme yapabilirler.
- Bu sebeple işletim sistemlerinin içinde uygulamalar için Program Files ve Program Files (x86) vardır.
- 32 bit mimaride çalışan uygulamalar Program Files (x86) klasörünü kullanırlar; DLL’lerini buraya bırakırlar.
  
  
  
