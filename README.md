# OsiLayersAndAttacks

<img width="290" alt="image" src="https://github.com/Hamza-Limon/OsiLayersAndAttacks/assets/140405710/8a916693-33ed-4796-b790-b741ef55c837">

# OSI (Open Systems Interconnection)

- Osi modeli, bilgisayar ağlarını anlamak ve ağ iletişimi için gereken işlevleri ve protokolleri düzenlemek amacıyla oluşturulan bir referans modelidir. Bu model, ağ iletişimini yedi farklı katmana böler ve her katmanın belirli bir işlevi vardır. İşte OSI modelinin katmanlarını, en alttan en üste doğru sıralı olarak açıklayan bir özet:

### Fiziksel Katman (Physical Layer):

Bu katman, verilerin fiziksel ortamda nasıl iletilip alınacağını tanımlar.
Elektrik sinyalleri, optik sinyaller veya radyo dalgaları gibi fiziksel iletim araçları kullanılır.
Örnek cihazlar: Ethernet kablosu, ağ kartları.

### Veri Bağlantı Katmanı (Data Link Layer):

Bu katman, verilerin güvenli bir şekilde iletilmesini sağlar.
Hataları düzeltme, akış kontrolü ve MAC (Media Access Control) adreslemesi gibi işlevleri içerir.
Örnek cihazlar: Ethernet anahtarları, ağ kartları.

### Ağ Katmanı (Network Layer):

Bu katman, verilerin kaynak ve hedef arasındaki en uygun yol üzerinden iletilmesini sağlar.
IP adresleri kullanarak yönlendirme işlemini gerçekleştirir.
Örnek protokoller: IP (Internet Protocol), ICMP (Internet Control Message Protocol).

### Taşıma Katmanı (Transport Layer):

Bu katman, veri iletimini son noktaya ulaştırırken güvenilirlik ve akış kontrolü sağlar.
Verilerin bölünmesi, paketlerin numaralandırılması ve yeniden monte edilmesi gibi işlemleri içerir.
Örnek protokoller: TCP (Transmission Control Protocol), UDP (User Datagram Protocol).

### Oturum Katmanı (Session Layer):

Bu katman, veri iletimini başlatır, sürdürür ve sonlandırır.
Oturum kurma, sıra kontrolü ve veri senkronizasyonunu yönetir.
Örnek işlevler: Oturum başlatma, oturum sürdürme.

### Sunum Katmanı (Presentation Layer):

Bu katman, verilerin farklı formatlarda ve dillerde sunulmasını ve çevrilmesini sağlar.
Veri şifreleme, sıkıştırma ve veri dönüşümü gibi işlevleri içerir.
Örnek işlevler: Veri şifreleme, veri sıkıştırma.

### Uygulama Katmanı (Application Layer):

Bu katman, kullanıcıların ağ hizmetlerine erişimini sağlar.
Uygulama programları, veritabanları, e-posta istemcileri ve web tarayıcıları gibi kullanıcı uygulamaları burada bulunur.
Örnek protokoller: HTTP, FTP, SMTP.
Her katman, ağ iletişimi sürecinde belirli bir işlevi yerine getirir ve daha üst katmanlara hizmet sağlar. Aynı zamanda altındaki katmanlardan gelen veriyi alır, bu veriyi kendi katmanının protokolüne uygun şekilde işler ve üst katmana iletilmesini sağlar. Bu katmanlı yaklaşım, ağ iletişiminin daha iyi anlaşılmasına ve farklı ağ teknolojilerinin birlikte çalışabilmesine yardımcı olur.


- Her OSI model katmanında, siber saldırganlar tarafından farklı türde saldırılar gerçekleştirilebilir. İşte her katmanda karşılaşılabilecek potansiyel siber saldırılardan bazıları:

### Fiziksel Katman Saldırıları:

- Fiziksel Erişim (Physical Access): Saldırganlar, ağa fiziksel olarak erişim sağlayarak cihazlarına zarar verebilirler veya verileri çalabilirler.

### Veri Bağlantı Katmanı Saldırıları:

- MAC Spoofing: Saldırganlar, sahte MAC adresleri kullanarak ağa kaynak gibi görünmeye çalışabilirler.

- ARP Spoofing (ARP Zehirleme): Saldırganlar, ağda ARP tablosunu zehirleyerek hedef cihazların trafiklerini yönlendirebilirler.

### Ağ Katmanı Saldırıları:

- Denial of Service (DoS) Saldırıları: Saldırganlar, hedef cihazın IP adresine yoğun trafiği yönlendirerek hizmet kesintisi yaratabilirler.

- IP Spoofing: Saldırganlar, sahte IP adresleri kullanarak kimliklerini gizleyebilirler.

- Yönlendirme Saldırıları: Saldırganlar, yanlış yönlendirme bilgileri göndererek trafiği yanlış yerlere yönlendirebilirler.

### Taşıma Katmanı Saldırıları:

- TCP SYN Flooding: Saldırganlar, çok sayıda SYN isteği göndererek sunucuları aşırı yükleyebilirler.

- UDP Flooding: Saldırganlar, ağa büyük miktarda UDP trafik göndererek hizmetleri zehirleyebilirler.

### Oturum Katmanı Saldırıları:

- Session Hijacking: Saldırganlar, oturum kimlik bilgilerini ele geçirerek kullanıcı oturumlarını ele geçirebilirler.

- Man-in-the-Middle (MitM) Saldırıları: Saldırganlar, iletişim sürecinin ortasına girerek verileri izleyebilir veya değiştirebilirler.

### Sunum Katmanı Saldırıları:

- Payload Injection: Saldırganlar, kötü amaçlı kod veya veri enjekte ederek sunucu tarafında güvenlik açıklarını kullanabilirler.

- Cross-Site Scripting (XSS): Saldırganlar, kullanıcıların tarayıcılarında çalışacak kötü amaçlı kodları enjekte edebilirler.

### Uygulama Katmanı Saldırıları:

-SQL Injection: Saldırganlar, web uygulamalarına kötü amaçlı SQL sorguları enjekte ederek veritabanına erişebilirler.

-DDoS (Distributed Denial of Service): Saldırganlar, çok sayıda zombi cihazı kullanarak ağ hizmetlerini aşırı yükleyebilirler.

> Her katmanda karşılaşılabilecek siber saldırılar, ağ güvenliği uzmanları tarafından izlenmeli ve savunma önlemleri alınmalıdır. Ayrıca, katmanlar arası güvenlik önlemleri ve güçlü şifreleme gibi güvenlik uygulamaları da siber saldırılara karşı koruma sağlayabilir.
