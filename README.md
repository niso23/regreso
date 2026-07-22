<div align="center">

<!-- Logo del juego: reemplazar cuando esté listo -->
<!-- <img src="assets/logo/logo.png" alt="Regreso" width="160" /> -->

# Regreso

### *Encuentra tu libertad*

**Un juego narrativo para aprender Bitcoin desde cero, sin tecnicismos y sin humo.**

[![Estado](https://img.shields.io/badge/estado-beta-orange)](#-estado-del-proyecto)
[![Versión](https://img.shields.io/badge/versi%C3%B3n-0.4.0--beta-blue)](CHANGELOG.md)
[![Plataforma](https://img.shields.io/badge/plataforma-web-brightgreen)](#-juega-ahora)
[![Idiomas](https://img.shields.io/badge/idiomas-english%20%C2%B7%20espa%C3%B1ol-yellow)](#-características)
[![Licencia](https://img.shields.io/badge/licencia-todos%20los%20derechos%20reservados-lightgrey)](LICENSE)

[Juega ahora](#-juega-ahora) · [Características](#-características) · [Roadmap](ROADMAP.md) · [Visión completa](docs/game-overview.md) · [Changelog](CHANGELOG.md)

</div>

---

## 📖 ¿Qué es Regreso?

**Regreso** es un juego educativo narrativo, jugable desde el navegador, que te pone en la piel de una persona común atravesando la crisis financiera de 2008. A través de su historia —ahorros que pierden valor, despidos, bancos que tambalean— descubres, igual que lo hizo el mundo real, por qué nació Bitcoin y qué significa tener dinero que de verdad te pertenece.

No es un curso. No es una charla motivacional. Es una **aventura por niveles**: escenas, decisiones, secretos ocultos, minijuegos y un sistema de progresión que convierte conceptos áridos (inflación, intermediarios, claves privadas, satoshis) en momentos que se sienten y se recuerdan.

## 🎯 El problema que intenta resolver

La educación financiera y sobre Bitcoin tiene hoy dos extremos, y ambos fallan:

- **Contenido técnico** escrito para programadores o economistas, que expulsa al recién llegado en el segundo párrafo.
- **Contenido de "gurús"** que promete riqueza rápida y deja a la gente más expuesta a estafas que antes de empezar.

**Regreso** apuesta por un tercer camino: aprender **jugando una historia**. Nadie recuerda una definición de "intermediario financiero", pero nadie olvida haber enviado $100 a su hermano y que le llegaran $82. El juego transforma cada concepto en una experiencia antes de ponerle nombre — y solo después lo formaliza en el glosario.

## ✨ Características

- 🗺️ **Sistema de mundos** con desbloqueo progresivo: un Prólogo narrativo (la crisis de 2008) y el Mundo 1 *Descubriendo Bitcoin*, con 6 mundos más ya visibles en el mapa.
- 🎮 **10 minijuegos integrados en la historia**: reconstruir el documento de Satoshi, crear tu primera wallet, detectar estafas, resolver el laberinto del dinero, asignar un presupuesto, construir y dividir un bitcoin, y más.
- 📚 **Glosario interactivo**: cada término se descubre jugando y se aprende con un micronivel de 30–60 segundos (explicación sencilla + ejemplo cotidiano + preguntas rápidas).
- 🎒 **Mochila**: objetos educativos que encuentras durante la aventura y cuentan tu propia historia dentro del juego.
- 🏆 **Coleccionables**: logos reales del ecosistema Bitcoin (Bitcoin, Mempool, BTCPay Server…) que se desbloquean al avanzar, cada uno con su explicación.
- ⭐ **Sistema de XP transversal**: ganas experiencia por avanzar en la historia, aprender términos, completar niveles perfectos, mantener tu racha diaria y descubrir secretos.
- 🕵️ **Secretos ocultos** en los niveles, para quienes miran dos veces.
- 🏅 **Logros** que marcan los hitos de tu viaje.
- 💾 **Progreso guardado localmente**: tu partida es tuya, sin cuentas ni servidores.
- 🌍 **Bilingüe (inglés y español)**: detección automática del idioma del navegador en la primera visita, cambio instantáneo desde la barra superior y preferencia guardada. El inglés es el idioma por defecto y la arquitectura está preparada para sumar más idiomas.
- 🎙️ **Narración por voz con IA** en las escenas narrativas del juego, en ambos idiomas, con respaldo automático si algún audio no está disponible.
- 🔊 **Sonido ambiental** con control de silencio.
- ❤️ **Botón de donaciones** para quienes quieran apoyar el desarrollo.

## 📸 Capturas de pantalla

<!-- Reemplazar los marcadores por capturas reales en assets/screenshots/ -->

| Mapa de mundos | Nivel narrativo | Minijuego |
| :---: | :---: | :---: |
| *(próximamente)* | *(próximamente)* | *(próximamente)* |
| `assets/screenshots/mapa.png` | `assets/screenshots/nivel.png` | `assets/screenshots/minijuego.png` |

| Glosario | Mochila | Perfil y logros |
| :---: | :---: | :---: |
| *(próximamente)* | *(próximamente)* | *(próximamente)* |
| `assets/screenshots/glosario.png` | `assets/screenshots/mochila.png` | `assets/screenshots/perfil.png` |

<!-- GIFs de jugabilidad: assets/gifs/ -->

## 🛠️ Tecnologías

| Área | Tecnología |
| --- | --- |
| Interfaz | React 19 |
| Build y desarrollo | Vite 8 |
| Estilos | Tailwind CSS 4 |
| Animaciones | Motion (Framer Motion) |
| Navegación | React Router 7 |
| Iconografía | Lucide |
| Internacionalización | Sistema i18n propio (archivos de traducción por módulo) |
| Narración por voz | ElevenLabs (IA), con Web Speech API como respaldo |
| Calidad de código | Oxlint |
| Despliegue | Vercel |

## 🚧 Estado del proyecto

**Beta pública.** El Prólogo y el Mundo 1 están completos y jugables de principio a fin. El contenido, el balance de XP y la interfaz siguen evolucionando semana a semana.

> **Nota sobre el código fuente:** este repositorio contiene únicamente la documentación y presentación del proyecto. El código fuente permanece privado durante la fase beta y se evaluará su publicación al alcanzar la versión estable. Este repositorio sirve además como registro público de autoría del proyecto.

## 🗺️ Roadmap resumido

- ✅ Prólogo completo (3 niveles) — la crisis de 2008 y tus primeros satoshis
- ✅ Mundo 1: *Descubriendo Bitcoin* (4 niveles)
- ✅ Glosario, mochila, coleccionables, logros, XP y rachas
- ✅ Juego bilingüe (inglés y español) con detección automática y selector de idioma
- ✅ Narración por voz con IA en las escenas narrativas, en ambos idiomas
- 🔄 Mundo 2: *Seguridad* — proteger claves y detectar estafas avanzadas
- 🔜 Mundo 3: *Lightning* — pagos instantáneos sobre Bitcoin
- 🔜 Mundo 4: *Privacidad*
- 💡 Minería, Economía Bitcoin, Programación Bitcoin, y más

El detalle completo está en [ROADMAP.md](ROADMAP.md).

## 🕹️ Cómo jugar

1. Abre el juego en tu navegador (enlace abajo). Funciona en escritorio y móvil, sin instalar nada.
2. Comienza por el **Prólogo**: vive la historia, toma decisiones y completa los minijuegos.
3. Explora: hay **secretos ocultos** que premian la curiosidad.
4. Visita el **glosario** y completa los microniveles para dominar cada término.
5. Revisa tu **mochila**, tus **coleccionables** y tu **perfil** para ver cuánto has avanzado.
6. Vuelve cada día: la **racha diaria** también da XP.

Tu progreso se guarda automáticamente en tu dispositivo.

## 🔗 Juega ahora

**➡️ [Jugar Regreso](https://regreso-psi.vercel.app/)**

## 📄 Licencia

© 2026 niso23. **Todos los derechos reservados.**

La documentación e imágenes de este repositorio pueden consultarse libremente, pero no reutilizarse ni redistribuirse sin autorización. Ver [LICENSE](LICENSE) para el detalle.

## 👤 Autor

**niso23** — diseño, narrativa, desarrollo y contenido educativo.

Proyecto creado y mantenido por una sola persona. Si el juego te aportó algo, la mejor forma de apoyarlo es jugarlo, compartirlo y, si quieres, usar el botón de donaciones dentro del juego.

---

<div align="center">
<sub>Hecho con la convicción de que entender el dinero no debería ser un privilegio.</sub>
</div>
