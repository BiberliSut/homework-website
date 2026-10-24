# SynapseMap AI · Project Runtime

Tutoring dersi için sunudaki **SynapseMap AI** proje önerisine dayanan, yalnızca tarayıcıda çalışan bir arayüz demonstrasyonudur. Holo-glass paneller, Dynamic Island benzeri üst durum kapsülü, responsive gezinme, proje zaman çizelgesi, paydaş matrisi, KPI/risk panosu, simüle edilmiş sinyal grafiği ve rapor eki olarak açıklamalı örnek artefaktlar içerir.

## Çalıştırma

Python 3 kuruluysa bu klasörde terminal açıp şunu çalıştırın:

```bash
python3 -m http.server 8000
```

Ardından tarayıcıda `http://localhost:8000` adresini açın. Alternatif olarak `index.html` dosyasını doğrudan tarayıcıda açabilirsiniz; yerel sunucu yöntemi daha tutarlı çalışır. Sunucuyu durdurmak için terminalde `Ctrl+C`.

## Dosyalar

- `index.html` — uygulama iskeleti ve içerik
- `styles.css` — holo-glass / responsive arayüz
- `app.js` — sayfa yönlendirme, simülasyon kontrolleri, örnek grafik, checklist ve yerel etkileşimler

## Etkileşimler

- Sol menüden Mission Control, Signal Runtime, Implementation, Stakeholders, M&E/KPI ve Evidence Vault sayfaları arasında geçiş yapılır.
- **Start simulation / Run demo stream** sentetik node-edge animasyonu ve örnek dalga grafiği başlatır; gerçek sensöre, veri kümesine veya modele bağlanmaz.
- Implementation sayfasındaki checklist işaretleri tarayıcının `localStorage` alanında saklanır.
- Log/update düğmeleri yalnızca sayfa içi demo etkinlik akışına not ekler; bir sunucuya gönderim yapmaz.
- Capture düğmesi tarayıcı yazdırma penceresini açar; oradan PDF olarak kaydedebilir veya işletim sistemi ekran görüntüsü aracını kullanabilirsiniz. Belirli bir paneli kanıt olarak alırken tarayıcı yakınlaştırmasını ve pencere boyutunu ayarlayın.

## Önemli akademik not

Bu uygulamadaki KPI değerleri, etkinlik kayıtları, paydaş check-in soruları, poster, katılım çağrısı, ekran görüntüsü örneği ve log kartları **temsili/simüle edilmiş materyallerdir**. Gerçek katılımcı verisi, gerçek anket yanıtı, gerçek proje toplantısı, etik kurul onayı, gerçek deney sonucu veya tamamlanmış uygulama kanıtı değildir. Raporunuzda her eki “arayüz demonstrasyonu / mock artifact” olarak açıklayın ve gerçek uygulama kanıtı olarak göstermeyin. Çalışmanızda gerçekten elde ettiğiniz fotoğraf, toplantı kaydı ya da sonuçlar oluşursa bunları izin ve mahremiyet koşullarına uygun biçimde ayrıca ekleyin.

Arayüz dış servis veya paket gerektirmez. Yazı tipi internet varsa Google Fonts'tan yüklenir; bağlantı yoksa sistem sans-serif yazı tipine düşer.
