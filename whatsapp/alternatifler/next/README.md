# NEXT Mesajlaşma

**Geliştirici:** 2N Medya Anonim Şirketi
**Merkez:** Şişli, İstanbul, Türkiye
**Destekleyen:** T3 Vakfı / Baykar ekosistemi
**Platform:** Android, iOS, macOS
**Çıkış tarihi:** Temmuz 2025
**İletişim:** info@2ntech.com.tr · developer@2ntech.com.tr

> Bu analiz yalnızca bilgilendirme amaçlıdır, hukuki tavsiye niteliği
> taşımaz. Tespitler NEXT'in uygulaması içinden temin edilen Gizlilik
> Politikası, Play Store/App Store açıklamaları ve kamuya açık teknik
> analizlere dayanmaktadır.

---

## Belge Durumu

| Belge | Durum |
|---|---|
| Gizlilik Politikası | Uygulama içinden temin edildi — kamuya açık URL yok |
| Kullanım Koşulları | **Bulunamadı** — kamuya açık bir belge mevcut değil |
| KVKK Aydınlatma Metni | Bulunamadı |

Hem Gizlilik Politikası'na hem de Kullanım Koşulları'na dışarıdan
erişilememesi tek başına önemli bir şeffaflık sorunudur.

KVKK'nın 10. maddesi ve GDPR'nin 13. maddesi uyarınca aydınlatma
yükümlülüğü, kayıt işlemi gerçekleştirilmeden önce yerine
getirilmelidir. Belgelerin yalnızca uygulama içinden erişilebilir
olması bu yükümlülükle çelişmektedir.

---

## Skorlar

| Kriter | Değer |
|---|---|
| Genel risk skoru | 🟡 5 / 10 |
| Uçtan uca şifreleme | 🟢 Var, varsayılan aktif |
| Belge şeffaflığı | 🔴 Kamuya açık URL yok, ToS bulunamadı |
| KVKK uyumu | 🔴 Atıf yok, Aydınlatma Metni yok |
| Metadata/veri toplama | 🟡 Sınırlı ama altyapı sağlayıcıları belirsiz |
| Hukuki çerçeve | 🔴 Yetkili mahkeme ve hukuk belirtilmemiş |
| Platform olgunluğu | 🔴 9 aylık, bağımsız denetim yok |
| Teknik mimari | 🟢 Matrix protokolü, kendi sunucu desteği |

---

## Teknik Mimari: Matrix Protokolü

NEXT'i diğer mesajlaşma uygulamalarından temel olarak ayıran mimari
tercih Matrix.org protokolüdür.

**Matrix nedir?** Açık kaynaklı, federatif bir iletişim protokolüdür.
Mastodon'un sosyal medyada yaptığını mesajlaşmada yapar: farklı
sunuculardaki kullanıcılar birbirleriyle iletişim kurabilir, hiçbir
merkezi otorite tüm trafiği göremez.

**Pratik sonuçları:**
- Kendi sunucunuzu kurarsanız verileriniz tamamen sizin kontrolünüzdedir
- Telefon numarası değil e-posta adresi ile kayıt olunur — bu
  WhatsApp ve BiP'e kıyasla daha anonim bir yapı sağlar
- Uygulama kurulumunda sunucu seçimi istenir

**Önemli uyarı:** Varsayılan sunucu olarak matrix.org önerilmektedir.
Matrix.org Avrupa merkezli bir organizasyondur. Kendi sunucunuzu
kurmadığınız takdirde verileriniz Türkiye'de barındırılmaz.

**Kaynak:** Euronews teknik analizi (31.07.2025) ·
Ekşi Sözlük kullanıcı deneyimleri

---

## Güçlü Yönler

### Uçtan Uca Şifreleme Varsayılan Olarak Aktif

Gizlilik Politikasının 2.1 maddesine göre tüm mesajlaşmalar,
sesli/görüntülü aramalar ve medya paylaşımları uçtan uca
şifrelidir. Şifreleme anahtarları yalnızca kullanıcı cihazlarında
saklanmaktadır. Sunucular, geliştiriciler ve üçüncü taraflar
içeriklere erişememektedir.

**Kaynak:** NEXT Gizlilik Politikası Madde 2.1

---

### Rehber Sunucuya Gönderilmiyor

Gizlilik Politikasının 1.5 maddesine göre rehber erişimi yalnızca
mevcut kullanıcıları eşleştirmek için kullanılmakta ve
**rehber verileri sunucuya kaydedilmez veya paylaşılmaz.**

Ayrıca NEXT'in Matrix tabanlı yapısı telefon numarası yerine
e-posta adresiyle çalıştığından, WhatsApp ve BiP'teki gibi
rehber yükleme mekanizması mimari olarak farklı işlemektedir.

**Kaynak:** NEXT Gizlilik Politikası Madde 1.5 ·
Ekşi Sözlük kullanıcı gözlemleri

---

### Reklam ve Pazarlama Amaçlı Veri Paylaşımı Yok

Gizlilik Politikasının 3. maddesine göre veriler pazarlama veya
reklam amacıyla üçüncü taraflarla paylaşılmamaktadır.

**Kaynak:** NEXT Gizlilik Politikası Madde 3

---

### İzin Bazlı Hassas Veri Erişimi

Mikrofon, kamera ve konum gibi hassas verilere yalnızca kullanıcıdan
açık izin alındıktan sonra erişilmektedir. İzinler cihaz
ayarlarından geri alınabilmektedir.

**Kaynak:** NEXT Gizlilik Politikası Madde 1

---

### Kendi Sunucu Kurabilme

Kurumlar veya bireyler kendi sunucularını kurarak tüm iletişim
verilerini tamamen kendi altyapılarında tutabilir. Bu özellik
WhatsApp, BiP ve Signal'de mevcut değildir.

---

### Türkiye'de Kurulu Şirket

Geliştirici 2N Medya Anonim Şirketi, Türk hukukuna tabi yerli
bir şirkettir.

---

## 🔴 Kırmızı Bayraklar

### Kullanım Koşulları Belgesi Bulunamadı

Araştırma sürecinde NEXT'e ait kamuya açık bir Kullanım Koşulları
belgesi tespit edilememiştir. Bu durum kritik bir eksikliktir:
kullanıcı hesabının nasıl sonlandırılabileceği, hangi içerikler
yasak kapsamında değerlendirileceği, ihlal durumunda neler olacağı,
ve platformun kendisine hangi hakları sakladığı gibi temel sorular
yanıtsız kalmaktadır.

---

### Yetkili Hukuk ve Mahkeme Belirtilmemiş

Gizlilik Politikasında uyuşmazlık durumunda hangi ülke hukukunun
ve hangi mahkemelerin yetkili olduğu hiç belirtilmemiştir. Bu bilgi
olmadan kullanıcıların yasal başvuru yolu belirsizdir.

WhatsApp (Kaliforniya), Signal (Kaliforniya) ve BiP (Türkiye)
bu bilgiyi açıkça sunmaktadır. NEXT bu konuda sessizdir.

---

### KVKK'ya Hiç Atıf Yapılmamış

Gizlilik Politikasında Türkiye'nin 6698 sayılı Kişisel Verilerin
Korunması Kanunu'na hiç atıf yapılmamaktadır. Türkiye'de faaliyet
gösteren ve Türk kullanıcılara hizmet veren bir şirket için bu
kritik bir eksikliktir.

Kıyaslama: BiP'in Aydınlatma Metni hem KVKK hem GDPR'ye açıkça
atıf yapmakta ve her madde için yasal dayanağını göstermektedir.

---

### Altyapı Sağlayıcılarının Kimliği Belirsiz

Gizlilik Politikasının 3. maddesine göre veriler
"sunucu altyapı sağlayıcıları (örneğin: mesaj teslimi veya analiz
platformları)" ile paylaşılabilmektedir. Bu sağlayıcıların
hangi şirketler olduğu belirtilmemiştir. Hangi ülkelerde veri
işlenebileceği de açık değildir.

**Kaynak:** NEXT Gizlilik Politikası Madde 3

---

### Varsayılan Sunucu Türkiye'de Değil

Uygulama kurulumunda varsayılan sunucu matrix.org'dur.
Matrix.org, Avrupa merkezlidir. Kendi sunucunuzu kurmadığınız
takdirde verileriniz Türkiye'de barındırılmaz. "Veri Türkiye'de"
iddiası yalnızca kendi sunucusu kuranlar için geçerlidir.

**Kaynak:** Euronews teknik analizi (31.07.2025)

---

### Veri Saklama Süresi Muğlak

Politikanın 6. maddesinde veriler "artık ihtiyaç kalmadığında"
silineceği belirtilmektedir. Bu somut bir süre değildir. BiP'in
"azami 2 yıl" gibi net bir sınır koymasıyla kıyaslandığında
belirsiz kalmaktadır.

**Kaynak:** NEXT Gizlilik Politikası Madde 6

---

## 🟡 Dikkat Edilmesi Gereken Maddeler

### Kapalı Kaynak Uygulama Katmanı

Matrix protokolü açık kaynak olsa da NEXT'in bu protokol üzerine
inşa ettiği uygulama katmanının kaynak kodu kamuya açık değildir.
Protokolün güvenli olması uygulamanın her katmanının güvenli
olduğu anlamına gelmez.

---

### Bağımsız Güvenlik Denetimi Yok

NEXT'in bağımsız bir güvenlik firması tarafından denetlenip
denetlenmediğine dair kamuoyuyla paylaşılmış bir bilgi yoktur.
Signal'in bağımsız denetim geçmişi bu açıdan NEXT'ten ayrışmaktadır.

---

### Cihaz ID ve Kilitlenme Logları Toplanıyor

Gizlilik Politikasının 1.3 ve 1.4 maddelerine göre cihaz
tanımlayıcıları ve kilitlenme/teşhis verileri toplanmaktadır.
Bu verilerin kullanıcı kimliğiyle doğrudan eşleştirilmediği
belirtilmekte, ancak hangi koşullarda anonimleştirileceği
açıklanmamaktadır.

**Kaynak:** NEXT Gizlilik Politikası Madde 1.3, 1.4

---

### Yeni Platform — Track Record Yok

NEXT Temmuz 2025'te yayımlanmıştır. Henüz 9 aylıktır.
Türkiye'de önceki yerli mesajlaşma girişimleri (PTT Messenger,
BİP'in ilk dönemi) benzer vaatlerle çıkıp beklenen olgunluğa
erişememiştir. NEXT'in uzun vadeli sürdürülebilirliği henüz
sınanmamıştır.

---

## Karşılaştırma

| Kriter | WhatsApp | BiP | Signal | NEXT |
|---|---|---|---|---|
| Genel risk skoru | 🔴 8/10 | 🟡 4/10 | 🟡 3/10 | 🟡 5/10 |
| Sunucu konumu | ABD 🔴 | Türkiye 🟢 | ABD 🟡 | Değişken* 🟡 |
| Kendi sunucu | Hayır 🔴 | Hayır 🔴 | Hayır 🔴 | Evet 🟢 |
| Rehber sunucuya gidiyor | Evet 🔴 | Evet 🟡 | Hash 🟢 | Gitmiyor 🟢 |
| Protokol açık kaynak | Hayır 🔴 | Hayır 🔴 | Evet 🟢 | Kısmi 🟡 |
| Kamuya açık ToS | Var 🟢 | Var 🟢 | Var 🟢 | **Yok** 🔴 |
| KVKK atfı | İhlal 🔴 | Açık 🟢 | Yok 🟡 | **Yok** 🔴 |
| Yetkili mahkeme | Kaliforniya 🔴 | Türkiye 🟢 | Kaliforniya 🟡 | **Belirsiz** 🔴 |
| Bağımsız denetim | Yok 🟡 | Yok 🟡 | Var 🟢 | Yok 🔴 |
| Platform olgunluğu | Yüksek 🟢 | Orta 🟡 | Yüksek 🟢 | Yeni 🔴 |

*Varsayılan matrix.org (Avrupa). Kendi sunucu kurulursa değişir.

---

## Sonuç

NEXT, teknik tercihler açısından — Matrix protokolü, kendi sunucu
desteği, rehberin sunucuya gönderilmemesi, e-posta tabanlı kayıt —
rakiplerine kıyasla dikkat çekici bir temel üzerine oturmuştur.

Ancak kamuya açık Kullanım Koşulları belgesinin bulunmaması,
yetkili hukuk ve mahkemenin belirtilmemesi, KVKK'ya atıf
yapılmaması ve bağımsız güvenlik denetiminin gerçekleştirilmemiş
olması ciddi eksikliklerdir. Bu eksiklikler teknik iddiaları
doğrulanamaz kılmaktadır.

**Şu an için:** Kendi sunucusunu kuran kurumsal kullanıcılar için
değerlendirilmeye değer. Bireysel kullanımda ve hassas senaryolarda
belgesel eksiklikler giderilene kadar ihtiyatlı yaklaşım önerilir.

---

## Kaynaklar

| Belge | Kaynak | Erişim Tarihi |
|---|---|---|
| Gizlilik Politikası | Uygulama içi (kullanıcı tarafından temin edildi) | 23.04.2026 |
| Kullanım Koşulları | **Kamuya açık belge bulunamadı** | 23.04.2026 |
| Play Store | https://play.google.com/store/apps/details?id=im.next.app | 23.04.2026 |
| App Store | https://apps.apple.com/tr/app/next-messenger/id6744114179 | 23.04.2026 |
| Euronews Teknik Analiz | https://tr.euronews.com/next/2025/07/31/ovgu-elestiri-ve-tartismalar-10-soruda-next-sosyal-ve-next-mesajlasma | 23.04.2026 |
