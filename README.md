<p align="center">
  <a href="https://hitbot.org"><strong>HitBot</strong></a> — Gerçek tarayıcıyla çalışan SEO &amp; organik hit otomasyonu
</p>

<p align="center">
  <a href="https://github.com/erdemsoftware/hitbot-releases/releases/latest"><img alt="Son sürüm" src="https://img.shields.io/github/v/release/erdemsoftware/hitbot-releases?label=son%20s%C3%BCr%C3%BCm"></a>
  <img alt="Platform" src="https://img.shields.io/badge/platform-Windows%2010%2F11%20%7C%20Server-blue">
  <a href="https://hitbot.org"><img alt="Web" src="https://img.shields.io/badge/web-hitbot.org-7367f0"></a>
</p>

---

## HitBot nedir?

**HitBot**, sitenize arama motorlarından gerçek bir kullanıcı gibi ziyaret gönderen bir **Windows masaüstü uygulamasıdır**.
Her ziyaret gerçek bir **Chrome tarayıcısında** açılır: anahtar kelime arama kutusuna insan gibi yazılır, sonuçlarda siteniz
bulunup tıklanır, sitede kaydırma ve sayfa gezintisi yapılır. Bu sayede ziyaretler Google Search Console ve Google Analytics'te
**organik arama trafiği** olarak görünür.

Lisans, proxy ve cookie paketleri **[hitbot.org](https://hitbot.org)** üzerinden satın alınır; uygulama lisansınızla
hesabınıza bağlanır, satın aldığınız kaynakları otomatik olarak çeker.

> Bu depo yalnızca **derlenmiş kurulum dosyalarını** barındırır. Kaynak kod bu depoda **bulunmaz**.

## İndirme

| | |
|---|---|
| **En güncel sürüm** | [Releases → Latest](https://github.com/erdemsoftware/hitbot-releases/releases/latest) |
| **Doğrudan indirme** | [`HitBot-Setup.exe`](https://github.com/erdemsoftware/hitbot-releases/releases/latest/download/HitBot-Setup.exe) |
| **Lisans / paket satın alma** | [hitbot.org](https://hitbot.org) |

## Neler yapabilir?

### Gerçek tarayıcı, gerçek kullanıcı davranışı
- **Gerçek Chrome ile çalışır** — ziyaretler görünür (veya isteğe bağlı arka plan/headless) tarayıcı pencerelerinde yapılır.
- **Cloudflare otomatik geçiş** — Turnstile / "Checking your browser" doğrulamaları otomatik geçilir.
- **Oturum başına benzersiz tarayıcı kimliği** — Canvas, WebGL, Audio gibi parmak izleri her oturumda değişir; otomasyon izleri gizlenir.
- **WebRTC IP sızıntı koruması** ve proxy ülkesine göre **saat dilimi, dil ve konum eşleme**.
- **İnsan gibi etkileşim** — arama kutusuna yazım hataları ve düşünme molalarıyla yazma, eğrisel fare hareketi, gerçek (native) tıklama, kaydırma derinliği, ayarlanabilir sayfada kalma süresi.

### Arama ve trafik
- **Google, Bing, Yandex ve DuckDuckGo** desteği.
- **Anahtar kelime bazlı kampanyalar** — tam kelime veya `site:` hedefli arama; sitenizi sonuçlarda bulup tıklar.
- **Site içi akıllı gezinme** — menü, içerik ve ilgili sayfalar arasında doğal gezinti.
- **Masaüstü / mobil cihaz karışımı** — Search Console "Cihaz" raporuna yansıyacak oranı siz belirlersiniz.
- **Trafik kaynağı karışımı** (organik, doğrudan, sosyal) ve **geri gelen ziyaretçi** simülasyonu.
- **Gün içine dağıtım** — ziyaretleri saatlere yayan planlama seçenekleri.

### Proxy ve cookie yönetimi
- **HTTP, SOCKS4, SOCKS5** — kullanıcı adı/şifreli proxy, IPv4 ve IPv6 desteği.
- **HitBot'a özel proxy'ler** — hitbot.org'dan aldığınız proxy'ler uygulamada otomatik görünür,
  **kalan kota ve bitiş tarihi** uygulama içinden sorgulanır.
- **Proxy seçip aktif etme** — hangi proxy'lerin kullanılacağını tek tek seçin; kendi proxy'lerinizi de ekleyebilirsiniz.
- **Toplu proxy testi**, çevrimiçi/çevrimdışı filtreleme ve başarı oranı takibi.
- **Cookie yönetimi** — dosya/klasörden yükleme veya panelden satın alınan cookie'leri otomatik çekme.
- **Bant genişliği tasarrufu** — görsel/font engelleme ile proxy kotası daha uzun gider.

### Uygulama
- **Çoklu worker** — aynı anda birden fazla izole tarayıcı oturumu.
- **Genel bakış paneli** — canlı hit sayısı, başarı oranı, çalışma süresi ve hazırlık durumu.
- **Türkçe / İngilizce** arayüz, **açık / koyu / sistem** teması.
- **Otomatik güncelleme** — yeni sürüm çıktığında uygulama içinden haber verir.
- **Kullanım raporları** — gönderilen hitler hem uygulama içindeki **Hit Raporları**'nda hem de hitbot.org müşteri panelinizde raporlanır.

## Sistem gereksinimleri

- Windows 10 / 11 veya Windows Server (64-bit)
- Önerilen: 4 GB+ RAM — çok sayıda eşzamanlı worker için daha fazlası

## Kurulum ve ilk çalıştırma

1. [hitbot.org](https://hitbot.org) üzerinden bir lisans paketi satın alın. Lisans anahtarınız hesabınıza tanımlanır.
2. [`HitBot-Setup.exe`](https://github.com/erdemsoftware/hitbot-releases/releases/latest/download/HitBot-Setup.exe) dosyasını indirip çalıştırın.
3. Uygulama açıldığında lisans anahtarınızı girin. Lisans bu bilgisayara bağlanır.
4. **Veri Yönetimi** bölümünden anahtar kelimelerinizi ekleyin; proxy ve cookie paketleriniz panelden otomatik gelir.
5. **Bot Kontrolü**'nden ayarlarınızı yapıp başlatın.

## Otomatik güncelleme

Uygulama her açılışta bu depodaki son sürümü kontrol eder ve yeni bir sürüm varsa bildirir.
**İndirme, kullanıcı onayı olmadan başlamaz.** Güncelleme indirildikten sonra uygulama yeniden başlatılarak kurulur.

## Sürüm geçmişi

### v1.2.0
- **Eşzamanlı tarayıcı hatası düzeltildi:** aynı anda çalışan tarayıcılar artık birbirinin anahtar kelimesini, cihaz profilini ve ülke/dil ayarlarını karıştırmıyor.
- Captcha, proxy ve sayfa hatasıyla biten denemeler de hitbot.org raporlarına iletiliyor; başarılı/başarısız sayıları panelde eksiksiz.
- "Thread Sayısı" ayarının adı **Eşzamanlı Tarayıcı Sayısı** oldu; loglarda her satır hangi tarayıcıdan geldiğini gösteriyor.

Ayrıntılı değişiklik listesi: [v1.2.0 sürüm notları](https://github.com/erdemsoftware/hitbot-releases/releases/tag/v1.2.0)

### v1.1.0
**Öne çıkanlar**
- **HitBot'a özel proxy'ler:** satın aldığınız proxy'ler hesabınıza tanımlandığı anda uygulamada otomatik görünür, sipariş koduyla adlandırılır; kalan kota ve bitiş tarihi uygulamadan sorgulanır.
- **Proxy seçip aktif etme:** her proxy için aktif/pasif anahtarı, "yalnızca bunu kullan", tümünü aktif/pasif et — kendi eklediğiniz proxy'ler dahil.
- **Otomatik ülke eşleştirme:** tarayıcının dili, saat dilimi ve konumu proxy'nin ülkesine göre otomatik ayarlanır.
- **Daha doğal ziyaretler:** arama sonuçlarında gezinme, otomatik tamamlama ve yazım hatası, "en az / en çok" sitede kalma süresi, isteğe bağlı trafik kaynağı karışımı, geri gelen ziyaretçi ve tarayıcı ısıtma.
- **Captcha alan proxy dinlendirme** ve Hit Raporları'nda proxy bazında captcha takibi.
- **Cookie oturum kontrolü:** hangi cookie dosyasının kullanıldığı görünür; oturumu kapanmış dosya atlanır.
- Ayar yedekleme (dışa/içe aktarma), tema uyumlu uyarı pencereleri, güçlendirilmiş lisans doğrulaması ve çok sayıda düzeltme.

Ayrıntılı değişiklik listesi: [v1.1.0 sürüm notları](https://github.com/erdemsoftware/hitbot-releases/releases/tag/v1.1.0)

### v1.0.0
- HitBot'un ilk sürümü yayına alındı: anahtar kelime bazlı organik hit, proxy ve cookie yönetimi, hitbot.org lisans ve panel entegrasyonu.

Tüm sürümler: [Releases](https://github.com/erdemsoftware/hitbot-releases/releases)

## Destek

- Web: [hitbot.org](https://hitbot.org)
- Nasıl çalışır: [hitbot.org/nasil-calisir](https://hitbot.org/nasil-calisir)
- Sık sorulan sorular: [hitbot.org/sikca-sorulan-sorular](https://hitbot.org/sikca-sorulan-sorular)
- İletişim: [hitbot.org/iletisim](https://hitbot.org/iletisim) — ya da müşteri panelinizden destek talebi açın.

---

© HitBot.org — Tüm hakları saklıdır.
