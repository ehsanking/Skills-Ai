<h1 align="center">Skills AI</h1>
<p align="center">A directory of AI tools and the skills that make them better at your work — offline, in eight languages.</p>
<p align="center">**English** · [فارسی](docs/README.fa.md) · [العربية](docs/README.ar.md) · [Türkçe](docs/README.tr.md) · [हिन्दी](docs/README.hi.md) · [Español](docs/README.es.md) · [Deutsch](docs/README.de.md) · [Français](docs/README.fr.md)</p>



<p align="center">
  <img src="docs/screenshots/01-home.png" width="22%" alt="">
  <img src="docs/screenshots/02-profile.png" width="22%" alt="">
  <img src="docs/screenshots/03-community.png" width="22%" alt="">
  <img src="docs/screenshots/04-account.png" width="22%" alt="">
</p>


## What it is

Every AI tool answers better when you tell it how. A prompt that makes Claude stop apologising, a rule that keeps Cursor inside your conventions, a system message that gets Gemini to write Persian a native reader would actually write — those exist, scattered across hundreds of repositories, and finding the right one when you need it is the whole problem.

Skills AI collects **5,402 of them for 102 tools**, sorts them into 12 categories, and puts them one search away. The entire catalogue is inside the app: it opens on a train, in a tunnel, on a plane, with no signal and no account.

## What it does

### Works with no connection

The whole catalogue — 5,402 skills, their full text, and the search index — ships inside the app as a 17 MB SQLite database. Nothing is fetched to read it.

### Search that understands the language you type in

Full-text search across every title and body, with Persian and Arabic folded together: a query typed with Arabic yeh finds text written with Persian yeh, and three sets of digits count as one.

### Copy, do not retype

Every skill carries its exact text, an install procedure for the tool it belongs to, and a copy button on each part.

### Did it actually work?

One tap after you use a skill says whether it worked, partly worked, or did not — for the model you used. Skills are ranked by that, counted per person, so answering more often moves nothing.

### A community, without a scoreboard

Publish your own skills, follow the people whose work keeps helping you, and see on a skill itself which of them tried it. There is no public follower ranking and no endpoint that lists the graph.

### Eight languages, four of them right-to-left

English, Persian, Arabic, Turkish, Hindi, Spanish, German and French — the interface, the numerals, the dates and the direction of the layout.

## Download

Grab the APK for your phone from the [latest release](https://github.com/ehsanking/Skills-Ai/releases/latest). Most phones made in the last several years need **arm64-v8a**; older or cheaper ones need **armeabi-v7a**. `x86_64` is for emulators.

If you install the wrong one, Android refuses it — it does not install something broken.

## How it is built

| | |
|---|---|
| **Platform** | Android 8.0 and newer |
| **Framework** | Flutter 3.44 / Dart 3.12 |
| **Catalogue** | SQLite + FTS4, bodies compressed with zlib, 17 MB inside the APK |
| **Backend** | Laravel 13 + Filament 5, at [ai.ehsanking.ir](https://ai.ehsanking.ir) |
| **Package** | `gfly.skillsai.app` |
| **Tools / skills** | 102 / 5,402 |

## Privacy

The catalogue works with no account and no network. No advertising identifier, no device identifier, no analytics SDK. An account is needed only for the community — to post, to publish a skill of your own, or to say whether one worked — and even then the app collects nothing about you that you did not type. The full text is in the app under Settings, and on the [website](https://ai.ehsanking.ir/pp).

## Support

Everything in the app is free — every skill, the community, the search and the offline copy — with no paid tier, no subscription and nothing held back behind an account. What keeps it running is advertising and donations, and both go to the same place: servers, storage, bandwidth and the work of making it better.

**Advertise** — the app has two sponsored slots. Details on the [Advertising & Support page](https://ai.ehsanking.ir/advertise).

**Donate** — USDT on the TRON network (TRC-20):

```
TKPswLQqd2e73UTGJ5prxVXBVo7MTsWedU
```

> USDT · TRC-20 (TRON). Sending any other coin or using any other network will lose it.

## Licence

The application is proprietary — see [LICENSE](LICENSE). You may install and use the builds published here freely; you may not republish or resell them.

The **catalogue is not**. Every skill in it belongs to whoever wrote it and is redistributed under the licence they chose — CC0-1.0, MIT, Apache-2.0 or CC-BY-4.0. All 33 sources are named in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md), and the same notices ship inside the app. A skill offered under no licence at all was not included, because no licence means no permission.

## Author

**Ehsan King** — [github.com/ehsanking](https://github.com/ehsanking)


