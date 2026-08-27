<h1 align="center">Skills AI</h1>
<p align="center">Un directorio de herramientas de IA y las habilidades que las hacen mejores en tu trabajo — sin conexión, en ocho idiomas.</p>
<p align="center">[English](../README.md) · [فارسی](README.fa.md) · [العربية](README.ar.md) · [Türkçe](README.tr.md) · [हिन्दी](README.hi.md) · **Español** · [Deutsch](README.de.md) · [Français](README.fr.md)</p>



<p align="center">
  <img src="../docs/screenshots/01-home.png" width="22%" alt="">
  <img src="../docs/screenshots/02-profile.png" width="22%" alt="">
  <img src="../docs/screenshots/03-community.png" width="22%" alt="">
  <img src="../docs/screenshots/04-account.png" width="22%" alt="">
</p>


## Qué es

Toda herramienta de IA responde mejor cuando le dices cómo. Un prompt que hace que Claude deje de disculparse, una regla que mantiene a Cursor dentro de tus convenciones, un mensaje de sistema que consigue que Gemini escriba como lo haría un hablante nativo — existen, dispersos por cientos de repositorios, y encontrar el adecuado cuando hace falta es todo el problema.

Skills AI reúne **5,402 de ellos para 102 herramientas**, los ordena en 12 categorías y los deja a una búsqueda de distancia. Todo el catálogo está dentro de la app: se abre en un tren, en un túnel, en un avión, sin señal y sin cuenta.

## Qué hace

### Funciona sin conexión

Todo el catálogo — 5,402 habilidades, su texto completo y el índice de búsqueda — viaja dentro de la app como una base SQLite de 17 MB. No se descarga nada para leerlo.

### Una búsqueda que entiende el idioma en que escribes

Búsqueda de texto completo en cada título y cada cuerpo, con el persa y el árabe plegados juntos: una consulta escrita con ye árabe encuentra texto escrito con ye persa, y los tres conjuntos de dígitos cuentan como uno.

### Copia, no vuelvas a escribir

Cada habilidad lleva su texto exacto, el procedimiento de instalación de la herramienta a la que pertenece y un botón de copiar en cada parte.

### ¿Funcionó de verdad?

Un toque después de usar una habilidad dice si funcionó, funcionó en parte o no funcionó — para el modelo que usaste. Las habilidades se ordenan por eso, contado por persona, así que responder más veces no mueve nada.

### Una comunidad, sin marcador

Publica tus propias habilidades, sigue a quienes te ayudan una y otra vez, y ve en la propia habilidad quién de ellos la probó. No hay ranking público de seguidores ni endpoint que liste el grafo.

### Ocho idiomas, cuatro de derecha a izquierda

Inglés, persa, árabe, turco, hindi, español, alemán y francés — la interfaz, los números, las fechas y la dirección del diseño.

## Descargar

Descarga el APK para tu teléfono desde la [última versión](https://github.com/ehsanking/Skills-Ai/releases/latest). La mayoría de los teléfonos de los últimos años necesitan **arm64-v8a**; los más antiguos o económicos, **armeabi-v7a**. `x86_64` es para emuladores.

Si instalas el equivocado, Android lo rechaza: no instala algo roto.

## Cómo está hecho

| | |
|---|---|
| **Platform** | Android 8.0 and newer |
| **Framework** | Flutter 3.44 / Dart 3.12 |
| **Catalogue** | SQLite + FTS4, bodies compressed with zlib, 17 MB inside the APK |
| **Backend** | Laravel 13 + Filament 5, at [ai.ehsanking.ir](https://ai.ehsanking.ir) |
| **Package** | `gfly.skillsai.app` |
| **Tools / skills** | 102 / 5,402 |

## Privacidad

El catálogo funciona sin cuenta y sin red. Sin identificador publicitario, sin identificador de dispositivo, sin SDK de analítica. Solo hace falta una cuenta para la comunidad — publicar, compartir una habilidad propia o decir si funcionó — e incluso entonces la app no recoge nada sobre ti que tú no hayas escrito. El texto completo está en la app, en Ajustes, y en la [web](https://ai.ehsanking.ir/pp).

## Apoyo

Todo en la app es gratis — cada habilidad, la comunidad, la búsqueda y la copia sin conexión — sin nivel de pago, sin suscripción y sin nada retenido tras una cuenta. Lo que la mantiene en marcha son la publicidad y las donaciones, y ambas van al mismo sitio: servidores, almacenamiento, ancho de banda y el trabajo de mejorarla.

**Anúnciate** — la app tiene dos espacios patrocinados. Detalles en la [página de Publicidad y Apoyo](https://ai.ehsanking.ir/advertise).

**Dona** — USDT en la red TRON (TRC-20):

```
TKPswLQqd2e73UTGJ5prxVXBVo7MTsWedU
```

> USDT · TRC-20 (TRON). Sending any other coin or using any other network will lose it.

## Licencia

La aplicación es propietaria — véase [LICENSE](../LICENSE). Puedes instalar y usar libremente las versiones publicadas aquí; no puedes redistribuirlas ni revenderlas.

**El catálogo no lo es.** Cada habilidad pertenece a quien la escribió y se redistribuye bajo la licencia que eligió — CC0-1.0, MIT, Apache-2.0 o CC-BY-4.0. Las 33 fuentes están nombradas en [THIRD-PARTY-NOTICES.md](../THIRD-PARTY-NOTICES.md), y los mismos avisos viajan dentro de la app. Una habilidad sin ninguna licencia no se incluyó, porque sin licencia no hay permiso.

## Autor

**Ehsan King** — [github.com/ehsanking](https://github.com/ehsanking)


