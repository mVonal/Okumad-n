# Signal

**Geliştirici:** Signal Messenger LLC
**Üst kuruluş:** Signal Technology Foundation (501c3 kâr amacı gütmeyen vakıf)
**Merkez:** Mountain View, California, ABD
**Platform:** Android, iOS, Windows, macOS, Linux
**Açık kaynak:** Evet — github.com/signalapp (AGPL-3.0)
**Belge tarihi:** Gizlilik Politikası: 25 Mayıs 2018 (yürürlükte)
**Kaynak:** https://signal.org/legal/

> Bu analiz yalnızca bilgilendirme amaçlıdır, hukuki tavsiye niteliği
> taşımaz. Tüm tespitler Signal'in kendi yayımladığı belgeler esas
> alınarak hazırlanmıştır.

---

## Özet

Signal, güvenlik araştırmacıları ve gizlilik savunucuları tarafından
mesajlaşma uygulamaları arasında altın standart olarak gösterilen
platformdur. Temel farkı şudur: toplamadığı veriyi paylaşması
mümkün değildir. WhatsApp ile kıyaslandığında veri minimizasyonu
açısından tartışmasız üstündür. Ancak ABD merkezli bir şirket
olması ve Türkçe yasal belgelerinin bulunmaması dikkat gerektiren
noktalardır.

---

## Skorlar

| Kriter | Değer |
|---|---|
| Genel risk skoru | 🟢 2 / 10 |
| Veri yurt dışı riski | 🟡 Orta (ABD sunucuları, ama veri minimal) |
| Metadata toplama | 🟢 Minimal |
| Şeffaflık | 🟢 Açık kaynak, denetlenebilir |
| Ticari motivasyon | 🟢 Kâr amacı gütmeyen vakıf |

---

## Güçlü Yönler

### Kesin Veri Satmama Taahhüdü

Signal'in kendi Hizmet Şartlarında şu ifade yer almaktadır:
"Signal does not sell, rent or monetize your personal data
or content in any way — ever."

Bu ifade bir pazarlama sloganı değil, hizmet şartlarına
yazılmış bağlayıcı bir taahhüttür.

**Kaynak:** Signal Hizmet Şartları "Privacy of user data" maddesi

---

### Toplanan Veri Son Derece Sınırlı

Signal'in Gizlilik Politikasına göre platformun elinde
bulunan tek kişisel veri **telefon numaranızdır.** Bunun
yanı sıra teknik işleyiş için gerekli rastgele üretilmiş
kimlik doğrulama token'ları saklanmaktadır.

Mesaj içerikleri, grup üyelikleri, profil bilgileri ve
iletişim örüntüleri uçtan uca şifreli olduğundan
Signal sunucuları bunlara **erişememektedir.**

Bu taahhüdün gerçek dünyada sınanmış bir kanıtı
mevcuttur: 2016 yılında ABD Federal Soruşturma Bürosu
(FBI) bir mahkeme kararıyla Signal'den kullanıcı verisi
talep etmiştir. Signal'in verebileceği yalnızca iki
bilgi olmuştur: hesabın oluşturulduğu tarih aralığı ve
sunucuya son bağlantı tarihi. Bu süreç kamuya açık
mahkeme belgeleriyle kayıt altındadır.

**Kaynak:** Signal Gizlilik Politikası "Account Information"
ve "Messages" bölümleri · FBI mahkeme belgesi (2016,
kamuya açık)

---

### Rehber Gizliliği Kriptografik Olarak Korunuyor

Gizlilik Politikasına göre hangi rehber kişilerinin
Signal kullandığını tespit etmek için telefon numaraları
**kriptografik hash** yöntemiyle işlenmektedir. Bu
yöntemde Signal sunucuları rehberdeki gerçek numaraları
görmez; yalnızca hash değerlerini karşılaştırır.

Bu yaklaşım WhatsApp ve BiP'ten temel olarak ayrışan
bir gizlilik tasarımıdır.

**Kaynak:** Signal Gizlilik Politikası "Contacts" bölümü

---

### Açık Kaynak ve Bağımsız Denetim

Signal'in tüm istemci uygulamaları ve sunucu kodu
AGPL-3.0 lisansı altında GitHub'da kamuya açıktır.
Bağımsız güvenlik araştırmacıları kodu her an
denetleyebilmektedir. Bu durum "güvenilir" olduğunu
söylemek ile "denetlenebilir olduğu için güvenilir"
olmak arasındaki kritik farkı temsil eder.

**Kaynak:** github.com/signalapp

---

### Kâr Amacı Gütmeyen Yapı

Signal Technology Foundation, ABD'de 501(c)(3) statüsünde
tescilli bir kâr amacı gütmeyen vakıftır. Geliri
bağışlardan oluşmaktadır. Reklam geliri modeli yoktur;
dolayısıyla kullanıcı davranışlarını monetize etme
motivasyonu da yoktur.

---

## 🟡 Dikkat Edilmesi Gereken Maddeler

### ABD Merkezli Kuruluş

Signal Messenger LLC, Mountain View, California'da
kayıtlı bir ABD şirketidir. Hizmet Şartlarının
"Resolving Disputes" maddesine göre tüm uyuşmazlıklar
**Kuzey Kaliforniya mahkemelerinde, Kaliforniya hukukuna
göre** çözülür.

Bu madde WhatsApp ile aynı yapıdadır. Farkı şudur:
Signal'in elinde paylaşabileceği anlamlı kullanıcı
verisi bulunmadığından ABD hükümeti taleplerine
verebileceği yanıt son derece sınırlıdır.

**Kaynak:** Signal Hizmet Şartları "Resolving disputes" maddesi

---

### Tazminat Tavanı 100 USD

"Limitation of Liability" maddesine göre Signal'in
azami sorumluluğu **100 USD** ile sınırlandırılmıştır.
Bu madde WhatsApp ile aynıdır.

**Kaynak:** Signal Hizmet Şartları "Limitation of liability"

---

### Gizlilik Politikası Güncelleme Tarihi: 2018

Signal'in mevcut Gizlilik Politikası 25 Mayıs 2018
tarihlidir. Yedi yıldır resmi olarak güncellenmemiş
olması şeffaflık açısından bir eksikliktir; güncel
uygulama ile belge arasında fark olup olmadığını
doğrulamak kullanıcılar açısından güçleşmektedir.

**Kaynak:** Signal Gizlilik Politikası "Updated" notu

---

### Telefon Numarası Zorunlu

Hesap açmak için telefon numarası zorunludur. Bu durum
tam anonimliği engellemektedir. Signal, Mart 2024
itibarıyla kullanıcı adı özelliğini hayata geçirmiş
olup artık telefon numaranızı diğer kullanıcılardan
gizleyebilirsiniz — ancak kayıt için numara zorunluluğu
devam etmektedir.

**Kaynak:** Signal Hizmet Şartları "Account Registration"
· Wikipedia Signal maddesi (kullanıcı adı özelliği)

---

### Şartlar Değişebilir

Hizmet Şartlarına göre Signal koşulları istediği zaman
güncelleyebilir. Kullanmaya devam etmek yeni şartları
kabul etmek anlamına gelir.

**Kaynak:** Signal Hizmet Şartları "General" bölümü

---

## WhatsApp ile Karşılaştırma

| Kriter | WhatsApp | Signal |
|---|---|---|
| Veri satışı | Belirsiz 🔴 | Kesinlikle yok 🟢 |
| Mesaj içeriği | Şifreli, erişilemiyor | Şifreli, erişilemiyor |
| Metadata toplama | Kapsamlı 🔴 | Minimal 🟢 |
| Rehber işleme | Düz metin yükleme 🔴 | Kriptografik hash 🟢 |
| Açık kaynak | Hayır 🔴 | Evet 🟢 |
| Ticari yapı | Kâr amaçlı (Meta) 🔴 | Kâr amacı gütmeyen 🟢 |
| Sunucu konumu | ABD 🔴 | ABD 🟡 |
| Mahkeme yeri | Kaliforniya 🔴 | Kaliforniya 🟡 |
| Hükümete verilebilecek veri | Kapsamlı 🔴 | Neredeyse yok 🟢 |

---

## Kimler İçin Uygundur?

- Maksimum gizlilik ve güvenlik arayanlar
- Gazeteciler, avukatlar, aktivistler
- Teknik güvenilirliği kanıtlanmış platform isteyenler
- Açık kaynak denetimi öncelik olarak görenler

## Kimler İçin Sınırlı Kalabilir?

- Verilerinin Türkiye'de kalmasını kesin olarak
  isteyenler (BiP veya NEXT daha uygun)
- Türkçe yasal belge arayanlar
- Yalnızca Türkçe arayüz isteyenler

---

## Kaynaklar

| Belge | URL | Erişim Tarihi |
|---|---|---|
| Hizmet Şartları ve Gizlilik Politikası | https://signal.org/legal/ | 23.04.2026 |
| Kaynak Kodu | https://github.com/signalapp | 23.04.2026 |
| GDPR Desteği | https://support.signal.org/hc/en-us/articles/360007059412 | 23.04.2026 |
