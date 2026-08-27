<h1 align="center">Skills AI</h1>
<p align="center">Ein Verzeichnis von KI-Werkzeugen und den Fähigkeiten, die sie in deiner Arbeit besser machen — offline, in acht Sprachen.</p>
<p align="center">[English](../README.md) · [فارسی](README.fa.md) · [العربية](README.ar.md) · [Türkçe](README.tr.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · **Deutsch** · [Français](README.fr.md)</p>



<p align="center">
  <img src="../docs/screenshots/01-home.png" width="22%" alt="">
  <img src="../docs/screenshots/02-profile.png" width="22%" alt="">
  <img src="../docs/screenshots/03-community.png" width="22%" alt="">
  <img src="../docs/screenshots/04-account.png" width="22%" alt="">
</p>


## Was es ist

Jedes KI-Werkzeug antwortet besser, wenn man ihm sagt wie. Ein Prompt, der Claude das ständige Entschuldigen abgewöhnt, eine Regel, die Cursor innerhalb deiner Konventionen hält, eine Systemnachricht, die Gemini dazu bringt, so zu schreiben wie eine Muttersprachlerin es täte — das gibt es, verstreut über Hunderte Repositories, und das richtige im richtigen Moment zu finden ist das ganze Problem.

Skills AI sammelt **5,402 davon für 102 Werkzeuge**, sortiert sie in 12 Kategorien und legt sie eine Suche weit weg. Der gesamte Katalog steckt in der App: Sie öffnet im Zug, im Tunnel, im Flugzeug — ohne Empfang und ohne Konto.

## Was es kann

### Funktioniert ohne Verbindung

Der ganze Katalog — 5,402 Fähigkeiten, ihr vollständiger Text und der Suchindex — steckt als 17 MB große SQLite-Datenbank in der App. Zum Lesen wird nichts geladen.

### Eine Suche, die versteht, in welcher Sprache du tippst

Volltextsuche über jeden Titel und jeden Text, wobei Persisch und Arabisch zusammengefaltet werden: eine mit arabischem Ye getippte Anfrage findet Text mit persischem Ye, und drei Ziffernsätze zählen als einer.

### Kopieren statt abtippen

Jede Fähigkeit bringt ihren exakten Text mit, die Installationsanleitung für das Werkzeug, zu dem sie gehört, und einen Kopierknopf an jedem Teil.

### Hat es wirklich funktioniert?

Ein Tippen nach der Nutzung sagt, ob es funktioniert hat, teilweise oder gar nicht — für das Modell, das du benutzt hast. Danach werden Fähigkeiten sortiert, pro Person gezählt, sodass häufigeres Antworten nichts verschiebt.

### Eine Community ohne Punktetafel

Veröffentliche eigene Fähigkeiten, folge den Leuten, deren Arbeit dir immer wieder hilft, und sieh an der Fähigkeit selbst, wer von ihnen sie ausprobiert hat. Es gibt keine öffentliche Follower-Rangliste und keinen Endpunkt, der den Graphen auflistet.

### Acht Sprachen, vier davon von rechts nach links

Englisch, Persisch, Arabisch, Türkisch, Hindi, Spanisch, Deutsch und Französisch — die Oberfläche, die Ziffern, die Datumsangaben und die Leserichtung.

## Herunterladen

Lade die APK für dein Telefon aus der [neuesten Version](https://github.com/ehsanking/Skills-Ai/releases/latest). Die meisten Geräte der letzten Jahre brauchen **arm64-v8a**; ältere oder günstigere **armeabi-v7a**. `x86_64` ist für Emulatoren.

Installierst du die falsche, weist Android sie ab — es installiert nichts Kaputtes.

## Wie es gebaut ist

| | |
|---|---|
| **Platform** | Android 8.0 and newer |
| **Framework** | Flutter 3.44 / Dart 3.12 |
| **Catalogue** | SQLite + FTS4, bodies compressed with zlib, 17 MB inside the APK |
| **Backend** | Laravel 13 + Filament 5, at [ai.ehsanking.ir](https://ai.ehsanking.ir) |
| **Package** | `gfly.skillsai.app` |
| **Tools / skills** | 102 / 5,402 |

## Datenschutz

Der Katalog funktioniert ohne Konto und ohne Netz. Keine Werbe-ID, keine Geräte-ID, kein Analytics-SDK. Ein Konto braucht nur die Community — zum Posten, zum Veröffentlichen einer eigenen Fähigkeit oder um zu sagen, ob eine funktioniert hat — und selbst dann sammelt die App nichts über dich, was du nicht selbst geschrieben hast. Der volle Text steht in der App unter Einstellungen und auf der [Website](https://ai.ehsanking.ir/pp).

## Unterstützen

Alles in der App ist kostenlos — jede Fähigkeit, die Community, die Suche und die Offline-Kopie — ohne Bezahlstufe, ohne Abo und ohne irgendetwas, das hinter einem Konto zurückgehalten wird. Am Laufen halten sie Werbung und Spenden, und beide gehen an dieselbe Stelle: Server, Speicher, Bandbreite und die Arbeit daran, sie besser zu machen.

**Werben** — die App hat zwei gesponserte Plätze. Details auf der [Werbe- und Unterstützungsseite](https://ai.ehsanking.ir/advertise).

**Spenden** — USDT im TRON-Netzwerk (TRC-20):

```
TKPswLQqd2e73UTGJ5prxVXBVo7MTsWedU
```

> USDT · TRC-20 (TRON). Sending any other coin or using any other network will lose it.

## Lizenz

Die Anwendung ist proprietär — siehe [LICENSE](../LICENSE). Du darfst die hier veröffentlichten Builds frei installieren und nutzen; weiterveröffentlichen oder verkaufen darfst du sie nicht.

**Der Katalog nicht.** Jede Fähigkeit gehört der Person, die sie geschrieben hat, und wird unter der von ihr gewählten Lizenz weitergegeben — CC0-1.0, MIT, Apache-2.0 oder CC-BY-4.0. Alle 33 Quellen sind in [THIRD-PARTY-NOTICES.md](../THIRD-PARTY-NOTICES.md) genannt, und dieselben Hinweise liegen der App bei. Eine Fähigkeit ganz ohne Lizenz wurde nicht aufgenommen, denn keine Lizenz heißt keine Erlaubnis.

## Autor

**Ehsan King** — [github.com/ehsanking](https://github.com/ehsanking)


