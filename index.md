# Ucuza Bul – Gizlilik Politikası

**Sürüm:** 1.23.0 · **Son güncelleme:** 14 Ekim 2026
**Geliştirici / Veri sorumlusu:** Burak
**İletişim:** · ucuzlamis.com

Bu politika, "Ucuza Bul – Fiyat Karşılaştırma ve En Ucuz Fiyat Bulucu" Chrome eklentisinin (bundan sonra "Eklenti") hangi verileri işlediğini, nerede sakladığını ve kimlerle paylaştığını açıklar. Eklentinin kodu ile bu metin birebir uyumludur; kodda olmayan bir veri toplama yapılmaz.

## 1. Kısaca

- Eklentinin **kendi sunucusu yoktur**. Hesap, e-posta, şifre veya ödeme bilgisi istemez, toplamaz.
- Geçmiş, favoriler, fiyat takibi, ayarlar gibi verileriniz **yalnızca tarayıcınızda** (`chrome.storage.local`) saklanır.
- Aradığınız ürünün adı, ürün bağlantıları ve arama metniniz **bize gönderilmez**; yalnızca fiyat karşılaştırması için ilgili alışveriş sitelerine (aşağıda listelenmiştir) istek olarak gider.
- Eklenti, kullanım istatistiği için **Google Analytics 4**'e yalnızca toplu/teknik bilgi gönderir (Madde 4).
- Verileriniz **satılmaz**, reklam profili çıkarmak için kullanılmaz.
- Ürün bağlantıları **satış ortaklığı (affiliate)** parametresi içerebilir (Madde 6).

## 2. Eklentinin yaptığı işler ve işlenen veriler

**2.1. Ürün sayfasında "UCUZA BUL" butonu.** Trendyol, Hepsiburada, N11 ve Amazon TR ürün sayfalarında eklenti, sayfadaki ürün adı, fiyat, görsel ve bağlantıyı okur. Bu bilgi tarayıcı içinde işlenir ve karşılaştırma için kullanılır.

**2.2. Fiyat karşılaştırma ve serbest arama.** Ürün adından üretilen arama sorguları, eklentinin arka plan servisi tarafından şu sitelere HTTPS isteği olarak gönderilir: Trendyol, Amazon TR, Hepsiburada, N11, PttAVM, Pazarama, idefix, Motorossa, Teknosa. Dönen sayfa tarayıcıda ayrıştırılır; eşleşme ve fiyat hesabı cihazınızda yapılır. Bu istekler tarayıcınızdaki oturum çerezleriyle (`credentials: include`) gönderilir; yani bu sitelerde hesabınız açıksa site isteği hesabınızla ilişkilendirebilir. Eklenti çerezleri okumaz ve saklamaz (çerez izni yoktur). İstekler ilgili sitenin kendi gizlilik politikasına tabidir.

**2.3. Geçmiş ve fiyat geçmişi.** Yaptığınız karşılaştırmalar (ürün adı, fiyatlar, site adları, bağlantılar; en çok 60 kayıt) ve gördüğünüz ürünlerin fiyat değişim noktaları yalnızca cihazınızda saklanır. Popup'tan tek tek ya da toptan silebilirsiniz.

**2.4. Favoriler ve fiyat alarmı.** Hepsiburada, Trendyol, N11 ve Amazon TR'deki favori/istek listesi sayfasını **siz açtığınızda**, eklenti sayfadaki ürün kartlarını (ad, fiyat, görsel, bağlantı) okuyup yerel olarak kaydeder. Trendyol için eklenti, oturumunuzla favori sayfasını arka planda da okuyabilir. Fiyat alarmı için favori ve alarmı açık ürünlerin sayfaları periyodik olarak (en çok saatlik, ürün başına en az birkaç saatte bir) yeniden okunur. Bir ürünü kendiniz favoriye ekleyip çıkarabilirsiniz.

**2.5. Üyelik durumu (Amazon Prime, Trendyol Plus, Hepsiburada Premium).** Doğru fiyatı göstermek için eklenti, bu siteleri açtığınızda sayfa başlığındaki üyelik işaretini okur; ayrıca bu sitelerin ilgili sayfalarını oturum çerezlerinizle (`credentials: include`) arka planda okuyarak üye olup olmadığınızı **yalnızca "evet / hayır" olarak** yerel olarak kaydeder. Sayfanın diğer içeriği saklanmaz. Popup > Ayarlar > Aboneliklerim bölümünden bu değeri elle değiştirebilirsiniz. N11 için otomatik tespit yoktur.

**2.6. "Sana Özel" öneriler ve kampanya bannerları.** Amazon TR (size özel öneriler ve fırsatlar), Trendyol (önceden gezdikleriniz / sana özel), Hepsiburada ("son gezdiğin ürünler") ve N11 sayfaları oturum çerezlerinizle okunarak popup'taki öneri alanı; Hepsiburada, N11 ve Amazon TR ana/kampanya sayfaları okunarak reklam/kampanya alanı doldurulur. Bu içerik yalnızca cihazınızdaki önbellekte tutulur, bize gönderilmez.

**2.7. Bildirimler.** Fiyat alarmı açıksa fiyat düşüşü simge üzerinde bir nokta, sayfa içi küçük bir kart ve (ayarınız açıksa) Windows/işletim sistemi bildirimi olarak gösterilir. Bildirim ayarları Popup > Ayarlar > Bildirim Ayarları'ndadır. Bildirimler cihazınızda üretilir.

**2.8. Onboarding.** İlk kullanımdaki kısa tur yalnızca "gösterildi" bilgisini yerel olarak saklar.

## 3. Cihazınızda saklanan veriler

`chrome.storage.local` içinde: karşılaştırma önbelleği (en çok birkaç saat), karşılaştırma geçmişi, ürün fiyat geçmişi, favoriler ve kaldırdığınız favoriler, alarm tercihleri, bildirim ayarları, üyelik durumu (evet/hayır), öneri ve banner önbelleği, görülen öneriler, onboarding durumu, rastgele analitik kimliği ve oturum bilgisi. Bu veriler Google hesabınızla senkronize edilmez; eklentiyi kaldırdığınızda silinir. `localStorage` içinde yalnızca Trendyol Plus bilgisinin yerel kopyası tutulabilir.

## 4. Kullanım istatistikleri (Google Analytics 4)

Eklentiyi geliştirmek için GA4 Measurement Protocol ile anonim kullanım olayları gönderilir. Uzak betik yüklenmez; olaylar HTTPS isteğiyle `www.google-analytics.com` adresine iletilir.

**Gönderilenler:** rastgele üretilmiş istemci kimliği (Google hesabınızla ilişkisi yoktur) ve oturum numarası; eklenti sürümü; tarayıcı dili; üyelik durumu (Amazon Prime / Trendyol Plus için evet-hayır-bilinmiyor); olay adları ve toplu bilgiler: kaynak site adı, eşleşme sayıları, "daha ucuz bulundu mu", en ucuz sitenin adı, geniş fiyat aralığı (örn. "500-2000"), yuvarlanmış tahmini tasarruf (TL ve %), yanıt vermeyen site sayısı, süre (ms), butonun gösterilmesi/üzerine gelinmesi, popup sekme görüntüleme, ortaklık bağlantısına tıklama, paylaş düğmesi kullanımı, ayar değişikliği (hangi ayar, açık/kapalı), onboarding adımları, kurulum/güncelleme.

**Gönderilmeyenler:** ürün başlığı, arama metni, ürün veya sayfa adresleri (URL), favori ve geçmiş içeriği, hesap/kimlik/şifre/çerez bilgisi.

Google, isteğin doğası gereği IP adresinizi alır ve yaklaşık konum çıkarımı yapabilir; bu işleme Google'ın politikası uygulanır (https://policies.google.com/privacy). GA4 veri saklama süresi: [14 ay – GA4 ayarınıza göre güncelleyin]. Analitik gönderimi şu an Eklenti içinde kapatılamaz; durdurmak için Eklentiyi kaldırabilirsiniz.

## 5. Üçüncü taraflara yapılan istekler

| Alıcı | Neden | Ne gider |
|---|---|---|
| Trendyol, Amazon TR, Hepsiburada, N11, PttAVM, Pazarama, idefix, Motorossa, Teknosa | Fiyat/arama/öneri/üyelik/favori okuma | Arama sorgusu ve sayfa isteği; tarayıcı oturum çerezleriniz de ilgili siteye gider (eklenti çerezleri okumaz) |
| Google Analytics (google-analytics.com) | Kullanım istatistiği | Madde 4'teki toplu bilgiler |
| Google Fonts (fonts.googleapis.com) | Popup yazı tipi | Standart HTTP isteği (IP adresi, tarayıcı bilgisi) |
| mzstatic.com (Apple CDN), cdn.myikas.com ve ürün görseli sunan mağaza CDN'leri | Mağaza logoları ve ürün görselleri | Standart görsel isteği |

Eklenti uzaktan çalıştırılabilir kod indirmez; tüm kod paket içindedir.

## 6. Satış ortaklığı (affiliate) açıklaması

Eklenti ücretsizdir. Gelir modeli satış ortaklığıdır: Eklentinin gösterdiği ürün bağlantıları (karşılaştırma kartları, arama/öneri/reklam kartları, popup'taki "Ürüne git", QR kod ve paylaşım bağlantıları) ve desteklenen mağazaların sayfalarında tıkladığınız ürün bağlantıları, ortaklık ve/veya `utm_` izleme parametresi içerebilir. Bu bağlantılar üzerinden alışveriş yaparsanız mağazalardan komisyon alabiliriz; **ödediğiniz fiyat değişmez**. Eklenti çerez enjekte etmez, kupon uygulamaz. Bu açıklama Chrome Web Store sayfasında ve Eklenti arayüzünde (Ayarlar) de yer alır.

## 7. İzinlerin kullanım amacı

- **storage:** geçmiş, favori, ayar ve önbelleğin yerel saklanması.
- **alarms:** favori fiyat kontrolü, öneri ve üyelik yenilemesi için zamanlayıcı.
- **offscreen:** arama sonucu HTML'ini görünmez bir belgede ayrıştırmak (servis çalışanında DOM yoktur).
- **notifications:** fiyat düşüşünü bildirmek.
- **activeTab:** popup'tan açık ürün sayfasını okumak/karşılaştırmayı başlatmak.
- **Site izinleri (host):** yalnızca yukarıdaki alışveriş siteleri ve Google Analytics. Eklenti başka sitelerde çalışmaz.

## 8. Saklama, silme ve kontrol

Yerel verilerinizi Popup > Geçmiş'ten silebilir, favorileri/alarmları kaldırabilir, tüm verileri `chrome://extensions` üzerinden eklentiyi kaldırarak silebilirsiniz. Bildirimleri Ayarlar'dan kapatabilirsiniz. Analitik verisi Google'da yukarıdaki sürede tutulur; istemci kimliği yerel olduğundan eklentiyi kaldırdığınızda yeni bir kimlik oluşmaz ve eski kayıtla ilişki kurulamaz.

## 9. Çocuklar

Eklenti 13 yaşın altındaki çocuklara yönelik değildir ve bilerek onların verisini toplamaz.

## 10. KVKK ve haklarınız

Türkiye'deki kullanıcılar için 6698 sayılı KVKK kapsamında veri sorumlusu yukarıda belirtilen geliştiricidir. Analitik verisi, hizmetin geliştirilmesi (meşru menfaat) amacıyla ve kimliğinizi belirlemeyecek biçimde işlenir. KVKK m.11 uyarınca verilerinize erişme, düzeltme, silme, işlemeye itiraz etme haklarınız vardır; başvuru için [E-POSTA ADRESİ] adresine yazabilirsiniz. Veriler Google'ın altyapısı nedeniyle yurt dışına aktarılabilir.

## 11. Değişiklikler

Politika değiştiğinde bu sayfa ve Eklenti sürüm notları güncellenir. Önemli değişikliklerde Chrome Web Store sayfası da güncellenir.

---

# Ucuza Bul – Privacy Policy (English summary)

**Version 1.23.0 · Last updated: 14 Oct 2026 · Contact: [E-MAIL]**

Ucuza Bul has **no backend of its own**, requires no account and collects no email, password or payment data. History, favorites, price tracking and settings stay **locally in your browser** (`chrome.storage.local`). Product titles, search text and URLs are **never sent to us**; they are only used to query the supported shopping sites (Trendyol, Amazon TR, Hepsiburada, N11, PttAVM, Pazarama, idefix, Motorossa, Teknosa) for price comparison, and matching runs on your device.

**Requests to shopping sites** are sent with your browser session cookies (`credentials: include`), so a site where you are logged in may associate them with your account; the extension itself never reads or stores cookies. **Pages read:** product pages of Trendyol, Hepsiburada, N11 and Amazon TR; the wishlist pages of these sites when you open them; membership indicators (Amazon Prime, Trendyol Plus, Hepsiburada Premium) which are stored locally only as yes/no.

**Analytics:** anonymous usage events are sent via Google Analytics 4 Measurement Protocol (random client ID not linked to your Google account, extension version, browser language, membership yes/no, site names, counts, coarse price bucket, rounded estimated savings, setting toggles). No product titles, search text, URLs, favorites/history content or credentials are sent. Google receives your IP address as part of the request. Analytics cannot currently be switched off inside the extension; uninstall to stop it.

**Other requests:** Google Fonts (popup typeface) and image CDNs (store logos, product images).

**Affiliate disclosure:** product links shown by the extension and product links you click on supported stores may carry an affiliate and/or UTM parameter. We may earn a commission on purchases; the price you pay does not change. The extension does not inject cookies or apply coupons.

**Remote code:** none. **Data sale:** none. **Deletion:** clear history inside the popup or uninstall the extension. **Contact:** [E-MAIL].
