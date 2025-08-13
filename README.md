# Kahve Demleme Uygulaması - Coffee Brewing Application

Bu proje, Espresso ve V60 kahve demleme süreçlerini kaydedip yönetebileceğiniz açık kaynaklı bir web uygulamasıdır. Kullanıcılar demleme tariflerini oluşturabilir, kaydedebilir, güncelleyebilir ve dışa/içe aktarabilirler.

This project is an open-source web application that allows you to record and manage Espresso and V60 coffee brewing processes. Users can create, save, update, and export/import brewing recipes.

## 🌟 Özellikler / Features

### ☕ Kahve Türleri / Coffee Types
- **Espresso**: Espresso oranı ayarlanabilir (varsayılan 2.0)
- **V60**: Döküş adımları ile detaylı demleme süreci

### 📱 Kullanıcı Arayüzü / User Interface
- Modern ve duyarlı tasarım (Tailwind CSS)
- Türkçe ve İngilizce dil desteği
- Mobil uyumlu arayüz

### 🔧 Demleme Ayarları / Brewing Settings
- Su miktarına göre veya gramaja göre hesaplama
- Su sıcaklığı ayarı (varsayılan 94°C)
- Değirmen modeli seçimi
- Öğütüm aralığı (klik) ayarı

### 📊 Demleme Takibi / Brewing Tracking
- Gerçek zamanlı kronometre
- Döküş adımları takibi (V60 için)
- Demleme notları ve yorumları
- Otomatik su miktarı hesaplama

### 💾 Veri Yönetimi / Data Management
- Reçete kaydetme ve güncelleme
- JSON formatında dışa/içe aktarma
- LocalStorage ile yerel veri saklama
- Arşiv yönetimi

## 🚀 Kurulum / Installation

1. Projeyi indirin veya klonlayın
2. `index.html` dosyasını herhangi bir modern web tarayıcısında açın
3. Uygulama otomatik olarak çalışmaya başlayacaktır

## 📖 Kullanım Kılavuzu / Usage Guide

### 🆕 Yeni Reçete Oluşturma / Creating New Recipe

1. **Kahve Türü Seçimi**: Espresso veya V60 butonuna tıklayın
2. **Temel Bilgiler**:
   - Reçete ismi girin
   - Kahve bilgisi ekleyin
   - Su miktarı veya kahve gramajını belirleyin
3. **Demleme Ayarları**:
   - Su sıcaklığını ayarlayın
   - Değirmen modelini seçin
   - Öğütüm aralığını belirleyin

### ☕ Espresso Reçeteleri / Espresso Recipes

- **Oran Ayarı**: Espresso oranını 1.0-3.0 arasında ayarlayın
- **Hesaplama**: Su miktarı veya kahve gramajına göre otomatik hesaplama
- **Demleme**: Basit kronometre ile demleme süreci takibi

### 🌊 V60 Reçeteleri / V60 Recipes

- **Sertlik Seçimi**: Yoğun, Normal, Açık, Makine seçenekleri
- **Döküş Adımları**: Zaman ve miktar belirterek döküş planı oluşturun
- **Bitiş Zamanı**: Toplam demleme süresini belirleyin
- **Görsel Takip**: Dairesel ilerleme göstergesi ve adım takibi

### 📱 Demleme Süreci / Brewing Process

1. **Reçete Seçimi**: Önceki demlemelerden seçim yapın
2. **Demlemeye Başla**: "Kaydet ve Demlemeye Geç" butonuna tıklayın
3. **Süreç Takibi**: Kronometre ve döküş adımlarını takip edin
4. **Not Ekleme**: Demleme sırasında önemli anları kaydedin
5. **Tamamlama**: Demlemeyi bitir ve yorumları kaydedin

### 💾 Arşiv Yönetimi / Archive Management

- **Reçete İndirme**: Tüm reçeteleri JSON formatında indirin
- **Reçete Yükleme**: Daha önce indirilen reçeteleri yükleyin
- **Düzenleme**: Mevcut reçeteleri düzenleyin veya silin
- **Yorum Ekleme**: Demleme sonrası yorumlar ekleyin

## 🔧 Teknik Detaylar / Technical Details

### 🏗️ Teknolojiler / Technologies
- HTML5, CSS3, JavaScript (ES6+)
- Tailwind CSS (CDN)
- LocalStorage API
- Modern Web APIs

### 📁 Dosya Yapısı / File Structure
```
v60-main/
├── index.html          # Ana uygulama dosyası
├── LICENSE            # MIT lisans dosyası
└── README.md          # Bu dosya
```

### 💾 Veri Formatı / Data Format
Reçeteler JSON formatında saklanır:
```json
{
  "type": "V60",
  "recipeName": "V60 Demo",
  "coffeeInfo": "Ethiopian Yirgacheffe",
  "grammage": "15",
  "waterAmount": "250",
  "temperature": "94",
  "grinder": "Molent g50",
  "clicks": "37",
  "v60Hardness": "Normal",
  "pourSteps": [...],
  "endTime": "02:45"
}
```

## 🆘 Yardım ve Sorun Giderme / Help & Troubleshooting

### ❓ Sık Sorulan Sorular / FAQ

**Q: Uygulama çalışmıyor, ne yapmalıyım?**
A: Modern bir web tarayıcısı kullandığınızdan emin olun (Chrome, Firefox, Safari, Edge)

**Q: Reçetelerim kayboldu, nasıl geri getirebilirim?**
A: Arşiv ekranından "Reçete Yükle" butonunu kullanarak daha önce indirdiğiniz dosyayı yükleyin

**Q: Döküş adımları çalışmıyor**
A: V60 kahve türünü seçtiğinizden ve döküş adımları eklediğinizden emin olun

**Q: Dil nasıl değiştirilir?**
A: Sağ üst köşedeki dil seçim menüsünden TR/EN seçeneğini kullanın

### 🐛 Bilinen Sorunlar / Known Issues

- LocalStorage veri limiti (genellikle 5-10MB)
- Eski tarayıcılarda uyumluluk sorunları
- Çok büyük reçete listelerinde performans düşüşü

### 🔄 Güncelleme / Updates

Uygulama sürüm 0.6 ile aşağıdaki özellikler eklendi:
- Gelişmiş döküş adımları sistemi
- Dairesel ilerleme göstergesi
- Bitiş zamanı ayarı
- Espresso/V60 ayrımı
- Çok dilli destek

## 🤝 Katkıda Bulunma / Contributing

Bu proje açık kaynak kodludur. Katkılarınızı bekliyoruz:

1. Projeyi fork edin
2. Yeni özellik dalı oluşturun (`git checkout -b feature/amazing-feature`)
3. Değişikliklerinizi commit edin (`git commit -m 'Add amazing feature'`)
4. Dalınızı push edin (`git push origin feature/amazing-feature`)
5. Pull Request oluşturun

## 📄 Lisans / License

Bu proje MIT lisansı altında lisanslanmıştır. Detaylar için [LICENSE](LICENSE) dosyasına bakın.

## 👨‍💻 Geliştirici / Developer

**AbdullahKeles81** - [GitHub](https://github.com/AbdullahKeles81)

## 🙏 Teşekkürler / Acknowledgments

- Tailwind CSS ekibine modern UI framework için
- Açık kaynak topluluğuna
- Kahve tutkunlarına ilham için

---

**Not**: Bu uygulama eğitim amaçlı geliştirilmiştir. Profesyonel kahve demleme için ek ekipman ve bilgi gerekebilir.

**Note**: This application is developed for educational purposes. Professional coffee brewing may require additional equipment and knowledge.
