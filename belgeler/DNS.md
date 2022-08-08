# Fazz | DNS Notes

<h3>DNS Resource Records (RR)</h3>

* **SAO (Start of Authority) : Bulunduğu zone’da yetkili sunucunun kim olduğunu belirtir.**
* **NS (Name Server) : Domaindeki DNS sunucularını belirtir.**
* **A (ya da Host) : Host’ların IP bilgilerini belirtir. Host adlarını IP’lere eşler.**
* **CNAME (ya da Alias) : Comminical Name... A kaydı bulunan bir host için birden fazla kayıt girilebilmesini sağlar.**
* **PTR (Pointer) : A kaydının tersini yapar. IP’leri Host adlarına eşler. Ters görünür. FQDN’leri IP dizilimine uydurmak için kullanılır.**
* **MX (Mail Exchanger) : Domain’deki mail sunucularını belirtir. Birden fazla mail sunucusu varsa, priority vererek öncelik belirleyebilir.**
* **SRV (Service) : Domain’in DC’lerini belirtir. Kaydında LDAP ve Kerberos bilgilerini de tutar.**

<h3>DNS Zone Türleri </h3>

1) Primary Zone : Okunabilir ve yazılabilir kayıtlar buradadır. Birincil zone’dur.
2) Secondary Zone : Sadece okunabilir kayıtları tutar. Hata anında Primary Zone için yedeklilik sağlar.
3) Stub Zone: En çok arandan kayıtları tutar. Diğer zone’lar için yük üstlenme sağlar. Bulunamayan kayıtlar için diğer zone’lara bakılmasını belirtir.

<h3>DNS’in Seçilebilir Gelişmiş Özellikleri</h3>

1) Recursion: DNS Server’ın diğer DNS sunuculara sorgu atabilmesidir.
2) BIND Secondary: Zone’ların diğer DNS sunuculara taşınabilmesidir.
3) Fail on Load: Zone’lardaki verilerin hatalarının, algılanıp kullanılmalarını sağlamaktır.
4) Round Robin: Birden fazla A kaydı olan sunucular için yük dengelemedir.
5) Netmask Ordering: Sorgu gönderinin network’üne uygun cevabın dönülmesidir.
6) Cache Pollution: Önbelleğin kirlenmesini önlem amacıyla belirli sürelerde temizlenmesidir.

<h3>DNS için Unutulmaması Gerekenler</h3>

- Hosts dosyası sadece A ve PTR kaydı için kullanılabilir.
- DNS sadece UDP 53’ten çalışmaz. UDP datagramı uyumsuzluğunda TCP 53’ten çalışır.
Firewall’da TCP 53’ü de açmayı unutma!
- Client (Resolver)’ın cache durumunu hatırla; ipconfig /flushdns kullanmayı unutma.
- Reverse Lookup Zone’u aktif edip PTR kayıtları da tutmayı unutma.
- DNS kayıtlarında sadece A-Z, a-z, 0-9 ve – kullanılabiceğini unutma.
- Forwarder DNS sunuculara başvurma süresini kısalt. 1 veya 2 saniye idealdir.
- TTL değerinin, Client (Resolver)’ın cache’i için bir sorgunun yaşam süresi olduğunu unutma.
- Aging/Scavenging yaşlanan Resource Records’ların silinmesi işlemidir. Bu RR’lara ‘’Stale Records’’ denir.
- dcdiag DC ve DNS server için teşhis bilgileri toplar. İşler yolunda gitmediğinde kullan.
