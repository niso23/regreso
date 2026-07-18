# Regreso — Visión general del proyecto

*Encuentra tu libertad.*

Este documento explica en profundidad qué es **Regreso**, por qué existe, cómo enseña y hacia dónde va. Es la referencia de diseño del proyecto en su versión pública.

---

## 1. Objetivo

**Que cualquier persona, sin conocimientos previos de economía ni de tecnología, entienda qué es Bitcoin, por qué existe y cómo usarlo con criterio propio — jugando.**

Regreso no busca convencer a nadie de comprar nada. Busca algo anterior y más importante: que el jugador *entienda*. Que al terminar cada mundo pueda explicar con sus palabras qué es un intermediario financiero, por qué la inflación erosiona sus ahorros, qué es una clave privada o por qué un bitcoin se divide en cien millones de satoshis. La libertad del subtítulo no es un eslogan: es la que da comprender cómo funciona el dinero que usas todos los días.

## 2. Filosofía educativa

Regreso se construye sobre cuatro principios:

### La experiencia antes que la definición

El juego nunca abre con teoría. Primero el jugador **vive** el problema: envía $100 a su hermano y llegan $82; ve sus ahorros perder valor durante la crisis de 2008; pierde el acceso a algo por no custodiar una clave. Solo después, cuando la experiencia ya generó la pregunta, el glosario le pone nombre y estructura a lo que acaba de sentir. El orden es deliberado: la emoción crea el gancho, la definición llega cuando hay dónde colgarla.

### Honestidad radical

El contenido evita las dos trampas del género: el tecnicismo que excluye y la promesa de riqueza que estafa. Regreso no promete ganancias, no da consejos de inversión y dedica niveles enteros a **detectar estafas**. Si algo tiene riesgos, el juego los cuenta.

### Respeto por el tiempo del jugador

Cada pieza de aprendizaje es corta y completa: los microniveles del glosario duran 30–60 segundos; los niveles narrativos se completan en una sesión. Nada exige maratones, y la racha diaria premia la constancia en dosis pequeñas — el ritmo con el que realmente se consolida lo aprendido.

### La curiosidad se premia

Los niveles esconden **secretos**: datos reales e inquietantes que solo encuentra quien explora. El mensaje implícito es el corazón del proyecto: *no te quedes con lo que te muestran; mira dos veces, verifica por tu cuenta.*

## 3. Cómo funciona el sistema de aprendizaje

El aprendizaje en Regreso es un ciclo de cuatro etapas que se repite con cada concepto:

```
  VIVIR ──────► DESCUBRIR ──────► APRENDER ──────► DOMINAR
  (historia)    (el término       (micronivel:      (preguntas de
                 aparece en el     explicación +     dominio, XP
                 glosario)         ejemplo +         adicional)
                                   preguntas)
```

1. **Vivir.** La historia pone al jugador en una situación donde el concepto importa (una comisión que se come su envío, un banco que quiebra, una wallet que hay que proteger).
2. **Descubrir.** Ese momento desbloquea el término en el **glosario**. Descubrirlo ya otorga XP: el juego celebra la exposición al concepto, no solo su dominio.
3. **Aprender.** El jugador completa el **micronivel** del término: una explicación en lenguaje llano, un ejemplo cotidiano (una encomienda, una fotocopia, una llave) y una o dos preguntas rápidas. Responder todo correctamente da un bonus.
4. **Dominar.** Preguntas posteriores consolidan el término y otorgan el XP de dominio. Los objetos de la **mochila** y los **logos coleccionables** refuerzan el recuerdo: cada uno es un ancla física de algo que el jugador ya vivió.

Todo el sistema de XP está balanceado de forma centralizada (descubrir: 5 XP, aprender: 15 XP, dominar: 10 XP, nivel perfecto: 25 XP, racha diaria: 10 XP, mundo completado: 50 XP…) para que la progresión se sienta coherente entre historia, glosario y colecciones.

## 4. Mecánicas

### Estructura: mundos y niveles

El contenido se organiza en **mundos** temáticos que se desbloquean en orden:

| Mundo | Estado | Qué se aprende |
| --- | --- | --- |
| **Prólogo** | ✅ Jugable | La crisis de 2008 vivida en primera persona: inflación, intermediarios, el documento de Satoshi, la primera wallet, los primeros satoshis. |
| **Mundo 1: Descubriendo Bitcoin** | ✅ Jugable | Qué es Bitcoin, por qué fue creado, sus propiedades y por qué cambió la historia del dinero. |
| **Seguridad** | 🔄 En desarrollo | Proteger claves, detectar estafas avanzadas, custodia a prueba de errores. |
| **Lightning** | 🔜 Planificado | Pagos instantáneos sobre Bitcoin. |
| **Privacidad** | 🔜 Planificado | Qué revela cada transacción y cómo cuidar tus datos. |
| **Minería** | 💡 Futuro | Cómo se asegura la red y de dónde salen los bitcoins nuevos. |
| **Economía Bitcoin** | 💡 Futuro | Escasez, halving, pensamiento a largo plazo. |
| **Programación Bitcoin** | 💡 Futuro | Scripts, nodos propios, primeras herramientas. |

Cada nivel es una secuencia de **pasos**: escenas ambientales, diálogos fechados ("Día 1", "Día 15"…), explicativos animados cuadro a cuadro, decisiones, minijuegos, momentos de revelación y secretos ocultos.

### Minijuegos

Los minijuegos nunca son relleno: cada uno materializa el concepto del nivel donde aparece.

| Minijuego | Concepto que enseña |
| --- | --- |
| Asignar el presupuesto | A dónde se va el dinero de un mes real |
| El laberinto del dinero | Los intermediarios y comisiones de cada envío |
| Reconstruir el documento | El whitepaper de Satoshi, pieza a pieza |
| Crear tu primera wallet | Claves, custodia y responsabilidad propia |
| Detectar la estafa | Señales de fraude antes de que te alcancen |
| Clic contrarreloj | Actuar a tiempo bajo presión |
| Juego de memoria | Fijar conceptos por repetición activa |
| Arrastrar y clasificar | Distinguir categorías (qué es dinero, qué no) |
| Construir Bitcoin | Las propiedades que lo hacen único, pieza a pieza |
| Dividir Bitcoin | Los satoshis: por qué no necesitas "un bitcoin entero" |

### Progresión y colecciones

- **XP y barra de progreso global** hacia una meta total (~2000 XP en la versión actual).
- **Racha diaria** que premia volver cada día.
- **Mochila** con objetos narrativos encontrados en la aventura.
- **Coleccionables**: logos reales del ecosistema (Bitcoin, Mempool, BTCPay Server…), cada uno con su explicación — el jugador termina reconociendo el ecosistema real, no solo el del juego.
- **Logros** por hitos de historia, curiosidad y aprendizaje.

### Persistencia y privacidad

El progreso se guarda **localmente en el dispositivo del jugador**. No hay registro, cuentas, ni recolección de datos. Es una decisión de diseño coherente con el tema del juego: tu progreso, como tus claves, te pertenece.

## 5. Público objetivo

- **Personas adultas sin formación financiera ni técnica** que escuchan hablar de Bitcoin y quieren entender de qué se trata sin que las estafen en el intento. Es el público principal y el listón de claridad: si un nivel no lo entiende un recién llegado, se reescribe.
- **Jóvenes y estudiantes** (16+) que prefieren aprender jugando antes que leyendo manuales.
- **Educadores y divulgadores** que buscan una herramienta en español, honesta y sin conflictos de interés, para introducir estos temas.
- **Hispanohablantes en economías con inflación alta**, para quienes los problemas que narra el juego no son historia: son el presente.

El juego está escrito íntegramente en español, con lenguaje cotidiano y ejemplos de la vida real.

## 6. Futuras mejoras

En orden aproximado de prioridad (el detalle vive en [ROADMAP.md](../ROADMAP.md)):

1. **Mundo 2: Seguridad** — el contenido más pedido: custodia y anti-estafas en profundidad.
2. **Mundos Lightning y Privacidad**, con sus minijuegos, términos y coleccionables propios.
3. **Modo repaso** del glosario, para mantener frescos los conceptos ya dominados.
4. **Exportar/importar partida**, manteniendo la filosofía sin cuentas.
5. **PWA instalable con modo offline**, pensando en jugadores con conectividad limitada.
6. **Traducciones** (inglés, portugués) una vez estabilizado el contenido en español.
7. **Accesibilidad ampliada**: lector de pantalla, alto contraste, tamaños de texto.
8. **Publicación del código fuente** al alcanzar la versión estable, junto con una guía para contribuir.

---

*Documento vivo: se actualiza con cada versión del juego. Última revisión: julio de 2026.*
