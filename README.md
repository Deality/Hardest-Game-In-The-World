Hardest Game in the World
Hardest Game in the World, saf refleks ve yüksek odaklanma gerektiren, minimalist bir 2D "top-down" arcade oyunudur. Bu proje, oyun geliştirme sürecinde algoritmik döngülerin (loops) ve hareket yönetimi (movement management) mantığının mBlock platformu üzerinde kurgulanmasıyla tasarlanmıştır.

🧠 Oyun Mantığı ve Teknik Yapı
Oyunun temelinde, adının hakkını veren zorlayıcı bir döngü sistemi yatmaktadır. Teknik işleyiş mBlock’un blok tabanlı mantığı ile şu ana prensipler üzerine kuruludur:

Platform: Oyun, mBlock platformu üzerinde geliştirilmiştir. Bu sayede mantıksal akış şemaları (if-then-else, loop structures) görselleştirilerek optimize edilmiş bir oyun mekaniği oluşturulmuştur.

Oyuncu Denetimi: Oyuncu, ekranda bir "yuvarlak" (player circle) objesini yönetir. Kontroller, oyunun hızına yanıt verecek şekilde tanımlanmıştır.

Dinamik Engel Sistemi: Tuzaklar, "kare" (square) formunda tasarlanmış engellerdir. Bu kareler, mBlock'un döngü blokları kullanılarak aşağıdan yukarıya doğru sürekli bir loop içerisinde hareket ettirilir.

Döngüsel Akış (Infinite Loop): Karelerin hareketleri, sistem kaynaklarını verimli kullanacak şekilde kurgulanmıştır. Ekran sınırlarını aşan engellerin koordinatları, mBlock'un konum resetleme mantığı ile güncellenerek kesintisiz bir oyun akışı sağlanır.

Skor Mekaniği: Oyun alanı içerisinde beliren "minik yuvarlaklar", oyuncunun skorunu artırır. Bu etkileşim, "temas algılama" mantığı ile kontrol edilerek oyunun zorluk seviyesini zirveye taşır.

⚙️ Teknik Detaylar
Geliştirme sürecinde mBlock kullanarak yazılım mimarisini güçlendiren temel noktalar:

Mantıksal Akış: Karelerin aşağıdan yukarıya olan hareketi, repeat until ve forever döngüleri kullanılarak, sabit bir hız yönetimi ile sağlanmıştır.

Çarpışma Algılama: Yuvarlak oyuncu ve kare tuzaklar arasındaki etkileşim, mBlock'un "touching" (değdi mi?) sensör mantığı ile hata payı bırakmayacak şekilde işlenmiştir.

Performans Optimizasyonu: Nesne konumlarının güncellenmesi, blok tabanlı kodlamanın sınırları içerisinde en verimli algoritma ile kurgulanmıştır.
