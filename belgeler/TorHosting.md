# Fazz | Tor Web Hosting

**Kali Linux Üzerinden Apache Kullanacağız.**

**Apache Download : apt install apache2 -y**

*Durumu Görmek : systemctl status apache2*

*Başlatmak : systemctl start apache2*

*Sistem başladığında Apache'de başlar : systemctl enable apache2*

*Apache Web Dosya Yolu : var/www/html/*

Ngrok ile 80 Portuna yönlendirmek;

**ngrok http 80** kodu ile localhostumuza direkt yönlendirme sağlanacaktır.

Not : Ağı Kali'de bridged moda alın.

Şimdi modem arayüzüne girmeliyiz. (Varsayılan ip:192.168.1.1)

Genel Ağ > Port Yönlendirme > Lan yöneticisine Kali'nin ip adresini yazın. > Wan Port'u 80 - 80 yapın. (Lan yönetici portu da aynı şekil.)

Artık dış ip adresimizi web'e yazınca localhostumuza yönlendirilecektir.

<h2> Tor Browser </h2>

**TOR (The Onion Routing)**, iletişimde anonimlik sağlamak amacıyla geliştirilmiş bir projedir.

Projenin,

İlk fazında;1995’te ABD Deniz Harp Araştırma Laboratuvarı çalışanları Paul Syverson, Michael Reed
ve David Goldschlag tarafından geliştirilmiştir. ABD gizli servislerinin çevrimiçi istihbarat iletişimini
koruma amacı hedeflenmekteydi.

İkinci fazında; 2002’de, geliştirilmesi MIT (Massachusetts Institute of Technology) tarafından üstlenildi.
Gizliliğin ve geliştiriciliğinin artırılması için halkın da katılımı fikriyle halka açımı gerçekleştirildi. TOR,
ABD Deniz Harp Araştırma Laboratuvarı’ndan ayrıldı, açık kaynak haline getirildi.

Üçüncü fazında; açık kaynak haline getirilince EEF (The Electronic Frontier Foundation) tarafından
devralındı. Gizlilik endişelerinden dolayı askeri intibatının yok edilmesi için çalışmalar yaptı.

Günümüze gelene kadar birçok ödül aldı… (%100 güvenlik olmadığı gibi %100 gizlilik de yoktur.)

<img src="https://github.com/FazzPy/Regedit-CMD/blob/main/belgeler/img/tor.jpg">

**Tor Browser Kurulumu : apt install torbrowser-launcher -y**

*Not: .local dizininin içinde start-tor-browser içindeki root kodunun silinmesi gerekiyor. (if ile fi arası yorum satırına alınabilir.)*

<h2> TOR Web Hosting </h3>

Not : Eğer bir web sunucusu vs. yapıyorsanız ip adresini statik verin.

**nano /etc/apache2/ports.conf** > Listen 80'i Listen local IP:80 (Örnek: Listen 192.168.1.36:80)

service apache restart yazın.

Not: Kali'yi Tor ağına bağlamalıyız Örnek: Torghost veya Anonsurf kullanabilirsiniz.

**nano /etc/tor/torrc** > HiddenServiceDir ve Port'u yorum satırından çıkartın. (Dir'i html dosyalarının olduğu yapın ve ip'yi local ip olarak ayarlayın.)

<h3> Web Sayfasını Onion uzantılı olarak yayınlama </h3>

1) Eğer anonsurf çalışıyorsa stop yaparak kapayın.
2) **tor** yazarak tor servisini başlatın.
3) Eğer ki config dosyaları düzgün ise html dosyalarımızın yanına onion uzantımız gelecektir.
4) Arkada tor servisimiz çalıştığı sürece sitemiz tor'da yayınlanmış olacaktır.

**tail -100 /var/log/apache2/access.log** ile ziyaretçi ip adreslerini ve logları görebilirsiniz.
