# Innex Tools

Exporta desde **Pro Tools** todas las versiones de entrega de un máster (Master, Beat, Acapella, Live y Stems), genera los formatos (WAV 32 float / 24 / 16 bits y MP3), comprueba la calidad de cada archivo y lo deja todo ordenado en la carpeta que elijas. Incluye una cola para exportar varias sesiones seguidas.

> Versión de prueba. Si algo falla, cuéntalo en la pestaña **Issues** de este repositorio.

## Descargar

Entra en **[Releases → Última versión](../../releases/latest)** y baja el instalador de tu equipo:

| Tu equipo | Archivo |
|---|---|
| Mac con chip Apple (M1, M2, M3, M4…) | `Innex-Tools-…-mac-arm64.dmg` |
| Mac con procesador Intel | `Innex-Tools-…-mac-x64.dmg` |
| Windows 10 / 11 | `Innex-Tools-…-win-x64-setup.exe` |

¿No sabes qué Mac tienes? Menú  → **Acerca de este Mac**: si pone «Chip», es Apple; si pone «Procesador», es Intel.

## Qué necesitas antes

1. **Pro Tools** reciente (con PTSL, de 2022.12 en adelante), abierto mientras usas Innex Tools.
2. **El archivo `PTSL.proto` del SDK de Avid.** Lo descargas del SDK de Pro Tools en [developer.avid.com](https://developer.avid.com) (pide una cuenta gratuita de Avid). Dentro de la carpeta del SDK está en `Source/PTSL.proto`. La primera vez que abras Innex Tools te lo pide, lo eliges una sola vez y listo.
3. **ffmpeg** (convierte los formatos y comprueba la calidad):
   - Mac: instala [Homebrew](https://brew.sh) y en la Terminal: `brew install ffmpeg`
   - Windows: en PowerShell: `winget install Gyan.FFmpeg`, y vuelve a abrir Innex Tools.

## Instalar en Mac

1. Abre el `.dmg` y arrastra **Innex Tools** a **Aplicaciones**.
2. La app no está firmada con un certificado de Apple de pago, así que macOS la bloquea la primera vez («no se puede verificar» o «está dañada»). No lo está: se desbloquea una vez de una de estas dos formas:
   - En la Terminal: `xattr -cr "/Applications/Innex Tools.app"` y ábrela con normalidad.
   - O intenta abrirla, y en **Ajustes del Sistema → Privacidad y seguridad**, baja hasta el aviso de Innex Tools y pulsa **Abrir igualmente**.
3. La primera vez macOS te pedirá permiso para acceder a Escritorio y Documentos: acepta.

## Instalar en Windows

1. Ejecuta el `.exe`. Se instala solo, sin pedir permisos de administrador.
2. Windows SmartScreen avisará de que la app no es conocida (no está firmada con certificado de pago). Pulsa **Más información → Ejecutar de todas formas**.

## Actualizar

Cuando hay una versión nueva, la app lo avisa arriba con un botón **Descargar**. Baja el instalador nuevo e instálalo encima: tus ajustes y plantillas se conservan.

## Privacidad

Innex Tools no envía tus sesiones ni tus archivos a ningún sitio. Trabaja en tu ordenador. Lo único que consulta en internet es esta página de GitHub, para saber si hay una versión nueva.
