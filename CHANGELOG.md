# Changelog

Todos los cambios relevantes de **Regreso** se documentan en este archivo.

El formato sigue [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/)
y el proyecto adhiere a [Versionado Semántico](https://semver.org/lang/es/).

> El código fuente del juego es privado durante la beta; este changelog documenta la evolución de la versión pública jugable.

## [Unreleased]

- Mundo 2: *Seguridad* — protección de claves, estafas avanzadas y resguardo de satoshis.
- Nuevas capturas y material gráfico en este repositorio.

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
[0.2.0]: #
[0.1.0]: #
