# MyWardrobe 1.0

Krem/beyaz/siyah temalı, Türkçe, çevrimdışı çalışabilen kişisel gardırop PWA'sı.

## Özellikler
- Fotoğraflı kıyafet ve aksesuar kataloğu (kategori, marka, renk, beden, mevsim, notlar, favoriler)
- Arama, kategori filtreleme ve sıralama
- Çoklu kıyafet seçerek kombin kaydetme
- Kombin takvimi
- Fotoğrafları da içeren JSON yedekleme / geri yükleme
- IndexedDB ile cihazda yerel saklama; fotoğraflar en fazla 1200 px ve JPEG olarak sıkıştırılır
- Service Worker ile çevrimdışı açılış

## Bilgisayarda test
Bu klasörde `python3 -m http.server 8000` çalıştırın; tarayıcıda `http://localhost:8000` adresini açın. localhost service worker için güvenli bağlam kabul edilir.

## iPhone'a kurulum
1. Klasörü HTTPS destekli statik barındırmaya (ör. GitHub Pages / Cloudflare Pages) yayınlayın. Sadece ZIP dosyasını telefona indirmek PWA kurulumu için yeterli değildir.
2. Safari ile HTTPS adresini açın, sayfanın tam yüklendiğinden emin olun.
3. Paylaş > Ana Ekrana Ekle seçeneğini kullanın.
4. Bir kez çevrimiçiyken açın; sonra uçak modunda test edin.

## Gizlilik ve veri güvenliği
Tüm kullanıcı kayıtları tarayıcı IndexedDB veritabanındadır, sunucuya yüklenmez. Tarayıcı veya site verileri silinirse kayıtlar kaybolabilir. Ayarlar > Gardırobu yedekle ile düzenli JSON yedeği alın; bu dosya fotoğrafları da içerir ve özel tutulmalıdır. Başka cihazlarla otomatik senkronizasyon yoktur. iOS depolama kotaları ve sistem temizliği davranışları değişebilir.

## Kapsam
Sanal yapay zekâ prova, otomatik fotoğraf arka plan temizleme, hesap ve bulut senkronizasyonu bu sürümde yoktur.
