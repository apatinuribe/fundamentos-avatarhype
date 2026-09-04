---
name: avatarhype
description: Crea anuncios para ecommerce con IA siguiendo el método AvatarHype, en sus dos tracks: UGC realista con avatar humano (estrategia por ángulo y nivel de conciencia, guion clip a clip, imagen desde una referencia real, animación con Omni o Grok, limpieza de marca de agua y capa de realismo en CapCut) y ads animados (cadena de 8 prompts encadenados en ChatGPT y NotebookLM, imágenes 2K con Nano Banana Pro, transiciones con Kling 3, voz en ElevenLabs). Úsala cuando el usuario pida un anuncio UGC, un vídeo con avatar de IA, un guion para Meta Ads, prompts de imagen o de clip para Nano Banana, GPT Image, Veo, Omni Flash, Grok Imagine o Kling, un anuncio animado en estilo Pixar, claymation, Wes Anderson o sci-fi, o cuando mencione formatos como UGC con producto, moda, app o SaaS, podcast, dualcast, voz en off, trend viral o imágenes estáticas.
---

# AvatarHype — anuncios de ecommerce con IA

Dos métodos completos de la misma academia. **Lo primero es elegir track**, porque cambian la cadena de
herramientas entera y no se mezclan:

| Track | Cuándo | Cadena |
|---|---|---|
| **Realista** (etapas 1-6 de abajo) | Persona a cámara, UGC, testimonio, demo de producto en mano | Imagen (Nano Banana / GPT Image) → Omni o Grok → CapCut |
| **Animado** (sección "Track animado") | Pixar, claymation, Wes Anderson, sci-fi, Apple; producto difícil de enseñar con persona; marca sin cara | ChatGPT + NotebookLM → Nano Banana Pro → Kling 3 → CapCut |

Si el usuario no lo dice, preguntarlo antes de generar nada: es la decisión que condiciona todo lo demás.

**Lo que comparten:** el resultado se decide en la planificación (≈80 %), todo en 9:16 y 2K, ApiMart/KIE como
acceso barato a los modelos, ElevenLabs para la voz y CapCut gratuito con transiciones Mix.

---

## Cuándo leer cada referencia

Este archivo es el mapa. El detalle vive en `references/`; leer solo lo que pide la etapa en curso.

| Archivo | Leerlo cuando |
|---|---|
| `references/proceso.md` | Hace falta el paso a paso completo de una fase, o las variantes de montaje por formato |
| `references/practicas.md` | Hay que decidir algo (qué modelo, si hace falta character sheet, qué modo de quitamarcas) o revisar el resultado |
| `references/prompts.md` | Se va a escribir un prompt: menús de cámara, micro-acción, voz, acento y plantillas de imagen |
| `references/ejemplos.md` | Se busca un caso análogo ya resuelto, con sus guiones y recuentos reales |

`assets/` contiene las plantillas listas para rellenar. Copiarlas, no reescribirlas de memoria:
`prompt-imagen.md`, `prompt-clip.md`, `brief-estratega.md` y `checklist-edicion.md` son del track
realista; `cadena-animados.md` es la hoja de ruta completa del track animado. `direccion-clip.md` es la
única plantilla que **no sale del curso** (va marcada `[ANEXO]`): la biblia de continuidad y la ficha de
dirección por clip que se rellenan entre el guion y la imagen.

---

## Track realista · etapas 1-6

**La regla que gobierna este track: imagen primero, vídeo después.** Nunca texto → vídeo. Todo el control del
realismo está en la fase de imagen.

---

## Etapa 1 · Estrategia

Antes de generar nada, fijar **una** cosa: el ángulo.

1. **Ángulo** — a quién le hablas y desde qué dolor entras. Es ≈80 % del resultado.
2. **Oferta** — qué le das.
3. **Creatividad** — hook, edición, música. Amplifica; no salva un mal ángulo.

**Un ángulo por vídeo.** Del mismo producto salen 12 anuncios distintos sin tocar el producto.

Cruzarlo con el nivel de conciencia del espectador:

| Nivel | Qué toca hacer |
|---|---|
| 1 · Inconsciente | Historia. **No vender** |
| 2 · Consciente del problema | Remover el dolor, enseñar que hay salida |
| 3 · Consciente de la solución | Explicar el mecanismo señalando un culpable |
| 4 · Consciente del producto | Prueba social, **un vídeo por objeción** |
| 5 · Súper consciente | Oferta, urgencia, garantía |

**En Meta el tráfico es frío: priorizar 1-3.** Lanzar oferta a nivel 1 es el error más caro.

→ Detalle y los 12 ángulos: `references/practicas.md` § Estrategia y `references/ejemplos.md` § 10.

## Etapa 2 · Guion

Estructura fija: **clip 0 (hook) → problema → agitación → mecanismo → demostración → beneficio → CTA**.

Cada clip lleva tres campos: **rótulo en pantalla · visual · guion**.

Con el agente El Estratega (ver `assets/brief-estratega.md`): basta una frase vaga del producto y otra del
avatar. Cuando proponga ángulos, responder *"elige los tres mejores"*.

**El guion es lo importante de cada clip; la parte visual es negociable.** La parte visual alimenta el prompt
de imagen; el guion alimenta el prompt de vídeo.

Verificar siempre ingredientes, precios y beneficios que escriba el agente: los inventa plausibles.

## Etapa 2.5 · Dirección [ANEXO · no es del curso]

Antes de escribir un solo prompt, decidir. **Esta etapa no sale del curso**: el curso pasa del guion a la imagen
y resuelve lo visual sobre la marcha. Es una capa añadida y va marcada como tal; si choca con algo de
`references/`, manda `references/`.

Rellenar `assets/direccion-clip.md`, que produce dos cosas:

- **una biblia de continuidad** por anuncio — avatar, vestuario, set, luz, cámara base, voz, energía y las
  **3-5 anclas de consistencia**. Se escribe una vez, antes del primer clip, y no se renegocia. Es lo que impide
  que el avatar derive entre el clip 2 y el clip 5;
- **una ficha por clip** — función, guion literal, si habla, duración medida contra el guion, si reutiliza la
  imagen anterior, encuadre, movimiento, micro-acción ya en inglés y entre corchetes, continuidad y salida.

Antes de preguntar nada al usuario, clasificar: **CRÍTICO** (sin eso no se genera: foto de referencia, si habla o
hay voz en off, si se manipula producto, formato) se pregunta; **IMPORTANTE** se propone con un valor por
defecto; **OPCIONAL** se decide sin consultar. Preguntar siempre con opciones cerradas y una recomendación.

Los tres límites: **no** escribe el prompt de imagen (eso es el 6C de la etapa 3), **no** escribe el prompt del
clip (esa es la fórmula de la etapa 4), **no** toca el guion.

→ Qué no importar de un director al uso: `references/practicas.md` § Anexo · dirección entre guion e imagen.

## Etapa 3 · Imagen

**Nunca imaginar el avatar de cero.** Partir de la foto de una persona real (Pinterest, TikTok, Instagram).

1. Describir la referencia con el método **6C**: Character · Camera · Clothing · Context · Cinematic Light ·
   Consistency Anchors.
2. Generar con **Nano Banana Pro** o **GPT Image 2**. Con referencia, elegir la entrada **imagen a imagen**.
3. **Siempre 9:16 y calidad 2K.** Las imágenes que se van a superponer en edición, en **1:1**.

**En todo prompt con dos referencias** hay que decir cuál es la imagen 1 y cuál la 2, y prohibir
explícitamente traerse a la persona de la 2. Sin esa frase el modelo mezcla las dos caras.

**Diseñar el avatar contra la limitación del modelo**: Omni añade una capa sutil de textura de piel al animar.
Piel impoluta + esa textura = canta a IA. Buscar el avatar **más humano e imperfecto**, no el más guapo.

**Character sheet**: solo si el avatar aparece de cuerpo entero, gira, o el formato tiene muchos ángulos
(moda, voz en off). Para busto parlante no hace falta.

**En moda, el orden del pipeline importa**: `avatar → cuerpo entero → pared blanca → outfit 1 → outfit 2 …`,
cada outfit sobre el resultado anterior. Saltarse la pared blanca hace que los outfits hereden el fondo original.

**Una imagen por estado**, encadenadas: cada prompt edita la anterior con `Keep everything exactly the same`,
la lista explícita de lo que no cambia, y `the next frame of the same video`. Para producto de marca añadir
`without changing the branding, colors, typography, or label`.

→ Plantillas: `assets/prompt-imagen.md`. Catálogo completo: `references/prompts.md` §§ 6-9.

## Etapa 4 · Clips

Estructura del prompt: **CÁMARA + MOVIMIENTO + MICRO-ACCIÓN + GUION + VOZ + ACENTO**.
Prompts en inglés; el guion, en español.

**Reparto de modelo — por clip, no por proyecto:**

- **El avatar habla → Omni Flash.**
- **El avatar no habla → Grok Imagine 1.5** (~0,048 US$ por clip de 6 s a 720p).

Reglas al escribir:

- **Micro-acciones incrustadas en el guion**, entre corchetes y en inglés, en el punto exacto de la frase.
- `While speaking, …` para que ocurran durante el habla; `while saying in the first 3 seconds of the video`
  para acotarlas.
- **Cámara estática obligatoria si hay manipulación de producto.**
- **`NO TALKING` en todo clip sin guion.**
- **Coreografiar el gesto con la superposición**: si señala arriba a la derecha, ahí va la imagen en edición.
- `Photorealistic, realistic hands` cuando manipula objetos.
- **Acento**: el latino neutro sale solo; el de España hay que pedirlo siempre.

**Duración**: se mide el guion (4/6/8/10 s). Corto → 6 s, largo → 8 s. Mejor pasarse y recortar.
**En Grok, 720 y nunca 480: cuesta lo mismo.**

→ Plantilla y menús: `assets/prompt-clip.md`. Catálogo completo: `references/prompts.md` §§ 1-5, 10-11.

## Etapa 5 · Limpieza

Los clips de Flow con plan Pro salen con marca de agua; los de ApiMart, no.

Dos modos de quitamarcas. **Empezar siempre por la recomendada/avanzada.** El criterio es **el fondo detrás
de la marca**: complejo (gente, estampados) → avanzada; estático → general. Esperar a la detección automática
antes de tocar nada. Reprocesar con el otro modo si no convence es flujo normal.

## Etapa 6 · Montaje en CapCut

Seis pasos, en orden:

1. Importar clips e imágenes de superposición.
2. Ordenar en la timeline.
3. **Cortar los espacios muertos** del final de cada clip.
4. **Subir la velocidad clip a clip, de oído: 1.12–1.20.** La IA habla demasiado lento; es sistemático.
5. **Capa de realismo** de punta a punta.
6. Música y efectos.

**Capa de realismo — valores exactos** (Ajuste → Basic), el paso con más impacto de toda la edición:

| temp | tint | saturation | exposure | contrast | highlight | shadow | fade |
|---|---|---|---|---|---|---|---|
| -3 | 2 | -6 | -3 | 12 | -35 | 18 | 6 |

Se configura una vez y se guarda con **Save as preset**.

Otras reglas: transiciones **solo Mix** · superponer detrás del avatar = duplicar clip + quitar fondo (Pro)
**y bajar el volumen** · animaciones Zoom/Shake/Slide Up · rótulo fijo de retención · zoom falso con
fotogramas clave (rombo en *Escalar*, 100 % → 150 %).

→ Checklist: `assets/checklist-edicion.md`. Variantes por formato: `references/proceso.md` § Fase 7.

---

## Los nueve formatos del track realista

| Formato | Producción típica | Lo que cambia |
|---|---|---|
| UGC sin producto | 1 avatar + imágenes antes/después (1:1) · 4 Omni | Montaje de referencia: Mix, superposiciones, animaciones |
| UGC con producto | 1 imagen por estado · 3 Omni + 1 Grok | El más simple: rótulo fijo, sin transiciones |
| Moda | Avatar + sheet + 1 imagen por outfit · 3 Omni + 4 Grok | Inversión de planos: la pose ocupa el fotograma, el clip hablado va pequeño abajo a la derecha |
| App / SaaS | **1 imagen de avatar** + 2 pasos de pantalla · 3 Omni + screen recording | Avatar solo → logo → app a pantalla completa con el avatar en esquina |
| Podcast | 2 avatares, encuadres distintos · 1 clip por intervención | **Apilar los clips solapándolos** para cortar antes de que el otro acabe |
| Dualcast | **1 imagen** con las dos personas · 4 Omni | **Doble bloque de micro-acción**, `LEFT`/`RIGHT` en mayúsculas |
| Voz en off | Sheet + muchas imágenes · Grok + ElevenLabs | **Todas las imágenes primero.** Recortar clips a 2-3 s; **manda el audio** |
| Trend viral | Igual que voz en off | El TikTok va en la pista principal y su música sostiene el anuncio |
| Imágenes estáticas | Agente → 7 prompts → ApiMart | No hay montaje |

**Trampas propias de cada formato:**

- **Podcast** — el segundo interlocutor se crea con un prompt que además **adapta el fondo** (misma habitación,
  encuadre distinto). Duplicar la imagen y voltearla queda raro porque el fondo es idéntico. La cámara **nunca
  se mueve** y las micro-acciones son **reacciones del que escucha**. Compensa generar clips de dos palabras
  solo para el *reaction shot*.
- **Dualcast** — sin el segundo bloque de micro-acción, el modelo hace hablar a los dos o congela al que
  escucha.
- **Voz en off** — todas las imágenes antes de animar nada, y estética de móvil (`no cinematic grading`), no
  cinematográfica.
- **App / SaaS** — la pantalla se hace en **dos pasos**: primero el avatar sosteniendo el dispositivo con la
  pantalla **negra apagada**, después un segundo prompt que incrusta la captura encima. En un solo prompt el
  modelo se inventa la interfaz. Plantillas: `assets/prompt-imagen.md` § App o software.
- **Producto difícil** (abrir un bote, extender crema) — la IA falla en los dos. Se resuelve adjuntando una
  segunda referencia del mecanismo de apertura, y pidiendo que la cantidad visible de crema **decrezca**
  durante el clip.
- **Imágenes estáticas** — sustituir el marcador `marca` por el nombre real antes de generar.

→ Procedimiento de cada uno: `references/proceso.md` § Fase 7. Casos resueltos: `references/ejemplos.md`.

## Antes de dar por bueno un vídeo (track realista)

- [ ] Un solo ángulo, coherente con el nivel de conciencia elegido.
- [ ] Avatar imperfecto, salido de una referencia real.
- [ ] Cada clip sin guion lleva `NO TALKING`.
- [ ] Los clips hablados van en Omni; los mudos, en Grok a 720.
- [ ] Cada gesto que señala fuera de plano tiene su superposición en el montaje.
- [ ] Espacios muertos cortados y velocidad entre 1.12 y 1.20.
- [ ] Capa de realismo aplicada de punta a punta con los ocho valores exactos.
- [ ] Volumen bajado en los clips duplicados de las superposiciones.
- [ ] Rótulo fijo de retención en pantalla.
- [ ] Marca de agua eliminada si salió de Flow.

→ Lista completa de errores caros: `references/practicas.md` § Errores que salen caros.

---

## Track animado

Otro método, no una variante del anterior. **No hay avatar hablando, ni Omni, ni Grok, ni capa de realismo.**
Cada clip es una **transición animada entre dos imágenes**, no un plano generado de cero.

→ Hoja de ruta para ejecutarlo: `assets/cadena-animados.md`. Los 13 prompts literales: `references/prompts.md`
§ 13. Paso a paso: `references/proceso.md` § Track Animados.

### Etapa A1 · Planificación · 8 prompts encadenados

Una sola conversación de ChatGPT de principio a fin, en orden, sin saltarse ninguno. Al llegar al 7 el contexto
completo ya está dentro y se audita sin reexplicar nada.

| # | Prompt | Dónde | Devuelve |
|---|---|---|---|
| 1 | Avatar + research | ChatGPT | Avatar + 3 búsquedas para NotebookLM |
| 2 | Auto-research + insights | **NotebookLM** | 5 insights con cifras reales |
| 3 | Ángulos | ChatGPT | 3 ángulos, uno por dolor → elegir uno |
| 4 | Guion | ChatGPT | El guion |
| 5 | Storyboard | ChatGPT | Estructura y metáfora visual |
| 6 | Prompts de imagen | ChatGPT | Prompts con bloque **Style Lock** |
| 7 | Auditoría completa | ChatGPT | Guion definitivo + 2 variantes + todo auditado |
| 8 | Introducción al producto | ChatGPT | Lo anterior con la marca real |

Las tres trampas del método, por orden de frecuencia:

- **El Prompt 2 va en NotebookLM, no en ChatGPT.** Es el único que cambia de herramienta. En GPT devuelve
  cifras inventadas en vez de datos de las fuentes.
- **En el Prompt 6, dejar un solo estilo en el Style Lock.** Con varios, las imágenes salen incoherentes.
- **El estilo se elige en el Prompt 1**, junto al producto y el mercado. Cambiarlo a mitad invalida guion,
  storyboard y prompts.

En NotebookLM: cuaderno nuevo → *Discover Sources* → las tres búsquedas **una a una**, esperando a que cada una
termine → Importar. No acepta prompts largos: son búsquedas cortas tipo Google.

**Iterar es parte del método.** El punto donde más se itera es el storyboard. *"La IA hace el 80 % del trabajo;
ese 20 % —el criterio, el ojo humano— es lo que hace que el anuncio sea bueno o no."*

### Etapa A2 · Producción

**Imágenes** — Nano Banana Pro vía **ApiMart (0,05 US$/img)** o KIE (0,09 US$). Texto a imagen, **9:16**,
**2K siempre** (1K cuesta lo mismo). Varias pestañas en paralelo. Producto real → imagen de referencia.
**Nombrarlas `P1`, `P2`, `P3`… por número de prompt**: es lo único que mantiene el orden de los pares.

**Clips** — ApiMart → **Kling volumen 3**, 720p, 9:16. Cambiar el modo de «base» a **«Future»** y subir la
**primera y la última imagen** del par. Duración **3-5 s** (el curso usa 4). El prompt sale del menú de estilos
—Realista/Apple, Sci-fi, Pixar, Claymation, Wes Anderson— y **todos terminan en `sound effects (no talking)`**,
el equivalente animado del `NO TALKING` del track realista.

**Clips = imágenes − 1.**

**Voz** — ElevenLabs. Voz del catálogo → **Multilingual V2**; voz clonada propia → **V3**. No es intercambiable.

### Etapa A3 · Montaje

Arrastrar clips y voz a CapCut, **colocando el audio primero** y montando contra él.

| Velocidad | Transición | Duración transición | Música | SFX de los clips | Voz |
|---|---|---|---|---|---|
| **1,20** (1,20-1,30) | **Mix**, aplicar a todas | **0,5-0,7 s** | **−25 a −30** | **−8** | **+5** |

Quitar los silencios largos de la narración; balancear clip a clip de oído al final.
**Aquí no se aplica la capa de realismo**: es del track realista y en un anuncio animado sobra por definición.

### Antes de dar por bueno un vídeo (track animado)

- [ ] El Prompt 2 se pegó en NotebookLM.
- [ ] Un solo estilo en el Style Lock.
- [ ] Todas las imágenes en 9:16 y 2K, nombradas P1…Pn.
- [ ] Cada clip es una transición entre dos imágenes consecutivas, en modo «Future».
- [ ] Todos los prompts de clip terminan en `sound effects (no talking)`.
- [ ] Velocidad 1,20 · Mix 0,5-0,7 · música −25/−30 · SFX −8 · voz +5.
- [ ] El storyboard se iteró al menos una vez.

---

## Stack y costes

| Función | Herramienta |
|---|---|
| Generación barata | **Google Flow** — la imagen cuesta 0 créditos, solo el vídeo consume; el plan Pro **saca marca de agua** |
| Pago por uso | **ApiMart** — 10 créditos = 1 US$, mínimo 1 US$, sin marca de agua, admite generaciones en paralelo |
| Alternativa | **Kie** — igual, mínimo 5 US$ |
| Edición | **CapCut gratuito** — solo quitar el fondo exige Pro |
| Voz en off | **ElevenLabs** — 10.000 créditos gratis/mes |
| Música y SFX | Biblioteca AvatarHype (392 pistas) o **Epidemic Sound** — 30 días gratis |

Precios por modelo que cita el curso: Grok Imagine 1.5 ~**0,048 US$** por clip de 6 s a 720p · Nano Banana Pro
**0,05 US$/imagen en ApiMart** y **0,09 US$ en KIE**. Como referencia de lo que evita el método, HeyGen,
Freepik, Arcads, Wavy y Higgsfield parten de **0,15 US$/imagen**.

---

## Procedencia

Consolidado de 28 lecciones de dos cursos de la academia: **Avatar Hype Academy** (26 lecciones, track
realista, referencias `[M1-*]` a `[M4-*]`) y **Creativos Animados** (2 lecciones, track animado, `[M6-*]`).
Las referencias entre corchetes apuntan a la lección de origen en `sources/`.

**Todo lo marcado `[ANEXO]` no sale del curso**: la Etapa 2.5 y `assets/direccion-clip.md`. Es una capa añadida
para cerrar la costura entre el guion y la imagen, y por eso no lleva citas. Si contradice algo citado con
`[M…]`, manda lo citado.

Huecos conocidos: `4.7-ugly-ads` no tiene contenido publicado, así que ese formato no está cubierto. El curso
de Creativos Animados **se está regrabando entero** (aviso del propio curso): el track animado es una foto a
2026-09-03 y los nombres de algunos controles de interfaz pueden haber cambiado.

Los cuatro archivos de `references/` son copias de `knowledge/avatarhype/`. Para refrescarlos tras editar la
consolidación: `cp knowledge/avatarhype/{proceso,practicas,prompts,ejemplos}.md skills/avatarhype/references/`
