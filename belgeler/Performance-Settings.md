# Windows Regedit Sistem Hızlandırma

1

Windows : Registry Editor Açın
Bilgisayar\HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Session Manager\Memory Management
LargeSystemCache = 1
DisablePageingExecutive = 1
Ram Sayınız x 1024 | Sonuç x 1024 | En Son Sonuç x 128
IoPageLockLimit = Çıkan Sonuç (Decimal Olacak) 8GB = 1078132 (Noktalar silinecek)

2

Bilgisayar\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer
32 BİTLİK DWORD DEĞERİ AÇIN
Name = AlwaysUnloadDll
Değer = 1

3

CPU'YA IRQ Sinyali göndericez bu sayede bileşenler CPU'ya daha hızlı istek göndericek
Not : İşlemci yorulmaz
32 BİTLİK DWORD DEĞERİ AÇIN
Name = IRQ8Priority
Değer = 1

4


Bilgisayar\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Dfrg\BootOptimizeFunction
String (Yazı dizisi değeri açın)
Name = BootOptimizeFunction
Değer = Y 
(Yes demektir sadece Y yazarsanız yeter.)

5

Şimdi Regeditte yapılmayacak
**Önemli : Eğer elektrik kesilmesi vb. Sorunlar yaşıyabiliyorsanız ve Önemli bir iş yürütüyorsanız açmayın! Aksi takdirde veri kaybına uğrarsınız. Eğer Laptop veya Sunucu kullanıyorsanız kesinlikle açın. Çok fazla performans kazandırır.**

Bilgisayar yönetimi Programını açın.
Solda depolamanın altında Disk Yönetimi var ona tıklayın.
hemen sağında diskleriniz gelir C: Diskinize sağ tıklayıp özelliklere gidin
İlkelere girin.  2 Kutucuğuda işaretleyin Normalde 1. Si Seçili geliyor zaten.

6

Eğer HDD Kullanıyorsanız bunu yapın SSD ise gerek yok

Sürücüleri birleştir ve iyileştire gidin (Windows aramada çıkar)
Kapalıysa kesinlikle açın %20lik bir performans artışı olacaktır.

7

Bilgisayar Özelliklerine girin
Gelişmiş Ayarlara girin
Performansa tıklayın
Performansın yanında gelişmiş var ona kafa atın
aşağıda Değiştir(Change) Butonu var ona tıklayın
üstte otomatik yönet açıksa kapatın
Aşağıdaki disk belleği dosyası yoku açın
Sonra yeniden başlatın

8

Bilgisayar ilk açılırkan işlemci yavaş yavaş açılır parçacıkları 1-2-3 diye devreye sokar
Bunu direkt fullicez.

Çalıştır > msconfig yazın
Boot'a gelin (önyükleme)
Kullandığınız işletim sistemini seçin (Sizde 1 adet olacaktır)
Gelişmiş Seçeneklere basın
İşlemci sayısını açın
ve en sona getirin ne kadar varsa kullan braha

9

Son olarak arkada CPU'yu Az kullanmanıza rağmen çok gitmesini önler
CMD'Yi açın
Rundll32.exe advapi.dll,processIdleTasks
Bu kodu  yazın
Yavaş yavaş CPU'nun rahatladığını göreceksiniz.

Not : *1 Olan değerler Decimal veya Hexdecimal farketmez.*
