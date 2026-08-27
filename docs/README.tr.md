<h1 align="center">Skills AI</h1>
<p align="center">Yapay zeka araçlarının ve onları işinizde daha iyi yapan becerilerin rehberi — çevrimdışı, sekiz dilde.</p>
<p align="center">[English](../README.md) · [فارسی](README.fa.md) · [العربية](README.ar.md) · **Türkçe** · [हिन्दी](README.hi.md) · [Español](README.es.md) · [Deutsch](README.de.md) · [Français](README.fr.md)</p>



<p align="center">
  <img src="../docs/screenshots/01-home.png" width="22%" alt="">
  <img src="../docs/screenshots/02-profile.png" width="22%" alt="">
  <img src="../docs/screenshots/03-community.png" width="22%" alt="">
  <img src="../docs/screenshots/04-account.png" width="22%" alt="">
</p>


## Nedir

Her yapay zeka aracı, nasıl yapacağını söylediğinizde daha iyi yanıt verir. Claude'un sürekli özür dilemesini kesen bir istem, Cursor'u kendi kurallarınızın içinde tutan bir kural, Gemini'ye anadili konuşanın gerçekten yazacağı metni yazdıran bir sistem mesajı — bunlar var, yüzlerce depoya dağılmış hâlde, ve ihtiyaç anında doğrusunu bulmak işin tamamı.

Skills AI bunlardan **102 araç için 5,402 tanesini** topluyor, 12 kategoriye ayırıyor ve bir aramalık mesafeye koyuyor. Katalogun tamamı uygulamanın içinde: trende, tünelde, uçakta, sinyalsiz ve hesapsız açılır.

## Ne yapar

### Bağlantı olmadan çalışır

Katalogun tamamı — 5,402 beceri, tam metinleri ve arama dizini — uygulamanın içinde 17 MB’lık bir SQLite veritabanı olarak gelir. Okumak için hiçbir şey indirilmez.

### Yazdığınız dili anlayan arama

Her başlık ve metin üzerinde tam metin arama; Farsça ve Arapça birlikte katlanır: Arapça ye ile yazılan bir sorgu, Farsça ye ile yazılmış metni bulur ve üç rakam kümesi tek sayılır.

### Kopyalayın, yeniden yazmayın

Her beceri kendi tam metnini, ait olduğu araç için kurulum yordamını ve her parçada bir kopyalama düğmesini taşır.

### Gerçekten işe yaradı mı?

Bir beceriyi kullandıktan sonraki tek dokunuş, kullandığınız model için işe yaradı mı, kısmen mi, yoksa yaramadı mı söyler. Beceriler buna göre sıralanır ve kişi başına sayılır; daha sık yanıtlamak hiçbir şeyi değiştirmez.

### Skor tablosu olmayan bir topluluk

Kendi becerilerinizi yayımlayın, işi size sürekli yarayan kişileri takip edin ve becerinin kendi sayfasında hangilerinin denediğini görün. Herkese açık takipçi sıralaması yok, grafiği listeleyen bir uç nokta da yok.

### Sekiz dil, dördü sağdan sola

İngilizce, Farsça, Arapça, Türkçe, Hintçe, İspanyolca, Almanca ve Fransızca — arayüz, rakamlar, tarihler ve yerleşim yönü.

## İndir

Telefonunuza uygun APK dosyasını [son sürümden](https://github.com/ehsanking/Skills-Ai/releases/latest) indirin. Son yılların çoğu telefonu **arm64-v8a** ister; daha eski veya uygun fiyatlı olanlar **armeabi-v7a**. `x86_64` emülatörler içindir.

Yanlışını kurarsanız Android reddeder — bozuk bir şey kurmaz.

## Nasıl yapıldı

| | |
|---|---|
| **Platform** | Android 8.0 and newer |
| **Framework** | Flutter 3.44 / Dart 3.12 |
| **Catalogue** | SQLite + FTS4, bodies compressed with zlib, 17 MB inside the APK |
| **Backend** | Laravel 13 + Filament 5, at [ai.ehsanking.ir](https://ai.ehsanking.ir) |
| **Package** | `gfly.skillsai.app` |
| **Tools / skills** | 102 / 5,402 |

## Gizlilik

Katalog hesapsız ve ağsız çalışır. Reklam kimliği yok, cihaz kimliği yok, analitik SDK yok. Hesap yalnızca topluluk için gerekir — paylaşmak, kendi becerinizi yayımlamak veya bir becerinin işe yarayıp yaramadığını söylemek için — ve o zaman bile uygulama sizin yazmadığınız hiçbir şeyi toplamaz. Tam metin uygulamada Ayarlar altında ve [web sitesinde](https://ai.ehsanking.ir/pp).

## Destek

Uygulamadaki her şey ücretsiz — her beceri, topluluk, arama ve çevrimdışı kopya — ücretli bir katman, abonelik ya da hesap ardına saklanmış bir şey yok. Onu ayakta tutan reklam ve bağışlar; ikisi de aynı yere gidiyor: sunucular, depolama, bant genişliği ve daha iyisini yapma emeği.

**Reklam verin** — uygulamada iki sponsorlu alan var. Ayrıntılar [Reklam ve Destek sayfasında](https://ai.ehsanking.ir/advertise).

**Bağış** — TRON ağında USDT (TRC-20):

```
TKPswLQqd2e73UTGJ5prxVXBVo7MTsWedU
```

> USDT · TRC-20 (TRON). Sending any other coin or using any other network will lose it.

## Lisans

Uygulama tescillidir — bkz. [LICENSE](../LICENSE). Burada yayımlanan sürümleri serbestçe kurup kullanabilirsiniz; yeniden yayımlayamaz veya satamazsınız.

**Katalog öyle değil.** İçindeki her beceri onu yazana aittir ve onun seçtiği lisansla dağıtılır — CC0-1.0, MIT, Apache-2.0 veya CC-BY-4.0. 33 kaynağın tamamı [THIRD-PARTY-NOTICES.md](../THIRD-PARTY-NOTICES.md) içinde adlandırılmıştır ve aynı bildirimler uygulamayla birlikte gelir. Hiçbir lisansı olmayan beceri dahil edilmedi, çünkü lisans yoksa izin de yoktur.

## Geliştirici

**Ehsan King** — [github.com/ehsanking](https://github.com/ehsanking)


