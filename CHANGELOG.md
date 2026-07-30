# Changelog

Todos los cambios relevantes de **Regreso** se documentan en este archivo.

El formato sigue [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/)
y el proyecto adhiere a [Versionado Semántico](https://semver.org/lang/es/).

> El código fuente del juego es privado durante la beta; este changelog documenta la evolución de la versión pública jugable.

## [Unreleased]

- Mundo de *Minería*: cómo se asegura la red y de dónde salen los bitcoins nuevos.
- Nuevas capturas y material gráfico en este repositorio.

## [0.6.0] - 2026-07-29

Todo lo aprendido tiene ahora dónde verse: el juego incorpora el **Bitcoin Journey**, un certificado personal que reúne el recorrido completo del jugador y puede compartirse como imagen.

### Añadido

- **Bitcoin Journey** (`/trayectoria`): un registro personal de aprendizaje con forma de documento, que reúne la ruta recorrida, los conceptos aprendidos y dominados, los artefactos de la mochila, los proyectos del ecosistema descubiertos, los sellos ganados y un resumen del viaje con niveles, mundos y racha. Cada mundo aparece con su color y su motivo propio.
- **Folio del documento**: un identificador corto derivado del progreso real, para que el certificado tenga la forma que uno espera de un documento y dos recorridos distintos no produzcan el mismo papel. Cambia a medida que avanzas.
- **Compartir el certificado como imagen**: el juego dibuja una lámina vertical (1080×1350) diseñada específicamente para verse bien en WhatsApp y redes sociales, en lugar de capturar la pantalla. El reparto usa tres escalones según lo que permita el dispositivo: panel nativo con la imagen adjunta en móvil, descarga del PNG con el texto copiado al portapapeles en escritorio, y solo texto si el navegador no puede generar imágenes. En todos los casos la interfaz informa de lo que ocurrió.
- **Vista previa al compartir el enlace del juego**: al pegar la dirección en X, WhatsApp, Telegram, Reddit o Discord ahora aparece una tarjeta con título, descripción e imagen propia (etiquetas Open Graph y Twitter Card).
- **Acceso al certificado desde el mapa**, con aviso cuando hay un capítulo nuevo por ver.

### Cambiado

- La tarjeta de mundo completado pasa a ser una **franja compacta que sigue el avance real** del jugador, en lugar de una tarjeta grande fija en el prólogo.
- El certificado no guarda una segunda copia del progreso: se genera siempre a partir del estado real de la partida, así que nunca puede quedar desincronizado.
- Los textos de interfaz compartidos (nombre del juego, botones comunes) se movieron a un módulo de traducción propio, reutilizable por el resto del juego.

### Corregido

- El botón de compartir copiaba en silencio y dejaba al jugador sin saber si había ocurrido algo; ahora cada resultado se comunica en pantalla.
- La imagen de vista previa para redes sociales no existía en el sitio publicado: la ruta apuntaba a un archivo ausente y las redes recibían la página del juego en lugar de una imagen. La imagen se genera ahora de forma automática y reproducible en cada publicación.

## [0.5.0] - 2026-07-29

La actualización más grande desde el lanzamiento: el juego **triplica su contenido** con tres mundos nuevos completos. Regreso deja de ser una introducción a Bitcoin para convertirse en un recorrido que va desde la crisis de 2008 hasta la custodia, los pagos instantáneos y la privacidad.

### Añadido

- **Mundo 2: *Seguridad*** (4 niveles) — *La Llave de Todo*, *El Error Irreversible*, *El Engaño* y *La Prueba Final*. Quién tiene realmente la llave de tus sats, por qué en Bitcoin no existe el botón de deshacer, y cómo reconocer que a nadie lo "hackean": lo que intentan es convencerlo.
- **Mundo 3: *Lightning*** (4 niveles) — *El Problema de la Velocidad*, *La Red Invisible*, *Tu Primer Pago Lightning* y *La Red en Acción*. Por qué no todos los pagos son iguales, cómo un pago encuentra su ruta entre canales y nodos, y el hábito de decodificar una factura antes de pagarla.
- **Mundo 4: *Privacidad*** (4 niveles) — *El Libro Abierto*, *Las Huellas*, *No Dejes Tus Huellas* y *El Guardián de la Privacidad*. Bitcoin no es anónimo, y la cadena no dice quién eres: lo dice lo que tú compartes. Nada de lo que se enseña aquí es ilegal; todo revela más de lo necesario.
- **Ocho minijuegos nuevos**, uno por concepto clave: *Detectar el riesgo* y *Verificar la dirección* (Seguridad); *Comparar pagos*, *Encontrar la ruta* y *Pagar una factura* (Lightning); *Explorar la cadena*, *Rastrear la huella* y *Encontrar la fuga* (Privacidad). El juego pasa de 10 a 18 minijuegos.
- **Nivel de prueba final en cada mundo**: el cuarto nivel plantea cinco situaciones reales sin pistas, para demostrar lo aprendido antes de avanzar.
- **Frase de cierre de mundo**: al completar un mundo, la pantalla de resumen muestra una reflexión final que conecta lo aprendido con el mundo siguiente.
- **Seis logros nuevos**: Ojo Entrenado, Guardián de tus Sats, Primer Relámpago, Viajero de la Red, Rastreador y Detective de la Cadena.
- **Contenido de aprendizaje ampliado**: el glosario llega a 44 términos, la mochila a 23 objetos y la colección a 15 logos del ecosistema, todos con su explicación y su micronivel correspondiente.
- **Narración por voz con IA** también en las escenas de los tres mundos nuevos, en inglés y español, manteniendo el respaldo automático por voz del navegador.

### Cambiado

- La meta de XP total se recalculó de 2000 a **7500** para acompañar el nuevo volumen de contenido: la barra de progreso vuelve a reflejar el avance real hasta el final del juego.
- El mapa reordena los mundos futuros: *Minería* pasa a ser el siguiente en desarrollo, después de *Privacidad*.
- Cada mundo nuevo exige completar el anterior (Seguridad → Lightning → Privacidad), manteniendo una curva de dificultad progresiva.

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
[0.6.0]: #
[0.5.0]: #
[0.4.0]: #
[0.3.0]: #
[0.2.0]: #
[0.1.0]: #
