<p align="center">
  <img src="../assets/readme/hero.tr.svg" width="100%" alt="Yapay zeka araçlarının ve onları işinizde daha iyi yapan becerilerin rehberi — çevrimdışı, sekiz dilde.">
</p>

<div align="center">

Yapay zeka araçlarının ve onları işinizde daha iyi yapan becerilerin rehberi — çevrimdışı, sekiz dilde.

</div>

<div align="center">

[English](../README.md) · [فارسی](README.fa.md) · [العربية](README.ar.md) · **Türkçe** · [हिन्दी](README.hi.md) · [Español](README.es.md) · [Deutsch](README.de.md) · [Français](README.fr.md)

</div>

## Nasıl göründüğü

<p align="center">
  <img src="screenshots/01-home.png" width="23%" alt="Ana ekran: her yapay zeka aracı, beceri sayısına göre sıralı">
  <img src="screenshots/02-profile.png" width="23%" alt="Bir kişi: yayımladığı beceriler ve başkalarının onlar hakkında söyledikleri">
  <img src="screenshots/03-community.png" width="23%" alt="Topluluk: gönderiler, yanıtlar ve okurların yayımladığı beceriler">
  <img src="screenshots/04-account.png" width="23%" alt="Hesap rafı: giriş, favoriler, dil ve tema">
</p>

## İndir

### Android

| Dosya | Şunun için |
|---|---|
| [`app-arm64-v8a-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/app-arm64-v8a-release.apk) | Çoğu telefon — kabaca son sekiz yılda yapılmış her şey. **Buradan başlayın.** |
| [`app-armeabi-v7a-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/app-armeabi-v7a-release.apk) | Daha eski ya da giriş seviyesi telefonlar, 32 bit. |
| [`app-x86_64-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/app-x86_64-release.apk) | Emülatörler ve birkaç x86 tablet. |

Yanlışını seçerseniz Android bozuk bir şey kurmak yerine kurulumu reddeder — yani önce `arm64-v8a` denemenin bir maliyeti yok.

**İndirdiğinizi doğrulamak**

Buradaki her APK aynı anahtarla imzalıdır ve bir şey kurmadan önce bunu doğrulayabilirsiniz:

```
apksigner verify --print-certs app-arm64-v8a-release.apk
```

Sertifikada `CN=Ehsan King, OU=Skills AI` ve şu SHA-256 parmak izi görünmeli. Bunu göstermeyen bir yapı buradan gelmemiştir.

```
DF:9A:3E:BD:B2:28:06:F4:0F:99:3F:64:0D:46:A2:D2:5A:EA:12:49:53:0F:FF:39:C6:75:C4:BB:4F:66:E1:B4
```

### Windows

| Dosya | Şunun için |
|---|---|
| [`SkillsAI-windows-x64-setup.exe`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/SkillsAI-windows-x64-setup.exe) — 23 MB | **Kurulum.** Kendi kullanıcı klasörünüze kurulur — yönetici izni istemez, hesabınızın dışına hiçbir şey yazmaz. Başlat menüsüne bir kısayol ve düzgün bir kaldırıcı ekler. |
| [`SkillsAI-windows-x64.zip`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/SkillsAI-windows-x64.zip) — 26 MB | **Taşınabilir zip.** Taşınabilir bir yapı. Nereye isterseniz açın ve `SkillsAI.exe` dosyasını çalıştırın — hiçbir şey kurulmaz, kayıt defterine bir şey yazılmaz ve katalog ilk açılışta `%APPDATA%\Skills AI` içine çıkarılır. Windows 10 (1809) ve üzeri, 64 bit. Kaldırmak için klasörü silin. |

<p align="center">
  <img src="screenshots/05-windows.png" width="46%" alt="Windows yapısı: aynı katalog, bir masaüstü penceresinde">
</p>

Windows yayıncıyı tanımadığını söyleyecek. Bu uyarı beklenen bir şey: yapı ücretli bir kod imzalama sertifikasıyla imzalanmadı. Sırf bana güvenip geçmenizi istemek yerine, her iki dosyanın SHA-256 değeri burada — indirdiğinizi karşılaştırın.

```
3fc2f1d3d222c6ba4b548b09884ed6d8dde9f609dc7f9a9394acfad5d45d0be1  SkillsAI-windows-x64-setup.exe
65b07b4d23503a7f613577d421d882a9b5625ea76aa4638d561f039491d644fa  SkillsAI-windows-x64.zip
```

```
certutil -hashfile SkillsAI-windows-x64-setup.exe SHA256
```

### iPhone ve iPad

App Store sürümü yok. Safari’de açıp ana ekranınıza ekleyin: sonrasında kendi simgesiyle tam ekran açılır ve bir uygulama gibi davranır.

[**ai.ehsanking.ir/app**](https://ai.ehsanking.ir/app)

> Açtığınız sayfalar bağlantı olmadan da okunabilir kalır. Bütün katalog çevrimdışı olarak Android ve Windows sürümlerinde bulunur.

## Nedir

Her yapay zeka aracı, nasıl yapacağını söylediğinizde daha iyi yanıt verir. Claude'un sürekli özür dilemesini kesen bir istem, Cursor'u kendi kurallarınızın içinde tutan bir kural, Gemini'ye anadili konuşanın gerçekten yazacağı metni yazdıran bir sistem mesajı — bunlar var, yüzlerce depoya dağılmış hâlde, ve ihtiyaç anında doğrusunu bulmak işin tamamı.

Skills AI bunlardan **102 araç için 5,402 tanesini** topluyor, 12 kategoriye ayırıyor ve bir aramalık mesafeye koyuyor. Katalogun tamamı uygulamanın içinde: trende, tünelde, uçakta, sinyalsiz ve hesapsız açılır.

## Ne yapar

- **Bağlantı olmadan çalışır** — Katalogun tamamı — 5,402 beceri, tam metinleri ve arama dizini — uygulamanın içinde 17 MB’lık bir SQLite veritabanı olarak gelir. Okumak için hiçbir şey indirilmez.
- **Yazdığınız dili anlayan arama** — Her başlık ve metin üzerinde tam metin arama; Farsça ve Arapça birlikte katlanır: Arapça ye ile yazılan bir sorgu, Farsça ye ile yazılmış metni bulur ve üç rakam kümesi tek sayılır.
- **Kopyalayın, yeniden yazmayın** — Her beceri kendi tam metnini, ait olduğu araç için kurulum yordamını ve her parçada bir kopyalama düğmesini taşır.
- **Gerçekten işe yaradı mı?** — Bir beceriyi kullandıktan sonraki tek dokunuş, kullandığınız model için işe yaradı mı, kısmen mi, yoksa yaramadı mı söyler. Beceriler buna göre sıralanır ve kişi başına sayılır; daha sık yanıtlamak hiçbir şeyi değiştirmez.
- **Skor tablosu olmayan bir topluluk** — Kendi becerilerinizi yayımlayın, işi size sürekli yarayan kişileri takip edin ve becerinin kendi sayfasında hangilerinin denediğini görün. Herkese açık takipçi sıralaması yok, grafiği listeleyen bir uç nokta da yok.
- **İsterseniz işinizi satın** — Kataloğun kendisi ücretsizdir ve öyle kalır. Kendi becerilerini, araçlarını ya da eklentilerini yayımlayan herkes onlara fiyat koyabilir: alıcı kripto parayla öder, satıcıya USDT ödenir, platformun payı %12. 1.1.0’dan itibaren satıcı tarafı uygulamanın içinde — bakiyeniz, cüzdanınız, ödemeleriniz ve her ilanın fiyatıyla bir **Kazanç** ekranı. Siz fiyat koymadıkça yayımladığınız hiçbir şey ücretli olmaz.
- **Sekiz dil, dördü sağdan sola** — İngilizce, Farsça, Arapça, Türkçe, Hintçe, İspanyolca, Almanca ve Fransızca — arayüz, rakamlar, tarihler ve yerleşim yönü.

## Kendi işinizi satmak

Uygulamayla gelen her şey ücretsizdir ve öyle kalır. Yanı sıra, kendi işini
yayımlayan herkesin ona bir fiyat koyabildiği bir pazar yeri var.

| | |
|---|---|
| **Size kalan** | Her satışın %88'i |
| **Bize kalan** | %12 ve başka hiçbir şey — listeleme ücreti yok, aylık ücret yok, ödeme ücreti yok |
| **Fiyat** | ABD doları, 1,00 – 999,00, siz belirlersiniz |
| **Alıcı öder** | Kripto parayla, NOWPayments üzerinden |
| **Size ödenir** | USDT, BEP-20 veya TRC-20 üzerinden |
| **En düşük ödeme** | 20,00 dolar |
| **Bekleme** | Bir satışın çekilebilmesi için 14 gün |

Bekleme süresi bir nakit akışı oyunu değil. Satıcı koşulları şunu taahhüt eder:
bir ilan dolandırıcılık çıkarsa, birinin telif hakkını ihlal ederse ya da ciddi
bir hukuki talebin konusu olursa, **para dondurulur, alıcıya iade edilir ve
ticari hesap kapatılır** — ve bu söz yalnızca para hâlâ buradayken tutulabilir.
Bir cüzdana gitmiş USDT gitmiştir.

**Uygulama para kazanır, ama satın almaz.** 1.1.0'dan itibaren satıcı tarafı
uygulamanın içinde bir ekran: ticari hesabı açmak, USDT cüzdanını girmek, dört
farklı şeyi anlatan dört rakam, ödeme talebi ve kendi ilanlarınızı
fiyatlandırmak. Ücretli bir ilanı satın almak tarayıcıda olur; bu bir eksiklik
değil, bir karar: dijital ürünleri bir Android yapısının içinde satmak tam da
Cafe Bazaar ile Myket'in ödeme kurallarının konusudur. Para almak, telefonu
tutan kişinin satın alması değildir.

Ödeme cüzdanının değişmesi, ait olduğu hesaba bildirim gönderir — uygulamada,
web uygulamasında ve e-postayla. Sizin girmediğiniz bir adresi, bir ödeme
kaybolduğunda değil, girildiği anda öğrenirsiniz.

Koşulların tamamı sekiz dilde [sitede](https://ai.ehsanking.ir/terms#seller), ve
her şeyi anlatan bir sayfa da
[ai.ehsanking.ir/earn](https://ai.ehsanking.ir/earn) adresinde.

## Çevrimdışı nasıl kalıyor

<p align="center">
  <img src="../assets/readme/how-it-works.svg" width="100%" alt="Üç adım: bütün katalog indirilen dosyanın içinde gelir, ağ olmadan açılır ve sonraki açılışta doğrulanmış bir güncellemeyle değiştirilir">
</p>

- **İndirilenin içinde** — `skills.db`, 17 MB SQLite: gövdeleri sıkıştırılmış 5,402 beceri, hepsinin üzerinde tam metin dizini ve 33 üçüncü taraf lisans metni tam olarak.
- **İlk açılış** — Paketten bir kez çıkarılır ve salt okunur açılır. Ara, oku, kopyala — ağ yok, hesap yok, kayıt yok.
- **Katalog büyüdüğünde** — Sunucu yeni bir derlem yayımlar. Uygulama indirir, sha256 değerini doğrular ve canlı dosyanın yanına koyar — üzerine değil — sonra bir sonraki açılışta değiştirir.

## Nasıl yapıldı

| | |
|---|---|
| **Android** | 8.0 and newer |
| **Flutter** | 3.44 / Dart 3.12 |
| **Catalogue** | SQLite + FTS4, bodies deflated, 17 MB inside the APK |
| **Backend** | Laravel 13 + Filament 5, [ai.ehsanking.ir](https://ai.ehsanking.ir) |
| **Package** | `gfly.skillsai.app` |
| **Tools / skills** | 102 / 5,402 |

## Gizlilik

Katalog hesapsız ve ağsız çalışır. Reklam kimliği yok, cihaz kimliği yok, analitik SDK yok. Hesap yalnızca topluluk için gerekir — paylaşmak, kendi becerinizi yayımlamak veya bir becerinin işe yarayıp yaramadığını söylemek için — ve o zaman bile uygulama sizin yazmadığınız hiçbir şeyi toplamaz. Tam metin uygulamada Ayarlar altında ve [web sitesinde](https://ai.ehsanking.ir/pp).

## Destek

Uygulamadaki her şey ücretsiz — her beceri, topluluk, arama ve çevrimdışı kopya — ücretli bir katman, abonelik ya da hesap ardına saklanmış bir şey yok. Onu ayakta tutan reklam ve bağışlar; ikisi de aynı yere gidiyor: sunucular, depolama, bant genişliği ve daha iyisini yapma emeği.

**Reklam verin** — uygulamada iki sponsorlu alan var. Ayrıntılar [Reklam ve Destek sayfasında](https://ai.ehsanking.ir/advertise).

**Bağış** — USDT, bu iki ağdan biri üzerinden. BEP-20 genelde daha ucuza gönderilir:

**BEP-20 · BNB Smart Chain**

```
0x53F494E1Fc1Ee777C55B49048dd1ab7e4C5d7244
```

**TRC-20 · TRON**

```
TKPswLQqd2e73UTGJ5prxVXBVo7MTsWedU
```

> Yalnızca USDT ve yalnızca bu iki ağ. Başka bir coin ya da başka bir ağ geri dönmez — sadece kaybolur.

## Lisans

Uygulama tescillidir — bkz. [LICENSE](../LICENSE). Burada yayımlanan sürümleri serbestçe kurup kullanabilirsiniz; yeniden yayımlayamaz veya satamazsınız.

**Katalog öyle değil.** İçindeki her beceri onu yazana aittir ve onun seçtiği lisansla dağıtılır — CC0-1.0, MIT, Apache-2.0 veya CC-BY-4.0. 33 kaynağın tamamı [THIRD-PARTY-NOTICES.md](../THIRD-PARTY-NOTICES.md) içinde adlandırılmıştır ve aynı bildirimler uygulamayla birlikte gelir. Hiçbir lisansı olmayan beceri dahil edilmedi, çünkü lisans yoksa izin de yoktur.

## Geliştirici

**Ehsan King** — [github.com/ehsanking](https://github.com/ehsanking)
