<p align="center">
  <img src="../assets/readme/hero.es.svg" width="100%" alt="Un directorio de herramientas de IA y las habilidades que las hacen mejores en tu trabajo — sin conexión, en ocho idiomas.">
</p>

<div align="center">

Un directorio de herramientas de IA y las habilidades que las hacen mejores en tu trabajo — sin conexión, en ocho idiomas.

</div>

<div align="center">

[English](../README.md) · [فارسی](README.fa.md) · [العربية](README.ar.md) · [Türkçe](README.tr.md) · [हिन्दी](README.hi.md) · **Español** · [Deutsch](README.de.md) · [Français](README.fr.md)

</div>

## Qué aspecto tiene

<p align="center">
  <img src="screenshots/01-home.png" width="23%" alt="La pantalla de inicio: cada herramienta de IA, ordenada por cuántas habilidades tiene">
  <img src="screenshots/02-profile.png" width="23%" alt="Una persona: las habilidades que publicó y lo que otros dijeron de ellas">
  <img src="screenshots/03-community.png" width="23%" alt="La comunidad: publicaciones, respuestas y habilidades publicadas por lectores">
  <img src="screenshots/04-account.png" width="23%" alt="El estante de la cuenta: iniciar sesión, favoritos, idioma y tema">
</p>

## Descargar

| Archivo | Para |
|---|---|
| [`app-arm64-v8a-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest) | La mayoría de los teléfonos — cualquiera de los últimos ocho años. **Empieza aquí.** |
| [`app-armeabi-v7a-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest) | Teléfonos antiguos o de gama de entrada, 32 bits. |
| [`app-x86_64-release.apk`](https://github.com/ehsanking/Skills-Ai/releases/latest) | Emuladores y las pocas tabletas x86. |

Si eliges el equivocado, Android se niega a instalarlo en lugar de instalar algo roto — así que probar `arm64-v8a` primero no cuesta nada.

### Comprobar lo que descargaste

Cada APK aquí está firmado con la misma clave, y puedes comprobarlo antes de instalar nada:

```
apksigner verify --print-certs app-arm64-v8a-release.apk
```

El certificado debe decir `CN=Ehsan King, OU=Skills AI` con esta huella SHA-256. Una compilación que no la muestre no vino de aquí.

```
DF:9A:3E:BD:B2:28:06:F4:0F:99:3F:64:0D:46:A2:D2:5A:EA:12:49:53:0F:FF:39:C6:75:C4:BB:4F:66:E1:B4
```

## Qué es

Toda herramienta de IA responde mejor cuando le dices cómo. Un prompt que hace que Claude deje de disculparse, una regla que mantiene a Cursor dentro de tus convenciones, un mensaje de sistema que consigue que Gemini escriba como lo haría un hablante nativo — existen, dispersos por cientos de repositorios, y encontrar el adecuado cuando hace falta es todo el problema.

Skills AI reúne **5,402 de ellos para 102 herramientas**, los ordena en 12 categorías y los deja a una búsqueda de distancia. Todo el catálogo está dentro de la app: se abre en un tren, en un túnel, en un avión, sin señal y sin cuenta.

## Qué hace

- **Funciona sin conexión** — Todo el catálogo — 5,402 habilidades, su texto completo y el índice de búsqueda — viaja dentro de la app como una base SQLite de 17 MB. No se descarga nada para leerlo.
- **Una búsqueda que entiende el idioma en que escribes** — Búsqueda de texto completo en cada título y cada cuerpo, con el persa y el árabe plegados juntos: una consulta escrita con ye árabe encuentra texto escrito con ye persa, y los tres conjuntos de dígitos cuentan como uno.
- **Copia, no vuelvas a escribir** — Cada habilidad lleva su texto exacto, el procedimiento de instalación de la herramienta a la que pertenece y un botón de copiar en cada parte.
- **¿Funcionó de verdad?** — Un toque después de usar una habilidad dice si funcionó, funcionó en parte o no funcionó — para el modelo que usaste. Las habilidades se ordenan por eso, contado por persona, así que responder más veces no mueve nada.
- **Una comunidad, sin marcador** — Publica tus propias habilidades, sigue a quienes te ayudan una y otra vez, y ve en la propia habilidad quién de ellos la probó. No hay ranking público de seguidores ni endpoint que liste el grafo.
- **Ocho idiomas, cuatro de derecha a izquierda** — Inglés, persa, árabe, turco, hindi, español, alemán y francés — la interfaz, los números, las fechas y la dirección del diseño.

## Cómo se mantiene sin conexión

<p align="center">
  <img src="../assets/readme/how-it-works.svg" width="100%" alt="Tres pasos: todo el catálogo viene dentro de la descarga, se abre sin red y se reemplaza por una actualización verificada en un arranque posterior">
</p>

- **Dentro de la descarga** — `skills.db`, 17 MB de SQLite: 5402 habilidades con sus textos comprimidos, un índice de texto completo sobre todas ellas y 33 textos de licencia de terceros íntegros.
- **Primer arranque** — Se copia del paquete una vez y se abre en solo lectura. Busca, lee, copia — sin red, sin cuenta, sin registro.
- **Cuando el catálogo crece** — El servidor publica un corpus nuevo. La app lo descarga, comprueba su sha256 y lo deja junto al archivo vivo — nunca encima — y lo sustituye en el siguiente arranque.

## Cómo está hecho

| | |
|---|---|
| **Android** | 8.0 and newer |
| **Flutter** | 3.44 / Dart 3.12 |
| **Catalogue** | SQLite + FTS4, bodies deflated, 17 MB inside the APK |
| **Backend** | Laravel 13 + Filament 5, [ai.ehsanking.ir](https://ai.ehsanking.ir) |
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
