# Ucuza Bul – Gizlilik Politikası

**Son güncelleme:** 19 Ekim 2026 · **Sürüm:** 1.27.0
**Yayıncı / Veri sorumlusu:** Burak · **İletişim:** burakyavastc@gmail.com

Ucuza Bul ("Eklenti"), bir ürünü desteklenen alışveriş sitelerinde karşılaştıran, fiyat geçmişi ve fiyat alarmı sunan bir Chrome eklentisidir. Bu politika, Eklenti'nin hangi verilere eriştiğini, nerede sakladığını ve kimlerle paylaştığını açıklar.

## 1. Kısaca
- Eklentinin kullanıcı verisi tutan **kendi sunucusu yoktur.** Geçmiş, favoriler, fiyat geçmişi, harcama özeti ve ayarlar **yalnızca tarayıcınızda** (`chrome.storage.local`) durur; Eklenti kaldırıldığında silinir.
- Ürün başlığı, arama metni, ürün adresi (URL), e-posta, ad, adres, telefon, parola ve ödeme bilgisi **toplanmaz, analitiğe gönderilmez, satılmaz.**
- Anonim kullanım istatistiği için Google Analytics 4 kullanılır (bölüm 4).
- Ürün bağlantılarına ortaklık (affiliate) ve UTM parametreleri eklenir; bu bağlantılardan alışveriş yaparsanız yayıncı komisyon alabilir, sizin ödediğiniz fiyat değişmez (bölüm 5).

## 2. Eklentinin eriştiği veriler ve amaçları
| Veri | Ne için | Nerede durur |
|---|---|---|
| Baktığınız ürün sayfasındaki ürün başlığı, fiyat, satıcı/marka bilgisi | Aynı ürünü diğer sitelerde aramak ve fiyat karşılaştırmak | Anlık işlenir; karşılaştırma sonucu önbellekte (en çok 6 saat) ve Geçmiş'te tutulur |
| Popup'a yazdığınız arama metni | Desteklenen sitelerde arama yapmak | Yalnızca ilgili sitelere istek olarak gider; Geçmiş'te yerel tutulur |
| Karşılaştırma geçmişi (en çok 60 kayıt) | Geçmiş ekranı, kazanç özeti | Yerel |
| Favoriler (site favori/istek/alışveriş listelerinizdeki ürünler: başlık, fiyat, görsel, bağlantı) ve fiyat geçmişi | Favori listesi, fiyat takibi, fiyat düşüş uyarısı | Yerel |
| Fiyat alarmı seçimleriniz, bildirim ayarları | Düşüş bildirimi göndermek | Yerel |
| Sipariş özeti (Trendyol, Hepsiburada, N11 ve Amazon TR hesabınızdaki siparişlerden yalnızca **toplam tutar, sipariş/ürün adedi, iptal bilgisi, ay/yıl dağılımı**) | "Toplam Harcaman" ekranı ve paylaşım görseli | Yerel. Tek tek sipariş, ürün adı, alıcı adı, adres **saklanmaz**. İlgili site için özelliği Profil'den kapatabilirsiniz |
| Abonelik durumu (Trendyol Plus, Hepsiburada Premium, Amazon Prime: üye/değil) | Üyelik fiyatlarının doğru değerlendirilmesi, üyelik fiyatının karışmaması | Yerel |
| Ayarlar (QR kartı, otomatik kupon, kupon hatırlatıcısı, tanıtım turu durumu vb.) | Tercihlerinizi hatırlamak | Yerel |

Siparişler, favoriler ve abonelik bilgileri; tarayıcınızda açık olan **kendi oturumunuz** üzerinden ilgili sitenin kendi sayfa/arayüz uçlarından okunur. Eklenti giriş bilgilerinizi (kullanıcı adı, parola, çerez içeriği) okumaz, kaydetmez ve göndermez. Harcama hesabı için ilgili sitede arka planda sessiz bir sekme açılabilir; iş bitince kapanır.

## 3. Ağ istekleri
Eklenti şu adreslere istek yapar:
- Alışveriş siteleri (Trendyol, Hepsiburada, N11, Amazon TR, PttAVM, Pazarama, idefix, Motorossa, Teknosa): arama sayfaları, favori/sipariş/üyelik bilgisi uçları. İstekler **sizin tarayıcınızdan ve IP adresinizden** gider; ilgili siteler bu istekleri kendi gizlilik politikalarına göre görür.
- Google Analytics (`www.google-analytics.com`): anonim istatistik (bölüm 4).
- `i.motorossa.com.tr`: yalnızca **veri** içeren bir yapılandırma dosyası (ortaklık/UTM parametreleri). İstek, kişisel veri içermez; bu sunucu sizin IP adresinizi standart sunucu kaydı olarak görebilir.
- Arayüzdeki bazı site logoları üçüncü taraf görsel sunucularından (ör. Apple `mzstatic.com`, `cdn.myikas.com`) yüklenir; bu sunucular görsel isteğiyle IP adresinizi görür.

Eklenti **uzaktan kod indirmez ve çalıştırmaz**; uzaktan alınan dosya yalnızca doğrulanan bir veri (JSON) dosyasıdır.

## 4. Anonim kullanım analitiği (Google Analytics 4)
Eklenti, Google Analytics 4 Measurement Protocol ile aşağıdaki **anonim** bilgileri gönderir:
- Rastgele üretilmiş istemci kimliği (Google hesabınızla ilişkisi yoktur) ve oturum kimliği.
- Olay adları ve teknik sayılar: eklenti kurulumu/güncellemesi, popup bölümü görüntüleme, karşılaştırma tamamlandı (eşleşme sayısı, en ucuz site adı, tasarruf tutarı ve yüzdesi, **geniş fiyat aralığı** örn. "2000-10000"), buton/tur/QR/paylaşım/ayar etkileşimleri.
- Kullanıcı özellikleri: Plus/Premium/Prime üyelik durumu (evet/hayır/bilinmiyor), toplam harcamanın **geniş aralığı** (örn. "10000-50000") ve en çok harcama yapılan site adı (**kesin tutar gönderilmez**), eklentiyi kullanma gün sayısı, eklenti sürümü.
- Cihaz bilgisi: tarayıcı adı/sürümü, işletim sistemi, tarayıcı dili, saat dilimi (yalnızca bölge adı).
- Google Analytics, isteğin IP adresinden yaklaşık konumu (ülke/bölge/şehir) kendiliğinden çıkarır; Eklenti konum, adres veya IP göndermez.

**Gönderilmeyenler:** ürün başlığı, arama metni, ürün/sayfa adresi, favori içeriği, kesin harcama tutarı, hesap/kimlik bilgisi.
Analitik verileri Google'ın [gizlilik politikası](https://policies.google.com/privacy) kapsamında işlenir.

## 5. Ortaklık (affiliate) bağlantıları
Eklenti, karşılaştırma sonuçlarındaki, popup'taki ve desteklenen sitelerde gezinirken tıkladığınız **ürün bağlantılarına** ortaklık ve/veya UTM parametreleri ekler (ör. Amazon TR için ortaklık etiketi). Bu bağlantılar üzerinden satın alma yaparsanız yayıncı ilgili mağazadan komisyon kazanabilir; **ödediğiniz fiyat değişmez.** Bir bağlantıda başka bir izleme parametresi varsa değiştirilebilir. Popup > Profil > Ayarlar'dan site içi bağlantı dönüştürmeyi kapatabilirsiniz. Ortaklık parametreleri, mağaza güncellemesi beklemeden değiştirilebilsin diye yukarıda belirtilen veri dosyasından okunur.

## 6. İzinlerin gerekçesi
| İzin | Gerekçe |
|---|---|
| `storage`, `unlimitedStorage` | Geçmiş, favoriler, fiyat geçmişi, önbellek ve ayarların yerel saklanması |
| `alarms` | Favori fiyatlarının ve ortaklık ayarlarının düzenli (arka plan) kontrolü |
| `notifications` | Fiyat düşüşü bildirimi (ayarlardan kapatılabilir) |
| `offscreen` | Arama sayfalarının HTML'ini görünmez bir belgede ayrıştırmak |
| `activeTab`, `contextMenus`, `sidePanel` | Yakında eklenecek özellikler için (bağlam menüsü, yan panel, etkin sekmeye geçici erişim) tanımlıdır; bu sürümde bu izinlerle veri okunmaz veya gönderilmez |
| `tabs` | Açık ürün sayfasını tanımak, harcama/favori okuması için sessiz sekme açıp kapatmak |
| Site erişimleri (`*.trendyol.com`, `*.hepsiburada.com`, `*.n11.com`, `*.amazon.com.tr`, `*.pttavm.com`, `*.pazarama.com`, `*.idefix.com`, `*.motorossa.com.tr`, `*.teknosa.com`, `www.google-analytics.com`) | Yalnızca karşılaştırma, favori/sipariş/üyelik okuma ve anonim analitik için; başka sitelere erişim istenmez |

## 7. Paylaşım ve satış
Verileriniz üçüncü taraflara **satılmaz**, reklam/profilleme amacıyla kullanılmaz, kredi veya yetkinlik değerlendirmesi için aktarılmaz. Yalnızca bölüm 3–5'te anılan hizmetlere, gerekli olduğu ölçüde veri gider. Eklenti'nin Chrome Web Store Kullanıcı Verileri Politikası'ndaki Sınırlı Kullanım gerekliliklerine uyduğunu beyan ederiz: erişilen veri yalnızca Eklenti'nin kullanıcıya dönük özelliklerini sağlamak için kullanılır.

## 8. Saklama, silme ve haklarınız
- Yerel veriler, siz silene (Geçmiş/Favori silme, Profil ayarları) ya da Eklenti kaldırılana kadar tarayıcınızda durur; önbellek ve eski kayıtlar otomatik budanır.
- Analitik verisi, Google Analytics'in saklama ayarlarına göre tutulur. Anonim istemci kimliği Eklenti kaldırıldığında silinir.
- 6698 sayılı KVKK kapsamında; verilerinize erişme, düzeltme, silme, işleme itirazı ve şikâyet haklarınız için burakyavastc@gmail.com adresine yazabilirsiniz. Yerel veriler cihazınızda olduğundan çoğunu doğrudan kendiniz silebilirsiniz.

## 9. Çocuklar
Eklenti 13 yaş altı çocuklara yönelik değildir ve bilerek çocuklardan veri toplamaz.

## 10. Marka bildirimi
Trendyol, Hepsiburada, N11, Amazon, PttAVM, Pazarama, idefix, Motorossa ve Teknosa ilgili sahiplerinin ticari markalarıdır. Ucuza Bul bu şirketlerle bağlantılı değildir, onlar tarafından onaylanmamıştır veya desteklenmemektedir.

## 11. Değişiklikler
Politika değişirse bu sayfa güncellenir ve "Son güncelleme" tarihi değişir. Önemli değişiklikler Eklenti sürüm notlarında duyurulur.
