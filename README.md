# 🅿️ İSPARK Park Yerleri iOS Uygulaması

Türkiye'deki İSPARK otoparklarının gerçek zamanlı doluluk durumunu, kapasite bilgilerini ve yüzdesel doluluk oranlarını gösteren modern bir iOS uygulaması.

## 📱 Özellikler

- ✅ **Gerçek Zamanlı Veriler**: İBB İSPARK API'sinden canlı otopark verileri
- 📊 **Detaylı İstatistikler**: Her otopark için kapasite, dolu ve boş yer bilgileri
- 📈 **Yüzdesel Gösterim**: Doluluk oranlarını görsel progress bar ile gösterim
- 🔍 **Gelişmiş Arama**: Park adı, ilçe ve park tipine göre arama
- 🎨 **Modern UI**: SwiftUI ile tasarlanmış kullanıcı dostu arayüz
- 🏷️ **Park Tipi Filtreleme**: Açık ve kapalı otoparkları ayırt etme
- 📍 **İlçe Bilgisi**: Her otoparkın bulunduğu ilçe bilgisi
- 🔄 **Pull-to-Refresh**: Aşağı çekerek verileri yenileme

## 🛠️ Teknolojiler

- **SwiftUI** - Modern iOS UI framework
- **Combine** - Reactive programming
- **URLSession** - Network işlemleri
- **Async/Await** - Modern concurrency
- **MVVM Architecture** - Clean architecture pattern

## 📖 Kullanım

### Ana Ekran
- Uygulama açıldığında tüm İSPARK otoparkları listelenir
- Her kart şu bilgileri gösterir:
  - Park adı
  - İlçe bilgisi
  - Park tipi (Açık/Kapalı)
  - Toplam kapasite
  - Boş yer sayısı
  - Dolu yer sayısı
  - Doluluk yüzdesi (progress bar ile)

### Arama
- Üst kısımdaki arama çubuğunu kullanarak:
  - Park adına göre arama yapabilirsiniz
  - İlçe adına göre filtreleyebilirsiniz
  - Park tipine göre arama yapabilirsiniz

### Veri Yenileme
- Aşağı çekerek (pull-to-refresh) verileri yenileyebilirsiniz
- Sağ üstteki yenile butonunu kullanabilirsiniz

## 🏗️ Proje Yapısı

```
ParkApp/
├── Models/
│   └── ParkYeri.swift          # Park yeri veri modeli
├── Services/
│   └── ParkYeriService.swift   # API servisi ve veri yönetimi
├── Views/
│   ├── ParkCardView.swift      # Park kartı görünümü
│   └── ParkListView.swift      # Ana liste görünümü
└── ParkAppApp.swift            # Uygulama entry point
```

## 🔌 API Entegrasyonu

Uygulama İBB İSPARK API'sini kullanmaktadır:

**Endpoint**: `https://api.ibb.gov.tr/ispark/Park`

**API Dokümantasyonu**: [İBB Açık Veri Portalı](https://data.ibb.gov.tr/dataset/ispark-otopark-listesi-web-servisi)

### API Response Formatı

```json
[
  {
    "parkID": 1487,
    "parkName": "0174 Vatan Caddesi PD Açık Otoparkı",
    "lat": "41.0157",
    "lng": "28.9405",
    "capacity": 397,
    "emptyCapacity": 361,
    "parkType": "AÇIK OTOPARK",
    "district": "FATİH"
  }
]
```

## 🎨 UI Özellikleri

### Renk Kodlaması
- **KAPALI OTOPARK**: Mor tonları
- **AÇIK OTOPARK**: Yeşil tonları
- **Doluluk Oranı**:
  - %0-70: Mavi (Düşük)
  - %70-90: Turuncu (Orta)
  - %90-100: Kırmızı (Yüksek)

### Tasarım Özellikleri
- Modern kart tasarımı
- Gradient arka planlar
- Smooth animasyonlar
- Dark mode desteği
- Responsive layout

## 📸 Ekran Görüntüleri

_(Ekran görüntüleri eklenecek)_

## 🤝 Katkıda Bulunma

1. Fork edin
2. Feature branch oluşturun (`git checkout -b feature/amazing-feature`)
3. Commit edin (`git commit -m 'Add some amazing feature'`)
4. Push edin (`git push origin feature/amazing-feature`)
5. Pull Request açın

## 📝 Lisans

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için `LICENSE` dosyasına bakın.

## 👤 Yazar

**SONER KILINÇ**

- GitHub: [@sonerkilinc](https://github.com/sonerkilinc)

## 🙏 Teşekkürler

- İBB (İstanbul Büyükşehir Belediyesi) - API desteği için
- İSPARK A.Ş. - Veri sağladığı için

## 📞 İletişim

Sorularınız veya önerileriniz için issue açabilirsiniz.

---

⭐ Bu projeyi beğendiyseniz yıldız vermeyi unutmayın!



<img width="344" height="738" alt="image" src="https://github.com/user-attachments/assets/128e8f2b-cd3f-4055-be0c-60a952e70028" />
