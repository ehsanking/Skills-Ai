<p align="center">
  <img src="../assets/readme/hero.de.svg" width="100%" alt="Ein Verzeichnis von KI-Werkzeugen und den Fähigkeiten, die sie in deiner Arbeit besser machen — offline, in acht Sprachen.">
</p>

<div align="center">

Ein Verzeichnis von KI-Werkzeugen und den Fähigkeiten, die sie in deiner Arbeit besser machen — offline, in acht Sprachen.

</div>

<div align="center">

[English](../README.md) · [فارسی](README.fa.md) · [العربية](README.ar.md) · [Türkçe](README.tr.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · **Deutsch** · [Français](README.fr.md)

</div>

## Wie es aussieht

<p align="center">
  <img src="screenshots/01-home.png" width="23%" alt="Der Startbildschirm: jedes KI-Werkzeug, nach der Zahl seiner Fähigkeiten sortiert">
  <img src="screenshots/02-profile.png" width="23%" alt="Eine Person: die Fähigkeiten, die sie veröffentlicht hat, und was andere dazu sagten">
  <img src="screenshots/03-community.png" width="23%" alt="Die Community: Beiträge, Antworten und von Lesern veröffentlichte Fähigkeiten">
  <img src="screenshots/04-account.png" width="23%" alt="Das Kontoregal: Anmelden, Favoriten, Sprache und Erscheinungsbild">
</p>

## Herunterladen

### Android

| Datei | Für |
|---|---|
| [`app-arm64-v8a-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/app-arm64-v8a-release.apk) | Die meisten Telefone — alles aus etwa den letzten acht Jahren. **Hier anfangen.** |
| [`app-armeabi-v7a-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/app-armeabi-v7a-release.apk) | Ältere oder einfache Telefone, 32 Bit. |
| [`app-x86_64-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/app-x86_64-release.apk) | Emulatoren und die wenigen x86-Tablets. |

Bei der falschen Datei verweigert Android die Installation, statt etwas Kaputtes zu installieren — `arm64-v8a` zuerst zu probieren kostet also nichts.

**Prüfen, was Sie geladen haben**

Jede APK hier ist mit demselben Schlüssel signiert, und Sie können das prüfen, bevor Sie etwas installieren:

```
apksigner verify --print-certs app-arm64-v8a-release.apk
```

Das Zertifikat sollte `CN=Ehsan King, OU=Skills AI` mit diesem SHA-256-Fingerprint zeigen. Ein Build, der ihn nicht zeigt, kommt nicht von hier.

```
DF:9A:3E:BD:B2:28:06:F4:0F:99:3F:64:0D:46:A2:D2:5A:EA:12:49:53:0F:FF:39:C6:75:C4:BB:4F:66:E1:B4
```

### Windows

| Datei | Für |
|---|---|
| [`SkillsAI-windows-x64-setup.exe`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/SkillsAI-windows-x64-setup.exe) — 23 MB | **Installer.** Installiert in Ihren eigenen Benutzerordner — ohne Administratorabfrage und ohne etwas außerhalb Ihres Kontos zu schreiben. Legt einen Startmenü-Eintrag und einen richtigen Uninstaller an. |
| [`SkillsAI-windows-x64.zip`](https://github.com/ehsanking/Skills-Ai/releases/latest/download/SkillsAI-windows-x64.zip) — 26 MB | **Portables ZIP.** Ein portabler Build. Irgendwo entpacken und `SkillsAI.exe` starten — es wird nichts installiert, nichts in die Registry geschrieben, und der Katalog wird beim ersten Start nach `%APPDATA%\Skills AI` entpackt. Windows 10 (1809) und neuer, 64 Bit. Zum Entfernen den Ordner löschen. |

<p align="center">
  <img src="screenshots/05-windows.png" width="46%" alt="Der Windows-Build: derselbe Katalog, als Desktop-Fenster">
</p>

Windows wird sagen, es kenne den Herausgeber nicht. Diese Warnung ist zu erwarten: der Build ist nicht mit einem kostenpflichtigen Signaturzertifikat signiert. Statt Sie zu bitten, sie auf Vertrauen hin wegzuklicken, hier der SHA-256 beider Dateien — prüfen Sie die, die Sie geladen haben.

```
3fc2f1d3d222c6ba4b548b09884ed6d8dde9f609dc7f9a9394acfad5d45d0be1  SkillsAI-windows-x64-setup.exe
65b07b4d23503a7f613577d421d882a9b5625ea76aa4638d561f039491d644fa  SkillsAI-windows-x64.zip
```

```
certutil -hashfile SkillsAI-windows-x64-setup.exe SHA256
```

### iPhone und iPad

Es gibt keine App-Store-Version. In Safari öffnen und zum Home-Bildschirm hinzufügen: dann startet es im Vollbild, mit eigenem Icon, und verhält sich wie eine App.

[**ai.ehsanking.ir/app**](https://ai.ehsanking.ir/app)

> Bereits geöffnete Seiten bleiben ohne Verbindung lesbar. Den ganzen Katalog offline tragen die Android- und Windows-Versionen.

## Was es ist

Jedes KI-Werkzeug antwortet besser, wenn man ihm sagt wie. Ein Prompt, der Claude das ständige Entschuldigen abgewöhnt, eine Regel, die Cursor innerhalb deiner Konventionen hält, eine Systemnachricht, die Gemini dazu bringt, so zu schreiben wie eine Muttersprachlerin es täte — das gibt es, verstreut über Hunderte Repositories, und das richtige im richtigen Moment zu finden ist das ganze Problem.

Skills AI sammelt **5,402 davon für 102 Werkzeuge**, sortiert sie in 12 Kategorien und legt sie eine Suche weit weg. Der gesamte Katalog steckt in der App: Sie öffnet im Zug, im Tunnel, im Flugzeug — ohne Empfang und ohne Konto.

## Was es kann

- **Funktioniert ohne Verbindung** — Der ganze Katalog — 5,402 Fähigkeiten, ihr vollständiger Text und der Suchindex — steckt als 17 MB große SQLite-Datenbank in der App. Zum Lesen wird nichts geladen.
- **Eine Suche, die versteht, in welcher Sprache du tippst** — Volltextsuche über jeden Titel und jeden Text, wobei Persisch und Arabisch zusammengefaltet werden: eine mit arabischem Ye getippte Anfrage findet Text mit persischem Ye, und drei Ziffernsätze zählen als einer.
- **Kopieren statt abtippen** — Jede Fähigkeit bringt ihren exakten Text mit, die Installationsanleitung für das Werkzeug, zu dem sie gehört, und einen Kopierknopf an jedem Teil.
- **Hat es wirklich funktioniert?** — Ein Tippen nach der Nutzung sagt, ob es funktioniert hat, teilweise oder gar nicht — für das Modell, das du benutzt hast. Danach werden Fähigkeiten sortiert, pro Person gezählt, sodass häufigeres Antworten nichts verschiebt.
- **Eine Community ohne Punktetafel** — Veröffentliche eigene Fähigkeiten, folge den Leuten, deren Arbeit dir immer wieder hilft, und sieh an der Fähigkeit selbst, wer von ihnen sie ausprobiert hat. Es gibt keine öffentliche Follower-Rangliste und keinen Endpunkt, der den Graphen auflistet.
- **Verkaufen Sie, was Sie schreiben — wenn Sie wollen** — Der Katalog ist kostenlos und bleibt es. Wer eigene Fähigkeiten, Werkzeuge oder Plugins veröffentlicht, darf einen Preis dafür verlangen: Käufer zahlen in Kryptowährung, Verkäufer bekommen USDT, die Plattform behält 12%. Seit 1.1.0 steckt die Verkäuferseite in der App selbst — ein **Verdienen**-Bildschirm mit Guthaben, Wallet, Auszahlungen und dem Preis jedes Angebots. Nichts, was Sie veröffentlichen, kostet etwas, außer Sie setzen selbst einen Preis.
- **Acht Sprachen, vier davon von rechts nach links** — Englisch, Persisch, Arabisch, Türkisch, Hindi, Spanisch, Deutsch und Französisch — die Oberfläche, die Ziffern, die Datumsangaben und die Leserichtung.

## Die eigene Arbeit verkaufen

Alles, was mit der App kommt, ist kostenlos und bleibt es. Daneben gibt es
einen Marktplatz: Wer eigene Arbeit veröffentlicht, darf einen Preis dafür
verlangen.

| | |
|---|---|
| **Sie behalten** | 88% jedes Verkaufs |
| **Wir behalten** | 12% und sonst nichts — keine Einstellgebühr, keine Monatsgebühr, keine Auszahlungsgebühr |
| **Preis** | US-Dollar, 1,00 bis 999,00, von Ihnen festgelegt |
| **Käufer zahlen** | in Kryptowährung, über NOWPayments |
| **Sie bekommen** | USDT, über BEP-20 oder TRC-20 |
| **Kleinste Auszahlung** | 20,00 Dollar |
| **Haltefrist** | 14 Tage, bevor ein Verkauf abgehoben werden kann |

Die Haltefrist ist kein Liquiditätstrick. Die Verkäuferbedingungen versprechen:
Stellt sich ein Angebot als Betrug heraus, verletzt es fremdes Urheberrecht
oder wird es Gegenstand einer belastbaren rechtlichen Forderung, **wird das
Geld eingefroren, an den Käufer zurückgezahlt und das Geschäftskonto
geschlossen** — und dieses Versprechen lässt sich nur halten, solange das Geld
noch hier ist. USDT, das eine Wallet erreicht hat, ist weg.

**Die App verdient; sie kauft nicht.** Seit 1.1.0 ist die Verkäuferseite ein
Bildschirm in der App: Geschäftskonto einschalten, USDT-Wallet hinterlegen,
vier Zahlen, die vier verschiedene Dinge bedeuten, Auszahlung anfordern und die
eigenen Angebote bepreisen. Gekauft wird ein bezahltes Angebot im Browser, und
das ist eine Entscheidung, kein Versäumnis: digitale Güter innerhalb eines
Android-Builds zu verkaufen ist genau das, worum es in den Zahlungsregeln von
Cafe Bazaar und Myket geht. Bezahlt zu werden ist kein Kauf durch die Person,
die das Telefon hält.

Ändert sich die Auszahlungs-Wallet, geht eine Benachrichtigung an das Konto,
dem sie gehört — in der App, in der Web-App und per E-Mail. Eine Adresse, die
Sie nicht gesetzt haben, erfahren Sie in dem Moment, in dem sie gesetzt wird,
nicht dann, wenn eine Auszahlung fehlt.

Die vollständigen Bedingungen stehen in allen acht Sprachen auf der
[Website](https://ai.ehsanking.ir/terms#seller); eine Seite, die das Ganze
erklärt, gibt es unter [ai.ehsanking.ir/earn](https://ai.ehsanking.ir/earn).

## Wie es offline bleibt

<p align="center">
  <img src="../assets/readme/how-it-works.svg" width="100%" alt="Drei Schritte: der ganze Katalog steckt im Download, öffnet ohne Netz und wird bei einem späteren Start durch ein geprüftes Update ersetzt">
</p>

- **Im Download** — `skills.db`, 17 MB SQLite: 5,402 Fähigkeiten mit komprimierten Texten, ein Volltextindex über alle und 33 vollständige Lizenztexte Dritter.
- **Erster Start** — Einmal aus dem Paket kopiert und schreibgeschützt geöffnet. Suchen, lesen, kopieren — kein Netz, kein Konto, keine Anmeldung.
- **Wenn der Katalog wächst** — Der Server veröffentlicht ein neues Korpus. Die App lädt es, prüft seinen sha256 und legt es neben die aktive Datei — nie darüber — und tauscht sie beim nächsten Start aus.

## Wie es gebaut ist

| | |
|---|---|
| **Android** | 8.0 and newer |
| **Flutter** | 3.44 / Dart 3.12 |
| **Catalogue** | SQLite + FTS4, bodies deflated, 17 MB inside the APK |
| **Backend** | Laravel 13 + Filament 5, [ai.ehsanking.ir](https://ai.ehsanking.ir) |
| **Package** | `gfly.skillsai.app` |
| **Tools / skills** | 102 / 5,402 |

## Datenschutz

Der Katalog funktioniert ohne Konto und ohne Netz. Keine Werbe-ID, keine Geräte-ID, kein Analytics-SDK. Ein Konto braucht nur die Community — zum Posten, zum Veröffentlichen einer eigenen Fähigkeit oder um zu sagen, ob eine funktioniert hat — und selbst dann sammelt die App nichts über dich, was du nicht selbst geschrieben hast. Der volle Text steht in der App unter Einstellungen und auf der [Website](https://ai.ehsanking.ir/pp).

## Unterstützen

Alles in der App ist kostenlos — jede Fähigkeit, die Community, die Suche und die Offline-Kopie — ohne Bezahlstufe, ohne Abo und ohne irgendetwas, das hinter einem Konto zurückgehalten wird. Am Laufen halten sie Werbung und Spenden, und beide gehen an dieselbe Stelle: Server, Speicher, Bandbreite und die Arbeit daran, sie besser zu machen.

**Werben** — die App hat zwei gesponserte Plätze. Details auf der [Werbe- und Unterstützungsseite](https://ai.ehsanking.ir/advertise).

**Spenden** — USDT, über eines dieser beiden Netzwerke. BEP-20 ist meist günstiger:

**BEP-20 · BNB Smart Chain**

```
0x53F494E1Fc1Ee777C55B49048dd1ab7e4C5d7244
```

**TRC-20 · TRON**

```
TKPswLQqd2e73UTGJ5prxVXBVo7MTsWedU
```

> Nur USDT, und nur auf diesen beiden Netzwerken. Eine andere Münze oder ein anderes Netzwerk kommt nicht zurück — es ist einfach weg.

## Lizenz

Die Anwendung ist proprietär — siehe [LICENSE](../LICENSE). Du darfst die hier veröffentlichten Builds frei installieren und nutzen; weiterveröffentlichen oder verkaufen darfst du sie nicht.

**Der Katalog nicht.** Jede Fähigkeit gehört der Person, die sie geschrieben hat, und wird unter der von ihr gewählten Lizenz weitergegeben — CC0-1.0, MIT, Apache-2.0 oder CC-BY-4.0. Alle 33 Quellen sind in [THIRD-PARTY-NOTICES.md](../THIRD-PARTY-NOTICES.md) genannt, und dieselben Hinweise liegen der App bei. Eine Fähigkeit ganz ohne Lizenz wurde nicht aufgenommen, denn keine Lizenz heißt keine Erlaubnis.

## Autor

**Ehsan King** — [github.com/ehsanking](https://github.com/ehsanking)
