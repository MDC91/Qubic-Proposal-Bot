<div align="center">

# 🤖 Qubic Proposal Bot

### **13 Dilde Otomatik Proposal Özetleri Qubic Topluluğu İçin**

<img width="250" height="250" alt="icon_2" src="https://github.com/user-attachments/assets/c960ae79-b84e-4b65-b540-360528faf126" />

---  
</div>

## 📖 İçindekiler

- [🚀 Proje Hakkında](#-proje-hakkında)
- [🏗️ Mimari & Teknoloji](#️-mimari--teknoloji)
- [📋 Desteklenen Diller](#-desteklenen-diller)
- [🎯 Detaylı Özellikler](#-detaylı-özellikler)
- [💬 Discord Kullanımı](#-discord-kullanımı)
  - [Botu Sunucunuza Ekleyin](#botu-sunucunuza-ekleyin)
  - [Discord Komutları](#discord-komutları)
- [📱 Telegram Kullanımı](#-telegram-kullanımı)
  - [Botu Grubunuza Ekleyin](#botu-grubunuza-ekleyin)
  - [Telegram Komutları](#telegram-komutları)
- [⚙️ Durum Yönetimi](#️-durum-yönetimi)
- [❓ Sık Sorulan Sorular](#-sık-sorulan-sorular)
- [🛠️ Destek](#️-destek)

## 🚀 Proje Hakkında

**Qubic Proposal Bot**, Qubic topluluğu için özel olarak geliştirilmiş, yeni yönetişim proposal'larını otomatik olarak tespit eden, AI kullanarak 13 farklı dilde özetleyen ve Discord sunucuları ile Telegram gruplarında yayınlayan bir bottur.

### 🌟 Ana Faydalar

- **🔍 Otomatik Tespit** - Yeni Qubic proposal'larını sürekli olarak izler
- **🌍 Çok Dilli Erişilebilirlik** - Proposal'ları İngilizce konuşmayan topluluk üyeleri için kullanılabilir hale getirir
- **🤖 AI Destekli Özetler** - Doğru, anlaşılması kolay özetler için DeepSeek AI kullanır
- **⏰ Zamanında Bildirimler** - Yeni proposal'ları yayınlandıktan 15 dakika içinde paylaşır
- **📊 Oylama Sonuçları** - Her epoch sonunda sonuçları otomatik olarak yayınlar

## 🏗️ Mimari & Teknoloji

Bot, sağlam bir çok platformlu mimariye dayanmaktadır:

### Çekirdek Bileşenler

- **Qubic API Entegrasyonu** - Aktif ve tamamlanmış proposal'ları alır
- **DeepSeek AI** - Çok dilli özetler oluşturur
- **Discord & Telegram Köprüleri** - Çapraz platform dağıtım
- **GitHub Tabanlı Depolama** - Kalıcı durum yönetimi ve önbellekleme
- **Akıllı Önbellekleme** - Yinelenen API çağrılarını önler

## 📋 Desteklenen Diller

Bot şu anda **13 dili** desteklemektedir:

| Dil | Kod |
|----------|------|
| Almanca | `de` |
| İngilizce | `en` |
| Fransızca | `fr` |
| İspanyolca | `es` |
| İtalyanca | `it` |
| Portekizce | `pt` |
| Rusça | `ru` |
| Japonca | `ja` |
| Çince | `zh` |
| Korece | `ko` |
| Arapça | `ar` |
| Türkçe | `tr` |
| Vietnamca | `vi` |

## 🎯 Detaylı Özellikler

### 🤖 Otomatik Proposal Tespiti
- **15 Dakikalık Aralık** - Düzenli olarak yeni proposal'ları kontrol eder
- **Epoch Tabanlı İşleme** - Epoch başına ayrı durum yönetimi
- **Yinelenen Tespiti** - Çoklu bildirimleri önler

### 🧠 Akıllı AI Özetleri
- **Bağlam Farkında Özetleme** - Her proposal'dan anahtar noktaları çıkarır
- **Dile Özgü Biçimlendirme** - Kültürel nüanslara uyarlanmış
- **Önbellek Mekanizması** - Aynı proposal'lar için yinelenen AI çağrılarını önler

### 🔄 Sağlam Durum Yönetimi
- **Sunucu/Sohbet Başına Durum** - Her topluluk kendi durumunu yönetir
- **GitHub Kalıcılığı** - Durumlar yeniden başlatmalardan sonra hayatta kalır
- **Otomatik Temizlik** - Eski epoch verilerini kaldırır

### 🌐 Çok Platform Desteği
- **Sorunsuz Discord Entegrasyonu** - Slash komutları ve gömülü mesajlar
- **Telegram Optimizasyonu** - Satır içi klavyeler ve Markdown desteği
- **Tutarlı Deneyim** - Her iki platformda aynı özellikler

## 💬 Discord Kullanımı

### Botu Sunucunuza Ekleyin
1. [**Davet bağlantısını**](https://discord.com/oauth2/authorize?client_id=1400149716385267835&permissions=2147568640&integration_type=0&scope=applications.commands+bot) kullanın
2. **Yönetici izinleri** verin ve botu istediğiniz kanala ekleyin
3. `/setup` ile **kurulum** yapın

### Discord Komutları

| **Komut** | **Açıklama** | **Parametreler** |
|-------------|-----------------|----------------|
| ❔ `/help` | Yardım gösterir | Detaylı yardım ve talimatlar |
| ⚙️ `/setup` | Botu sunucunuz için ayarlar | • `channel`: Proposal özetleri için kanal<br>• `language`: Özetler için dil |
| ℹ️ `/info` | Bot durumu hakkında detaylı bilgi gösterir | • Yapılandırılmış kanal ve dil<br>• Mevcut epoch<br>• Aktif proposal sayısı<br>• DeepSeek API durumu<br>• Bot çalışma süresi<br>• Kontrol aralığı |

## 📱 Telegram Kullanımı

### Botu Grubunuza Ekleyin
1. **Grubu yönet**
2. **Üye ekle**
3. **Bot ara:** `@QubicTranslationBot`
4. **Gruba yönetici olarak ekle**
5. **"Konuları yönet"i etkinleştir** <br>

<img width="363" height="621" alt="yönetici_hakları" src="https://github.com/user-attachments/assets/f11920b4-213a-4361-aaf8-cd66f2fcc383" />

6. **Kurulumu gerçekleştir** `/setup` ile

> [!IMPORTANT]
> `/setup` komutu yeni "Proposals" konusunu oluşturur. Konuyu daha sonra yeniden adlandırabilirsiniz. Yönetici hakları verilmezse bot ana sohbeti yedek olarak kullanır.

### Telegram Komutları

| **Komut** | **Açıklama** | **Parametreler** |
|-------------|-----------------|----------------|
| ❔ `/start` veya `/help` | Yardım gösterir | Detaylı yardım ve talimatlar |
| ⚙️ `/setup` | Dil seçimi için satır içi klavye açar | • Dil seçenekleri ile satır içi klavye<br>• İstenen dili seçin |
| ℹ️ `/info` | Bot durumu hakkında detaylı bilgi gösterir | • Yapılandırılmış sohbet ve dil<br>• Mevcut epoch<br>• Aktif proposal sayısı<br>• DeepSeek API durumu<br>• Bot çalışma süresi<br>• Kontrol aralığı |

## ⚙️ Durum Yönetimi

Bot her epoch için şunları yönetir:

- **İşlenmiş Proposal'lar** - Yinelenmelerden kaçınma
- **Proposal Sayacı** - Epoch başına sürekli numaralandırma
- **Dile Özgü Durumlar** - Veri kaybı olmadan dil değiştirmeyi sağlar

## ❓ Sık Sorulan Sorular

### 🤔 Genel Sorular

**S: Hangi diller destekleniyor?**  
C: Şu anda 13 dil: Almanca, İngilizce, Fransızca, İspanyolca, İtalyanca, Portekizce, Rusça, Japonca, Çince, Korece, Arapça, Türkçe, Vietnamca.

**S: Proposal özetleri ne kadar güncel?**  
C: Yeni proposal'lar yayınlandıktan 15 dakika içinde tespit edilir ve özetlenir.

**S: Daha sonra dili değiştirebilir miyim?**  
C: Evet, sadece `/setup` komutunu tekrar kullanın. Zaten işlenmiş proposal'lar yeni dilde sunulacaktır.

### 🔧 Teknik Sorular

**S: Bot komutlara yanıt vermiyor - ne yapmalıyım?**  
C: Botun gerekli izinlere sahip olduğundan emin olun ve komutu tekrar deneyin.

**S: Oylama sonuçları nasıl duyuruluyor?**  
C: Her Çarşamba saat 12:15 UTC'de, önceki epoch'un sonuçları otomatik olarak yayınlanır.

### 🌐 Platforma Özgü Sorular

**S: Tüm komutlar her iki platformda da çalışıyor mu?**  
C: Evet, temel işlevsellik Discord ve Telegram'da aynıdır.

**S: Botu hem Discord hem Telegram'da kullanabilir miyim?**  
C: Evet, botu her iki platformda paralel olarak kullanabilirsiniz.

**S: Botun Discord'da hangi izinlere ihtiyacı var?**  
C: Botun mesaj gönderme, bağlantı yerleştirme ve slash komutlarını kullanma izinlerine ihtiyacı vardır.

## 🛠️ Destek

Bot ile ilgili sorularınız veya sorunlarınız için lütfen şununla iletişime geçin:

**📞 Discord/Telegram İletişim:** MDC

**⚠️ Önemli:**  
Lütfen aşağıdaki bilgileri hazır bulundurun:
- Sorunun oluştuğu sunucu/sohbet ID'si
- Çalışmayan tam komut
- Sorunun zamanı
- Hata mesajı (mevcutsa)

---

<div align="center">

**🌍 Qubic Topluluğu İçin Bir Proje**  
*Herkesin, her dilde proposal'lara erişebilmesini sağlamak*

</div>
