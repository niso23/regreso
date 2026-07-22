# Changelog

Todos los cambios relevantes de **Regreso** se documentan en este archivo.

El formato sigue [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/)
y el proyecto adhiere a [Versionado Semántico](https://semver.org/lang/es/).

> El código fuente del juego es privado durante la beta; este changelog documenta la evolución de la versión pública jugable.

## [Unreleased]

- Mundo 2: *Seguridad* — protección de claves, estafas avanzadas y resguardo de satoshis.
- Nuevas capturas y material gráfico en este repositorio.

## [0.4.0] - 2026-07-22

Las escenas narrativas del juego (los momentos tipo "aviso en pantalla" que abren y cierran cada capítulo) ahora se narran en voz alta con una voz de inteligencia artificial, en ambos idiomas.

### Añadido

- **Narración por voz con IA** en las escenas narrativas del prólogo y del Mundo 1, en inglés y en español, con una voz elegida específicamente para sonar cálida y natural en ambos idiomas.
- El ritmo de aparición del texto en pantalla ahora sigue el ritmo de la narración en lugar de un tiempo fijo, para que la lectura y el audio vayan siempre sincronizados.
- **Respaldo automático**: si el audio de alguna escena todavía no está disponible (por ejemplo, contenido nuevo recién agregado), el juego narra con la voz del navegador en su lugar, sin quedar nunca en silencio.

### Corregido

- Bug de sonido donde, en ciertas condiciones, podían escucharse dos narraciones superpuestas o la voz de respaldo sonando junto con la narración real.

## [0.3.0] - 2026-07-19

Regreso se abre al mundo: el juego, hasta ahora solo en español, pasa a ser **completamente bilingüe (inglés y español)**, con el **inglés como idioma principal** y una arquitectura de internacionalización pensada para sumar nuevos idiomas sin tocar el código del juego.

### Añadido

- **Internacionalización (i18n) completa**: toda la interfaz, la navegación, la historia, los diálogos, los tutoriales, el glosario, los mundos, los niveles, los minijuegos, las preguntas y respuestas, los mensajes, las notificaciones, los logros, la mochila, los objetos, las colecciones y las pantallas finales están disponibles en **inglés y español**. No queda ningún texto fijo dentro del código.
- **Inglés como idioma por defecto**, con español como segundo idioma. La versión en inglés está *adaptada* para sonar natural a un hablante nativo, no traducida palabra por palabra.
- **Detección automática del idioma** en la primera visita, a partir de la configuración del navegador: si está en español (`es`, `es-ES`, `es-MX`, `es-EC`…), el juego carga en español; para cualquier otra configuración, en inglés.
- **Preferencia de idioma persistente**: al elegir un idioma manualmente, la elección se guarda en el dispositivo y se respeta en las siguientes visitas, por encima del idioma del navegador.
- **Selector de idioma** en la barra superior (🇺🇸 English / 🇪🇸 Español), siempre visible, que cambia toda la interfaz al instante y sin recargar la página.

### Cambiado

- El contenido se reorganizó separando la **lógica del juego** (XP, requisitos, respuestas correctas, configuraciones de minijuegos) de los **textos**, que ahora viven en archivos de traducción por módulo (interfaz, historia, glosario, mundos, logros, objetos, minijuegos…). Añadir un idioma nuevo es tan simple como crear una carpeta de traducciones: no hay que tocar los componentes.
- Todo el progreso existente (guardado, mochila, glosario, XP, logros, colecciones, niveles y mundos) se conserva intacto; la única diferencia es que ahora el idioma puede cambiarse de forma dinámica.

### Corregido

- Los botones de idioma y sonido de la barra superior ya no tapan la información de XP ni el botón de reintentar dentro de un nivel.

## [0.2.0] - 2026-07-15

La actualización más grande hasta la fecha: el juego pasa de ser una historia lineal a una **plataforma de aprendizaje por mundos** con progresión, colecciones y metajuego.

### Añadido

- **Mundo 1: *Descubriendo Bitcoin*** — 4 niveles nuevos completos: qué es Bitcoin, por qué fue creado y por qué cambió la historia del dinero.
- **Sistema de mundos** con desbloqueo progresivo: cada mundo requiere completar el anterior, y el mapa ya muestra los 6 mundos futuros (Seguridad, Lightning, Privacidad, Minería, Economía Bitcoin y Programación Bitcoin) con lo que se aprenderá en cada uno.
- **Mochila**: inventario de objetos educativos que se encuentran durante la aventura (el diario del mes difícil, el documento reconstruido, tu primera wallet, tus primeros satoshis…).
- **Coleccionables**: galería de logos reales del ecosistema Bitcoin (Bitcoin, Mempool, BTCPay Server, entre otros) que se desbloquean al avanzar en la historia, cada uno con su explicación.
- **Glosario interactivo**: los términos se descubren jugando y se aprenden mediante microniveles de 30–60 segundos con explicación sencilla, ejemplo cotidiano y preguntas rápidas; dominar un término otorga XP adicional.
- **Sistema de XP transversal**: experiencia por descubrir, aprender y dominar términos, completar niveles perfectos, mantener la racha diaria, encontrar objetos, desbloquear logos y completar mundos, con barra de progreso global.
- **Nuevos minijuegos**: *Construir Bitcoin* (arma sus propiedades pieza a pieza) y *Dividir Bitcoin* (descubre los satoshis), integrados en los niveles del Mundo 1.
- **Botón de donaciones** dentro del juego para apoyar el desarrollo.

### Cambiado

- El mapa principal se reorganizó en secciones por mundo, con estado de cada nivel (bloqueado, disponible, completado).
- El balance de XP se unificó en una tabla central de recompensas para mantener la progresión coherente entre historia, glosario y colecciones.

## [0.1.0] - 2026-01-07

Primera versión beta pública.

### Añadido

- **Prólogo completo** (3 niveles): *El Mundo del Dinero*, la historia de una persona común durante la crisis financiera de 2008, desde la pérdida de valor de sus ahorros hasta sus primeros satoshis.
- Motor narrativo por pasos: escenas, diálogos, momentos explicativos animados, decisiones y momentos de revelación.
- Minijuegos iniciales: *Asignar el presupuesto*, *El laberinto del dinero*, *Reconstruir el documento* (el whitepaper de Satoshi), *Crear tu primera wallet*, *Detectar la estafa* y *Clic contrarreloj*.
- **Secretos ocultos** en los niveles, con recompensa de XP para quienes exploran.
- **Sistema de logros** con hitos narrativos y de aprendizaje.
- Comparador visual de dinero y explicador de blockchain integrados en la historia.
- Guardado automático de progreso en el dispositivo (sin cuentas ni servidores).
- Sonido ambiental con control de silencio.
- Epílogo y pantalla de resumen al completar cada nivel.
- Despliegue web en Vercel.

[Unreleased]: #
[0.4.0]: #
[0.3.0]: #
[0.2.0]: #
[0.1.0]: #
