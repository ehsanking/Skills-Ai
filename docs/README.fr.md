<h1 align="center">Skills AI</h1>
<p align="center">Un répertoire d'outils d'IA et des compétences qui les rendent meilleurs dans votre travail — hors ligne, en huit langues.</p>
<p align="center">[English](../README.md) · [فارسی](README.fa.md) · [العربية](README.ar.md) · [Türkçe](README.tr.md) · [हिन्दी](README.hi.md) · [Español](README.es.md) · [Deutsch](README.de.md) · **Français**</p>



<p align="center">
  <img src="../docs/screenshots/01-home.png" width="22%" alt="">
  <img src="../docs/screenshots/02-profile.png" width="22%" alt="">
  <img src="../docs/screenshots/03-community.png" width="22%" alt="">
  <img src="../docs/screenshots/04-account.png" width="22%" alt="">
</p>


## Ce que c'est

Tout outil d'IA répond mieux quand on lui dit comment. Un prompt qui empêche Claude de s'excuser sans arrêt, une règle qui maintient Cursor dans vos conventions, un message système qui pousse Gemini à écrire ce qu’un locuteur natif écrirait vraiment — cela existe, éparpillé dans des centaines de dépôts, et trouver le bon au bon moment est tout le problème.

Skills AI en rassemble **5,402 pour 102 outils**, les range en 12 catégories et les met à une recherche de distance. Tout le catalogue est dans l'application : elle s'ouvre dans un train, dans un tunnel, dans un avion, sans réseau et sans compte.

## Ce qu’il fait

### Fonctionne sans connexion

Tout le catalogue — 5,402 compétences, leur texte intégral et l'index de recherche — tient dans l'application sous forme d'une base SQLite de 17 Mo. Rien n'est téléchargé pour le lire.

### Une recherche qui comprend la langue dans laquelle vous tapez

Recherche plein texte sur chaque titre et chaque corps, le persan et l’arabe étant repliés ensemble : une requête tapée avec le yé arabe trouve un texte écrit avec le yé persan, et les trois jeux de chiffres comptent pour un.

### Copiez, ne retapez pas

Chaque compétence porte son texte exact, la procédure d'installation pour l'outil auquel elle appartient, et un bouton de copie sur chaque partie.

### Est-ce que ça a vraiment marché ?

Une pression après avoir utilisé une compétence dit si elle a marché, en partie, ou pas — pour le modèle que vous avez utilisé. Les compétences sont classées là-dessus, compté par personne, donc répondre plus souvent ne déplace rien.

### Une communauté, sans tableau des scores

Publiez vos propres compétences, suivez les personnes dont le travail vous sert régulièrement, et voyez sur la compétence elle-même qui parmi elles l’a essayée. Il n’y a aucun classement public d’abonnés et aucun point d’accès qui liste le graphe.

### Huit langues, dont quatre de droite à gauche

Anglais, persan, arabe, turc, hindi, espagnol, allemand et français — l'interface, les chiffres, les dates et le sens de la mise en page.

## Télécharger

Téléchargez l'APK de votre téléphone depuis la [dernière version](https://github.com/ehsanking/Skills-Ai/releases/latest). La plupart des téléphones récents ont besoin de **arm64-v8a** ; les plus anciens ou plus abordables, de **armeabi-v7a**. `x86_64` est pour les émulateurs.

Si vous installez le mauvais, Android le refuse : il n'installe rien de cassé.

## Comment c’est construit

| | |
|---|---|
| **Platform** | Android 8.0 and newer |
| **Framework** | Flutter 3.44 / Dart 3.12 |
| **Catalogue** | SQLite + FTS4, bodies compressed with zlib, 17 MB inside the APK |
| **Backend** | Laravel 13 + Filament 5, at [ai.ehsanking.ir](https://ai.ehsanking.ir) |
| **Package** | `gfly.skillsai.app` |
| **Tools / skills** | 102 / 5,402 |

## Confidentialité

Le catalogue fonctionne sans compte et sans réseau. Aucun identifiant publicitaire, aucun identifiant d’appareil, aucun SDK d’analytique. Un compte n'est nécessaire que pour la communauté — publier, proposer votre propre compétence ou dire si elle a marché — et même alors, l'application ne recueille rien sur vous que vous n'ayez écrit. Le texte complet est dans l’app sous Réglages et sur le [site](https://ai.ehsanking.ir/pp).

## Soutenir

Tout dans l'application est gratuit — chaque compétence, la communauté, la recherche et la copie hors ligne — sans palier payant, sans abonnement et sans rien retenu derrière un compte. Ce qui la fait tourner, c’est la publicité et les dons, et les deux vont au même endroit : serveurs, stockage, bande passante et le travail pour l’améliorer.

**Annoncer** — l’application a deux emplacements sponsorisés. Détails sur la [page Publicité et soutien](https://ai.ehsanking.ir/advertise).

**Faire un don** — USDT sur le réseau TRON (TRC-20) :

```
TKPswLQqd2e73UTGJ5prxVXBVo7MTsWedU
```

> USDT · TRC-20 (TRON). Sending any other coin or using any other network will lose it.

## Licence

L'application est propriétaire — voir [LICENSE](../LICENSE). Vous pouvez installer et utiliser librement les versions publiées ici ; vous ne pouvez ni les republier ni les revendre.

**Le catalogue, non.** Chaque compétence appartient à qui l’a écrite et est redistribuée sous la licence qu’elle a choisie — CC0-1.0, MIT, Apache-2.0 ou CC-BY-4.0. Les 33 sources sont nommées dans [THIRD-PARTY-NOTICES.md](../THIRD-PARTY-NOTICES.md), et les mêmes avis accompagnent l'application. Une compétence sans aucune licence n'a pas été incluse, car pas de licence signifie pas de permission.

## Auteur

**Ehsan King** — [github.com/ehsanking](https://github.com/ehsanking)


