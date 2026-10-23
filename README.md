# 🏡 ARCHI-VILLA PRO v2.0 — 2D CAD & 3D BIM Mimari Tasarım Stüdyosu

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-emerald.svg)
![Tech](https://img.shields.io/badge/Three.js-r128-black.svg)
![UI](https://img.shields.io/badge/TailwindCSS-CDN-38bdf8.svg)

**ARCHI-VILLA PRO**, herhangi bir kurulum veya sunucu gerektirmeden doğrudan tarayıcı üzerinde çalışan, **2D Teknik Mimari Plan (Retina CAD)** ve **Gerçek Zamanlı 3D Görselleştirme (Three.js BIM)** özelliklerini birleştiren tek dosyalı (Single-File) modern villa ve malikane tasarım yazılımıdır.

---

## ✨ Öne Çıkan Özellikler

* **📐 Çift Ekranlı Senkronize Mimari Motor:** Sol ekranda 1 kare = 1 metre ölçekli 2D CAD planı çizerken, sağ ekranda tüm yapı elemanları eşzamanlı olarak 3 boyutlu modele dönüştürülür.
* **🧱 İçi Boş 4 Duvarlı Oda & Otomatik Boşluk (CSG/Interval) Motoru:** Odalar içi boş 4 duvarlı hacimler olarak oluşturulur. Duvar üzerine yerleştirilen **cam cephe**, **kapı** ve **pencereler** otomatik algılanarak duvarlarda gerçek boşluklar açılır.
* **🛋️ İç Mekan Kesit Modu ve Tefrişat Kütüphanesi:** Tek tıkla çatıyı gizleyerek (`🔍 İç Mekan Kesiti`) odaların içindeki kanepe, yatak, yemek masası, dolap ve bitki yerleşimlerini 3 boyutlu inceleyebilirsiniz.
* **🏢 Çok Katlı Tasarım (Zemin, 1. Kat, Çatı/Teras):** Üst katları çizerken alt katın duvar izlerini (hayalet/referans plan) 2D ekranda görerek kusursuz aks hizalaması yapabilirsiniz.
* **☀️ Atmosferik Işıklandırma ve Gölgeler:** Gündüz (`☀️`), Gün Batımı (`🌅`) ve Gece (`🌙`) modları ile havuz içi LED aydınlatmaları ve iç mekan sıcak mimari ışıklarını gerçek zamanlı test edebilirsiniz.
* **📊 Otomatik Metraj & Dışa Aktarma:** Kapalı alan ($m^2$), havuz alanı ($m^2$), teras/deck ($m^2$), cam cephe ($m$), duvar uzunluğu ($m$) ve kapı/pencere sayılarını otomatik hesaplar.
  * **📄 PDF Metraj Raporu:** Proje özetini ve kat bazlı eleman listesini PDF olarak indirir.
  * **📸 3D PNG Render:** 3 boyutlu sahnenin anlık yüksek çözünürlüklü ekran görüntüsünü PNG olarak kaydeder.
  * **💾 JSON Proje Kayıt / Yükleme:** Projelerinizi `.json` formatında bilgisayarınıza kaydedip daha sonra tekrar yükleyebilirsiniz.
* **📱 Tam Mobil ve Tablet Uyumu:** `Pointer Events` altyapısı ve duyarlı sekme yapısı ile hem masaüstünde hem de dokunmatik ekranlarda (iOS / Android) sorunsuz çalışır.

---

## 🚀 Canlı Demo (GitHub Pages Kurulumu)

Bu projeyi GitHub üzerinde ücretsiz olarak yayınlamak için:

1. Bu depoyu (repository) kendi GitHub hesabınıza yükleyin (`index.html` ana dizinde olmalıdır).
2. GitHub deponuzda **Settings (Ayarlar) > Pages** sekmesine gidin.
3. **Source (Kaynak)** kısmından `Deploy from a branch` seçin ve dal olarak `main` (veya `master`) `/ (root)` seçip **Save** butonuna tıklayın.
4. Birkaç saniye içinde projeniz `https://<kullanici-adiniz>.github.io/<repo-adi>/` adresinde yayına girecektir.

---

## 🎮 Kontroller ve Kullanım

| Alan | İşlem | Kontrol |
| :--- | :--- | :--- |
| **2D CAD Planı** | Duvar / Oda / Havuz / Teras Çizimi | Sol Tık (veya Dokun) + Sürükle Bırak |
| **2D CAD Planı** | Kolon / Mobilya / Kapı / Pencere | Aracı Seç + Planda İlgili Noktaya Tıkla |
| **2D CAD Planı** | Eleman Düzenleme / Koordinat Değişimi | `🖱️ Seç / düzenle` Aracı + Elemana Tıkla |
| **3D Görünüm** | Kamerayı Döndür (Orbit) | Sol Tık + Sürükle |
| **3D Görünüm** | Kamerayı Kaydır (Pan) | Sağ Tık + Sürükle |
| **3D Görünüm** | Yakınlaş / Uzaklaş (Zoom) | Fare Tekerleği veya İki Parmak Kıstırma |

---

## 🛠️ Kullanılan Teknolojiler

* **HTML5 Canvas API** (Retina / High-DPI ölçeklemeli 2D CAD motoru)
* **Three.js (r128)** & **OrbitControls** (WebGL tabanlı 3D BIM ve gölge motoru)
* **Tailwind CSS** (Modern karanlık tema stüdyo arayüzü)
* **jsPDF** (Türkçe karakter uyumlu mimari metraj raporu üretimi)

---

## 📄 Lisans

Bu proje [MIT Lisansı](LICENSE) altında lisanslanmıştır. Dilediğiniz gibi kullanabilir, geliştirebilir ve paylaşabilirsiniz.
