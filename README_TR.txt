SınavYıldızım 2.0 — Faz 5–8 geliştirme paketi
==============================================

Yayınlama:
1. ZIP içindeki dosyaları birlikte bir klasöre çıkarın.
2. Klasör içeriğini HTTPS destekleyen bir statik hosting alanına yükleyin.
3. index.html, manifest.json, sw.js ve ikon dosyalarını aynı dizinde tutun.

Yeni modüller:
- Fotoğraflı soru kutusu: kamera/galeri seçimi, Canvas JPEG sıkıştırma, IndexedDB kayıtları
- Kural tabanlı haftalık çalışma programı
- Web Speech API ile sesli not (tarayıcı desteği/izinine bağlı)
- 3B dönen bilgi kartları
- Çalışma seanslarının saat dilimine göre süre özeti
- İki turlu deneme süre kaydı
- Yerel çoklu profil temeli
- Haftalık kodla soru/XP karşılaştırması
- Salt-okunur veli raporu HTML dosyası
- Uygulama rozeti ve Web Audio API ses efekti
- PWA kısayolları: Hızlı Deneme Gir ve Pomodoro Başlat
- IndexedDB'de fotoğraf depolama; diğer mevcut ilerleme verileri eski yerel kayıt yapısını korur

Sınırlar / test durumu:
- JavaScript sözdizimi Node.js ile kontrol edildi.
- Gerçek iPhone/Android cihaz, kamera izinleri, ses tanıma, Badging API ve canlı hosting üzerinde uçtan uca test yapılmadı.
- Profil sistemi bu cihazda yerel profil değiştirme için temel düzeydedir; profiller arası tam bağımsız hesaplar ve yetkilendirme için daha fazla geliştirme gerekir.
- Haftalık düello kodu güvenilir kimlik doğrulamalı bir sosyal sistem değildir; kodu alan kişi verileri değiştirebilir.
- Veli raporu indirilen andaki statik kopyadır, canlı takip bağlantısı değildir.
- Firebase veya başka bir bulut senkronizasyonu bu pakette etkin değildir.
- IndexedDB ve PWA özellikleri için uygulamayı HTTPS üzerinden yayınlayın; file:// üzerinden açmayın.
