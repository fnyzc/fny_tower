# Icy Tower Karakter Seçimi - Oyun Analizi

## Genel Bilgi
"Icy Tower Karakter Seçimi" oyunu, klasik Icy Tower oyunundan esinlenilmiş bir tarayıcı tabanlı platform oyunudur. Oyuncunun amacı, seçtiği karakterle sürekli yukarı doğru zıplayarak platformlar arasında ilerlemek ve en yüksek skoru elde etmektir. Oyun, HTML5 Canvas ve JavaScript kullanılarak geliştirilmiştir ve görsel olarak çekici bir arayüze sahiptir. Oyuncular, farklı karakterler seçebilir, platformlar arasında hareket edebilir ve buff/debuff öğeleriyle oyun deneyimini zenginleştirebilir. Oyun, ana menü, karakter seçimi, ayarlar, yüksek skorlar ve nasıl oynanır ekranları gibi çeşitli kullanıcı arayüzü bileşenleri içerir. Arka plan müzikleri ve ses efektleri, oyun atmosferini desteklerken, yerel depolama (localStorage) kullanılarak yüksek skorlar kaydedilir.

Oyun, dinamik platform oluşturma, hareketli platformlar, tema değişiklikleri ve güçlendirici/zayıflatıcı öğeler gibi özelliklerle oyuncuya sürekli bir meydan okuma sunar. Skor, oyuncunun geçtiği platformlara ve topladığı buff'lara bağlı olarak artar. Tema değişiklikleri, skor ilerledikçe oyunun görsel stilini ve zorluk seviyesini değiştirir, böylece oyun monoton olmaktan çıkar.

## Nasıl Oynanır
Oyuna başlamak için ana menüden "Oyuna Başla" seçeneği tıklanır veya bir karakter seçildikten sonra oyun başlatılır. Oyuncu, yön tuşları (sol ve sağ ok tuşları veya A/D tuşları) ile karakterini yatay olarak hareket ettirir ve boşluk tuşu, yukarı ok tuşu veya W tuşu ile zıplar. Amaç, platformdan platforma zıplayarak yukarı doğru ilerlemek ve düşmeden mümkün olduğunca yüksek bir skora ulaşmaktır. Platformlar rastgele oluşturulur ve bazıları hareketlidir, bu da oyunu daha zor hale getirir. Oyuncu, duvarlara çarptığında otomatik olarak sıçrayabilir veya duvar kayması (wall sliding) yapabilir, bu da stratejik hareket imkanı sağlar.

Oyun sırasında, belirli platformlarda beliren buff'lar (örneğin, winter1, futuristic1, forest1, space1) toplanarak ek puan kazanılır. Ancak, debuff'lar (örneğin, ters kontroller) alındığında belirli bir süre boyunca kontroller tersine çevrilir, bu da oyuncunun dikkatini ve becerisini test eder. Oyun, oyuncunun ekranın altına düşmesiyle sona erer ve skor, yerel depolamada saklanarak yüksek skorlar listesine eklenir. Oyuncu, oyunu duraklatabilir (Escape tuşu ile) veya oyun bittiğinde yeniden oynayabilir ya da ana menüye dönebilir.

## Özellikler
- **Karakter Seçimi**: Oyuncular, dört farklı karakter (character1, character2, character3, character4) arasından seçim yapabilir. Her karakterin durma ve zıplama animasyonları için ayrı görselleri vardır, bu da oyuna görsel çeşitlilik katar.
- **Dinamik Platformlar**: Platformlar rastgele konumda ve boyutta oluşturulur. Bazı platformlar hareketlidir ve bu, oyuncunun reflekslerini zorlar.
- **Tema Değişiklikleri**: Skor ilerledikçe (300, 800, 1500 eşiklerinde) arka plan ve platform görselleri değişir, dört farklı tema (örneğin, winter, futuristic, forest, space) kullanılır.
- **Buff ve Debuff Sistemi**: Buff'lar (puan artırıcı öğeler) ve debuff'lar (ters kontroller gibi zorlaştırıcı etkiler) belirli aralıklarla platformlarda belirir, oyuna stratejik bir derinlik katar.
- **Ses ve Müzik Kontrolü**: Ayarlar menüsünden arka plan müziği ve ses efektleri açılıp kapatılabilir. Ses efektleri, zıplama ve buff toplama gibi olaylar için kullanılır.
- **Yüksek Skorlar**: Oyun, yerel depolama kullanarak en yüksek skoru ve son oynanan oyunların skorlarını kaydeder. Yüksek skorlar ekranında tarih ve puan bilgileri gösterilir.
- **Duraklatma ve Oyun Sonu Ekranları**: Oyun, Escape tuşu ile duraklatılabilir ve oyun bittiğinde skor, en yüksek skor ve yeni rekor bilgileri gösterilir.
- **Duvar Mekanikleri**: Oyuncu, duvarlara çarptığında otomatik sıçrama yapabilir veya kayabilir, bu da oyuna taktiksel bir boyut ekler.