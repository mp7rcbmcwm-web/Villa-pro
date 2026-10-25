SINAV YILDIZIM AI — YAYINLAMA PAKETİ

İÇERİK
- index.html: Sınav Yıldızım AI web uygulaması
- manifest.json: ana ekrana ekleme bilgileri
- sw.js: çevrimdışı temel uygulama kabuğu ve güncelleme önbelleği
- icon-180.png / icon-512.png / icon.svg: uygulama simgeleri
- SinavYildizim-Logo.svg: logo

YAYINLAMA
1. Paketin içindeki tüm dosyaları aynı klasör yapısını koruyarak HTTPS destekleyen hostinge yükleyin.
2. Uygulamayı Safari/Chrome üzerinden HTTPS adresinden açın. iPhone'da Safari > Paylaş > Ana Ekrana Ekle yolunu izleyin.
3. Eski uygulama sürümü takılı kalırsa sayfayı yeniden yükleyin; gerekirse ana ekran kısayolunu silip tekrar ekleyin.

GEMINI ÖZEL ÖĞRETMENİ (BYOK)
- Ayarlar > Yapay zekâ özel öğretmen alanına kişisel API anahtarınızı girin.
- Model seçin, anahtarı kaydedin ve “Bağlantıyı test et” düğmesiyle deneyin.
- Fotoğraf veya metin ile ilk ipucu isteyin. Öğrenci denemesini yazıp “Denememi değerlendir…” ile sonraki ipucunu alabilir; tam çözümü ayrı düğmeyle açabilir.
- Benzer soru üretimi de Gemini API ve internet gerektirir. Ücretsiz kota/model erişimi Google'ın güncel hesabı ve koşullarına bağlıdır. Bu uygulama sunucu üzerinden proxy kullanmaz; çağrılar tarayıcıdan doğrudan Google Gemini API'ye gider.
- API anahtarı yerel tarayıcı depolamasında saklanır; kaynak kodundan ve cihazdaki diğer erişimlerden tamamen gizlenmiş değildir. Paylaşılan cihazlarda anahtarı saklamayın, kullanımdan sonra silin.

OCR / ÇEVRİMDIŞI DURUMU
- Fotoğraf OCR'ı Tesseract.js ile tarayıcıda çalışır, Türkçe ve İngilizce için metin tanır; metindeki anahtar sözcüklerden ders ve konu tahmin eder.
- “OCR kaynaklarını hazırla” ilk yüklemede Tesseract.js ile dil verilerini indirip tarayıcı önbelleğine almaya çalışır. Bu pakette motorun tüm WASM/worker/dil dosyaları yerel olarak gömülü değildir. Dolayısıyla ilk kurulum için internet gerekir; daha sonra çevrimdışı çalışma, tarayıcı önbelleği ve iOS davranışına bağlıdır ve garanti edilmez. Gerçek, ilk açılışta da çevrimdışı OCR için Tesseract assetleri ayrı olarak aynı sunucudan paketlenmelidir.

DOĞRULAMA DURUMU
- JavaScript sözdizimi, manifest JSON ve paket yapısı kontrol edilir.
- Google API bağlantısı kişisel anahtar gerektirdiğinden bu ortamda gerçek uçtan uca test edilemez. Gerçek iPhone kamerası/mikrofonu ve çevrimdışı OCR bu ortamda fiziksel cihazda test edilmedi.


GÜNCELLEME — API ANAHTARI KAYDETME
Bu sürümde Ayarlar içindeki AI düğmelerinin olay bağlama hatası düzeltildi. Anahtar kaydetme işleminden sonra yerel depolamaya yazıldığı doğrulanır ve ekranda açık başarı/hata mesajı gösterilir. iPhone’da uygulamayı Safari üzerinden HTTPS adresinde açın; anahtarın gerçekten kaydedildiğini durum mesajıyla doğrulayın.
