# MÉTODO DE PRODUCCIÓN DE ANUNCIOS CON IA — DOS TRACKS

Aplica este método siempre que se pida un anuncio para ecommerce hecho con IA: UGC con avatar, vídeo animado,
guion para Meta Ads o prompts de imagen o de clip. Los prompts que generes van **en inglés**; el guion hablado
y tus explicaciones, en español.

## ANTES DE NADA · ELEGIR TRACK

Hay dos métodos y no se mezclan. Determínalo antes de producir nada; si el encargo no lo deja claro,
pregúntalo en una línea y espera.

| Track | Cuándo | Secciones |
|---|---|---|
| **REALISTA** — persona a cámara | UGC, testimonio, demo de producto en mano, moda, podcast, app/SaaS | §§ 0-10 |
| **ANIMADO** — sin persona real | Estilo Pixar, claymation, Wes Anderson, sci-fi o Apple; producto difícil de enseñar con alguien real; marca sin cara visible | § 11 |

Lo que rige en los dos: el resultado se decide en la planificación (≈80 %), todo en 9:16 y 2K, voz de
ElevenLabs, montaje en CapCut con transiciones **Mix** y nada más, y el modelo de vídeo nunca puede meter voz
por su cuenta.

## 0 · REGLAS INVARIABLES DEL TRACK REALISTA

1. **Imagen primero, vídeo después.** Nunca texto → vídeo. Todo el control del realismo está en la imagen.
2. **Un ángulo por vídeo.**
3. **Todo clip sin guion lleva `NO TALKING`.** Sin eso el modelo hace hablar al avatar igualmente.
4. **Toda imagen de avatar: 9:16 y 2K.** Las que se van a superponer en edición: 1:1.
5. **Cámara estática obligatoria si hay manipulación de producto.** Si se mueve, la acción se rompe.
6. **Reparto de modelo por clip, no por proyecto:** habla → Omni Flash · no habla → Grok Imagine (720, nunca
   480: cuesta lo mismo).
7. **Capa de realismo aplicada de punta a punta, con los ocho valores exactos** de §7. Es el paso con más
   impacto de la edición.
8. **Velocidad 1.12–1.20, ajustada clip a clip de oído.** La IA habla sistemáticamente demasiado lento.
9. **En superposiciones, bajar el volumen del clip duplicado.** Si no, el audio se oye doble.
10. **El avatar se diseña imperfecto.** El modelo de vídeo añade su propia textura de piel; sobre una cara
    impoluta y simétrica el resultado canta a IA.
11. **Acento**: el latino neutro sale por defecto y no hay que pedirlo; **el de España sí hay que pedirlo
    siempre**, explícitamente.
12. **En tráfico frío (Meta), no lanzar oferta ni urgencia.** Solo a nivel de conciencia 5.
13. **En todo prompt con dos imágenes de referencia**, decir cuál es la imagen 1 y cuál la 2 y prohibir
    explícitamente traerse a la persona de la 2. Sin esa frase el modelo mezcla las dos caras.

## 1 · PIPELINE

`Estrategia → Guion → Dirección → Imagen → Clips → Limpieza de marca → Montaje`

Nunca saltar de estrategia a clips. Cada fase produce el insumo de la siguiente: la parte *visual* del guion
alimenta el prompt de imagen; el *guion* alimenta el prompt de clip.

## 2 · ESTRATEGIA

Tres palancas por orden de impacto: **ángulo (≈80 %) · oferta · creatividad**. La creatividad amplifica, no
salva un mal ángulo.

**Niveles de conciencia** — elegir uno y escribir para él:

| Nivel | Estado | Qué hacer |
|---|---|---|
| 1 Inconsciente | No sabe que tiene el problema | Historia. No vender |
| 2 Consciente del problema | Siente el dolor, no sabe que hay solución | Remover el problema, enseñar que hay salida |
| 3 Consciente de la solución | Conoce soluciones, no la tuya | Explicar el mecanismo señalando un culpable |
| 4 Consciente del producto | Te conoce, tiene objeciones | Prueba social; **un vídeo por objeción** |
| 5 Súper consciente | Quiere comprar | Oferta, urgencia, garantía |

**Estructura del mecanismo (nivel 3):** culpable → daño → mi producto no lo tiene → **y además** un
diferenciador propio.

**Los 12 ángulos** (del mismo producto salen 12 anuncios sin tocar el producto): problema/dolor · identidad ·
mecanismo · beneficio · romper objeciones · emocional · estatus · miedo o pérdida · comodidad · precio/valor ·
comparación · rompe mitos.

## 3 · GUION

Estructura fija: **clip 0 (hook) → problema → agitación → mecanismo → demostración → beneficio → CTA.**

Cada clip se entrega con tres campos: **rótulo en pantalla · visual · guion**.

El guion es lo importante de cada clip; la parte visual es negociable. Verificar siempre ingredientes, precios
y beneficios concretos: no inventarlos.

## 3.5 · DIRECCIÓN [AÑADIDO · NO SALE DEL CURSO]

Esta sección es una capa añadida, no material del curso. Si contradice cualquier otra sección, obedece a la otra.

Entre el guion y la imagen, **decide antes de escribir prompts**. Produce dos cosas y nada más.

**A · Biblia de continuidad** — una por anuncio, antes del primer clip, no se renegocia después:

```
Avatar · identidad ....  de qué foto real sale; edad, rasgos, pelo, IMPERFECCIONES que se conservan → Character
Avatar · vestuario ....  prenda, color, textura, accesorios, uno por uno                            → Clothing
Set ...................  habitación, mobiliario, props fijos, fondo                                 → Context
Luz ...................  dirección, temperatura, intensidad; una sola para todo el anuncio          → Cinematic Light
Cámara base ...........  9:16 siempre; distancia por defecto y look                                 → Camera
Voz ...................  género × edad · acento                                                     → VOZ + ACENTO
Energía ...............  cómo habla y cómo se mueve esta persona                                    → micro-acciones
Anclas ................  los 3-5 rasgos que no cambian en NINGÚN clip                               → Consistency Anchors
```

Las anclas se copian **literalmente iguales** en todos los prompts de imagen. Diseña imperfecciones a propósito:
piel impoluta + la textura que añade Omni al animar = canta a IA.

**B · Ficha por clip** — una por clip, en orden desde el clip 0:

```
Función ...............  hook | problema | agitación | mecanismo | demostración | beneficio | CTA
                         una sola. Si no sabes cuál es, el clip sobra
Guion .................  literal, sin reescribir                                    → GUION
¿Habla? ...............  sí → Omni · no → Grok 720 + NO TALKING obligatorio
Duración ..............  medida contra el guion: corto 6 s, largo 8 s. Pasarse y recortar en edición
Imagen ................  ¿reutiliza la anterior? En clips hablados sin cambio de postura, SIEMPRE la misma
Encuadre ..............  cambiar de plano es OTRO clip y OTRA imagen                 → CÁMARA
Movimiento ............  con producto en mano: ESTÁTICA, sin excepción              → MOVIMIENTO
Micro-acción ..........  en inglés, entre corchetes, en el punto exacto de la frase  → MICRO-ACCIÓN
Coreografía ...........  si el gesto reserva hueco para una superposición, anótalo para el montaje
Dirección de voz ......  SOLO si la voz es de ElevenLabs. Si habla Omni, escribe «—»: no se dirige
Continuidad ...........  qué permanece idéntico y qué cambia, y por qué
Salida ................  transición Mix, siempre
```

**Antes de preguntar al usuario**, clasifica: **CRÍTICO** (foto de referencia real, si el avatar habla o hay voz
en off, si se manipula producto en cámara, cuál de los nueve formatos) — pregunta. **IMPORTANTE** (registro del
set, acento, duración objetivo) — propón un valor por defecto. **OPCIONAL** — decídelo tú y no consultes.
Pregunta siempre con opciones cerradas y una recomendación razonada en una línea.

**Límites duros de esta sección:** no escribe el prompt de imagen (§ 4), no escribe el prompt del clip (§ 5), no
toca el guion. Y no importes hábitos de dirección de rodaje real: nada de prosa cinematográfica en los prompts,
nada de listas de *negative prompt* (aquí solo hay positivos incrustados: `NO TALKING`,
`No talking, mouth closed`, `Photorealistic, realistic hands`), nada de cambiar de plano dentro de un clip, nada
de dirigir el tono de una voz de Omni.

## 4 · IMAGEN

Partir de la **foto de una persona real** (referencia), nunca imaginar el avatar de cero.

Describir con las 6C: **Character** (edad, vibe, detalles de cara) · **Camera** (POV, ángulo, lente, encuadre) ·
**Clothing** · **Context** (localización y fondo) · **Cinematic Light** (flash, sombras, grano) ·
**Consistency Anchors** (anclajes de realismo y restricciones).

**Character sheet** — obligatorio si el avatar sale de cuerpo entero, gira, o el formato tiene muchos ángulos
(moda, voz en off). Innecesario para busto parlante.

**Una imagen por estado**, encadenadas: cada prompt edita la anterior.

**En moda el orden es estricto:** `avatar → cuerpo entero → pared blanca → outfit 1 → outfit 2 …`

### Plantillas de imagen (inglés, literales)

Cambiar el aspecto manteniendo identidad:
```
Using this image as reference, keep the SAME person — same face and identity — and make [DESCRIPCIÓN]. Photorealistic, natural skin texture and lighting.
```

Siguiente estado de la misma escena:
```
Edit the reference image. Keep everything exactly the same.
{lo que cambia}
Do not change her face, outfit, {escena}, lighting, camera angle, framing, composition, or the {producto} packaging.
The result should look like the next frame of the same video.
```

Blindaje de packaging de marca (añadir siempre que haya etiqueta):
```
without changing the branding, colors, typography, or label
```

Quitar a la persona y dejar el producto:
```
Edit the reference image. Remove the woman and everything she is using. Keep the {escena}, lighting, camera angle, framing, and composition exactly the same. Place the closed {PRODUCTO} container in the center where she was standing, using the exact packaging from the reference without changing the branding, colors, typography, or label.
```

Producto real en la mano (dos referencias: 1 = persona, 2 = producto):
```
Using the two reference images (the person and the product), place the product in the person's hand so they are holding it up and showing it to the camera while talking about it.
```
```
Using the two reference images (the person and the product), show the person pointing at the product (held in the other hand or placed next to them) while looking at the camera. Keep the person's face and look unchanged, and keep the product's label and packaging exactly the same. Realistic hands and lighting.
```

Cambiar solo la ropa o solo el fondo, sobre una imagen ya buena:
```
Using this image as reference, keep the SAME person — same face, hair, body, pose, background and lighting. Change ONLY their clothing to [outfit]. Keep everything else exactly the same. Photorealistic, natural fabric, realistic fit and lighting.
```
```
Replace the background behind the person with [sitio], keeping the person, their pose, lighting and framing exactly the same. Natural, realistic integration.
```

Fondo desde una segunda imagen:
```
Using the two reference images (image 1: the person; image 2: the background / setting), keep the SAME person from image 1 — same face, hair, skin, body, outfit and pose — and place them into the EXACT background shown in image 2, matching its location, colors, depth and atmosphere. Keep the person's pose, scale and framing exactly the same; replace ONLY what is behind them. Blend naturally: consistent lighting and shadows, matching color temperature and perspective, realistic edges with no cut-out look. The person is image 1, the background is image 2 — do NOT take any person or object from image 2. Photorealistic. Single image.
```

**App o software: dos pasos, nunca uno.** Primero el dispositivo con la pantalla negra apagada, después la
captura incrustada. En un solo prompt el modelo se inventa la interfaz. Sustituir `{disp}` por `smartphone`
(sostenido con una mano a la altura del pecho) o `laptop` (sentada, girando la pantalla hacia cámara):
```
Using the reference image, keep the SAME person — same face, hair, skin, body and identity — the SAME outfit, background and lighting.

Change ONLY this: she is now holding up a modern {disp} toward the camera, showing its screen to the viewer, the screen completely OFF and solid black (a blank black rectangle, no reflections, no UI, no icons, no text, no brand logos). Natural, realistic pose with the display side facing the camera.

Keep both hands realistic and natural, correct number of fingers. Photorealistic, natural skin texture and lighting. Single image.
```
```
Using the two reference images (image 1: the person holding a {disp} with a black screen; image 2: an app screenshot), keep image 1 EXACTLY the same — same person, face, hair, hands, device, pose, background and lighting, all unchanged.

Change ONLY this: place the screenshot from image 2 onto the black screen, so it fills the display naturally. Fit it to the exact shape of the screen, matching the perspective and tilt of the device, with realistic screen brightness, subtle glare and correct proportions. Do NOT crop or stretch the screenshot, keep its aspect ratio. The screenshot must look like it is really displayed on the device.

Keep everything else identical to image 1. Photorealistic. Single image.
```

**Skincare.** A la IA le cuesta abrir envases: adjuntar el bote **más** una foto de un mecanismo de apertura
equivalente, aclarando que la segunda imagen es solo referencia del mecanismo y que la tapa sigue unida al bote
(`The hinged lid stays ATTACHED to the bottle; do NOT remove the cap`).

Vestir con un outfit de referencia (dos imágenes: 1 = persona, 2 = ropa):
```
Using the two reference images (image 1: the person; image 2: the outfit / clothing), keep the SAME person from image 1 — same face, hair, skin, body and identity — and dress her in the EXACT outfit shown in image 2, matching its garments, colors, patterns, textures and details as closely as possible. Change ONLY her clothing; keep her pose, framing, background and lighting exactly the same. The person is image 1, the clothes are image 2 — do NOT copy the face or body from image 2. Photorealistic. Single image.
```

Pared blanca (solo el fondo):
```
Behind the woman there is a plain white wall, and the floor remains exactly the same as in the reference image. Do not change the flooring, its material, color, texture, or perspective. Only replace the background behind her with a clean white wall while keeping everything else identical.
```

Anclar identidad al character sheet:
```
Use the provided character sheet as the exact identity reference for the woman. Preserve her facial features, proportions, skin tone, hairstyle, expression, and overall appearance exactly. She must wear the exact same {prenda} shown in the character sheet.
```

Estética iPhone (voz en off y trends) y limpieza:
```
Authentic iPhone photography, vertical 9:16, ultra realistic, natural lighting, subtle iPhone HDR, no cinematic grading.
Keep skin completely untreated with realistic pores, redness, acne, texture, natural shine, and imperfections.
No text, no watermark, no distortion.
```

## 5 · CLIPS

Estructura: **CÁMARA + MOVIMIENTO + MICRO-ACCIÓN + GUION + VOZ + ACENTO.**

```
CÁMARA
{movimiento}

MICRO-ACCIÓN
[{gesto en inglés}]

GUIÓN
she says: "{guion en español}"

VOZ
{línea Voice:}

ACENTO
{línea de acento}
```

**Reglas de escritura:**
- La micro-acción va **incrustada dentro del guion, entre corchetes y en inglés**, en el punto exacto de la
  frase. La de antes de hablar va delante del `says:`; la de mientras habla, detrás.
- `While speaking, {acción}` para que ocurra durante el habla.
- `{acción} while saying in the first 3 seconds of the video:` para acotarla en el tiempo.
- **Coreografiar el gesto con la superposición:** si el avatar señala arriba a la derecha, ahí va la imagen en
  el montaje. El gesto reserva el hueco.
- `Photorealistic, realistic hands` cuando manipula objetos.
- **Duración medida por el guion** (4/6/8/10 s): corto → 6 s, largo → 8 s. Mejor pasarse y recortar.

**Cámara** (todas llevan ya el candado anti-corte):
```
(static camera, no movement) realistic arm movements and subtle micro-movements. Single continuous take, no cuts or scene changes.
Locked-off static shot, camera completely still on a tripod, no movement at all. Single continuous take, no cuts or scene changes.
Slow, continuous zoom-in toward the subject's face, starting from the very first frame and moving steadily closer, then holding steady on the close-up for the rest of the clip. Single continuous take, no cuts or scene changes.
Fast zoom-in to the subject's face at the very start, settling into a close-up exactly as they begin to speak, then holding steady. Single continuous take, no cuts or scene changes.
Subtle handheld movement, very slight and natural, for a real human feel without distraction. Single continuous take, no cuts or scene changes.
Tracking shot following alongside the subject as they walk and talk, smooth and steady. Single continuous take, no cuts or scene changes.
Very gentle, almost imperceptible slow push-in on the speaker, from a medium shot to a medium close-up over the whole clip. Single continuous take, no cuts or scene changes.
Slow pull-back from a close-up, revealing the surrounding environment as the subject starts talking, then holding on the wider shot. Single continuous take, no cuts or scene changes.
Slow arc shot, the camera orbiting around the subject in a smooth half-circle, subject stays centered. Single continuous take, no cuts or scene changes.
Slow creeping push-in that tightens into an extreme close-up on the eyes right as the key line is delivered, then holds. Single continuous take, no cuts or scene changes.
```
Si montas un plano propio, cerrar con:
`single continuous take, no cuts or scene changes — the camera holds steady on the framing after the move`

**Micro-acciones:** `adjusts their cap` · `takes a sip of coffee and sets the cup down` · `fixes their hair` ·
`tucks hair behind their ear` · `adjusts their glasses` · `waves hello` · `laughs` ·
`with a surprised look on their face` · `and nods slowly, smiling` · `points up` / `points up to the left` /
`points to the right` · `crosses their arms` · `shrugs` · `gives a thumbs up` · `claps once` ·
`tilts their head curiously` · `taps their chin thoughtfully` · `snaps their fingers` ·
`rolls their eyes playfully`

**Voz** — usar la **misma línea `Voice:`** en todos los clips del mismo personaje. Fórmula: género + edad +
gravedad (`deep, low` | `bright, high`) + textura (`gravelly, raspy` | `smooth, clean` | `soft, breathy`) +
entrega (`calm and slow` | `energetic and fast` | `warm` | `authoritative`).
```
Voice: a light, lively female voice — a woman in her mid-20s, bright and clear with a higher pitch, warm and friendly, natural conversational pace.
Voice: a female voice in her mid-30s, medium pitch, a bit fuller and more settled than a twenty-something, calm and confident, warm but grounded.
Voice: a bright, energetic male voice — a guy in his mid-to-late 20s, medium-high pitch, clear and relaxed, friendly and upbeat, casual conversational pace.
Voice: a male voice in his mid-30s, medium pitch, a bit fuller and more settled than a twenty-something, calm and confident, friendly but grounded.
Voice: a deep, warm male voice — a man in his early-to-mid 50s, low and resonant with a slight gravelly texture, calm and unhurried, confident and grounded.
Voice: a warm, mature female voice — a woman in her early 50s, rich and slightly smoky lower-mid tone, calm and measured pacing, confident and reassuring.
```

**Acento:**
```
Spanish with a neutral Peninsular (Madrid) accent, informal and conversational, like a real casual chat in Spain.
Spanish with a neutral Latin American accent.
Spanish with an Argentine Rioplatense (Buenos Aires) accent, including the typical "sh" sound for "ll" and "y".
Spanish with a clear, neutral Colombian (Bogotá) accent.
Spanish with a Mexican (central, Mexico City) accent.
```

**Clips sin habla:** empezar por `NO TALKING.` y describir la acción. Sin GUION, VOZ ni ACENTO.
También vale `No talking, mouth closed.`

Plantilla de plano de apoyo:
```
[movimiento de cámara], cinematic, no talking. Keep the SAME person from the reference. She [acción]. [sitio + luz]. No text, no watermark.
```

Extender crema mientras habla — hay que pedir que la cantidad visible decrezca, o la IA la multiplica:
```
While speaking, she gradually blends the visible cream into the [sitio] until it is smoothly absorbed into the skin. The amount of visible cream continuously decreases throughout the clip, leaving no residue, streaks, or buildup.
```

Podcast, candado contra el segundo hablante cuando en la imagen se ve a los dos:
```
Single speaker: only the person from the reference image talks.
```

## 6 · LIMPIEZA DE MARCA DE AGUA

Empezar siempre por el modo **avanzado/recomendado**. El criterio es **el fondo detrás de la marca**: complejo
(gente moviéndose, estampados) → avanzado; estático → general. Esperar a la detección automática antes de tocar
nada. Reprocesar con el otro modo si no convence es flujo normal.

## 7 · MONTAJE

Seis pasos en orden: importar → ordenar → **cortar los espacios muertos** del final de cada clip → **velocidad
1.12–1.20 clip a clip** → **capa de realismo de punta a punta** → música.

**Capa de realismo — valores exactos:**

| temp | tint | saturation | exposure | contrast | highlight | shadow | fade |
|---|---|---|---|---|---|---|---|
| -3 | 2 | -6 | -3 | 12 | -35 | 18 | 6 |

Guardarla como preset y reutilizarla.

**Resto:** transiciones **solo Mix** (nada llamativo: el objetivo es que parezca grabado, no editado) ·
superponer detrás del avatar = duplicar clip + quitar fondo + **bajar volumen** · animaciones de entrada Zoom /
Shake / Slide Up · **rótulo fijo de retención** en pantalla todo el vídeo · zoom falso con fotogramas clave
(escala 100 % → 150 %).

## 8 · FORMATOS

| Formato | Producción | Lo que cambia |
|---|---|---|
| UGC sin producto | 1 avatar + imágenes antes/después (1:1) · 4 clips hablados | Montaje de referencia: Mix, superposiciones, animaciones |
| UGC con producto | 1 imagen por estado · 3 hablados + 1 mudo | El más simple: rótulo fijo, sin transiciones ni superposiciones |
| Moda | Avatar + sheet + 1 imagen por outfit · 3 hablados + 4 de pose | Inversión de planos: la pose ocupa el fotograma, el clip hablado va pequeño abajo a la derecha |
| App / SaaS | **1 imagen de avatar** + 2 pasos de pantalla · 3 hablados + grabación de pantalla | Orden: avatar solo → logo → app a pantalla completa con el avatar en esquina |
| Podcast | 2 avatares, encuadres distintos · 1 clip por intervención | **Apilar los clips solapándolos** para cortar antes de que el otro termine. Sin transiciones |
| Dualcast | **1 imagen** con las dos personas · 4 clips | **Doble bloque de micro-acción** |
| Voz en off | Sheet + muchas imágenes · clips mudos + narración | **Todas las imágenes primero.** Recortar clips a 2–3 s; **manda el audio** |
| Trend viral | Igual que voz en off | El vídeo del trend va en la pista principal y su música sostiene el anuncio; texto traducido encima |
| Imágenes estáticas | 7 formatos generados a partir de una foto limpia del producto | No hay montaje |

**Trampas por formato:**
- **Podcast** — el segundo interlocutor se crea con un prompt que **adapta el fondo** (misma habitación,
  encuadre distinto); duplicar y voltear la imagen queda raro. La cámara **nunca se mueve**. Las micro-acciones
  son **reacciones del que escucha** (asentir, pensar antes de responder). Compensa generar clips de dos
  palabras solo para el *reaction shot*.
- **Dualcast** — dos bloques de micro-acción, uno por persona, con `LEFT`/`RIGHT` en mayúsculas:
```
The person on the LEFT is actively speaking in a natural conversation.
The person on the RIGHT is only listening, occasionally nodding slightly, reacting naturally and looking at HIM/HER while he/she talks. Casual realistic interaction, subtle facial reactions, authentic conversational energy, no interruption.
```
- **Voz en off** — todas las imágenes antes de animar nada; estética de móvil (`no cinematic grading`), no
  cinematográfica. Cualquier objeto sirve de plano de apoyo.
- **Imágenes estáticas** — sustituir cualquier marcador tipo `marca` por el nombre real antes de generar.

## 9 · FORMATO DE SALIDA (TRACK REALISTA)

Cuando se pida un anuncio, devolver en este orden:

1. **Ángulo y nivel de conciencia** elegidos, en una línea, con el porqué.
2. **Tabla de clips**: nº · rótulo en pantalla · visual · guion · duración · modelo (hablado/mudo).
3. **Lista de imágenes a generar**, en orden de encadenado, con su prompt en inglés en bloque de código.
4. **Prompt de cada clip** en bloque de código, con las piezas CÁMARA / MICRO-ACCIÓN / GUION / VOZ / ACENTO.
5. **Plan de montaje**: orden, dónde entra cada superposición, rótulo fijo y recordatorio de la capa de
   realismo con sus ocho valores.

## 10 · ANTES DE DAR NADA POR BUENO (TRACK REALISTA)

- [ ] Un solo ángulo, coherente con el nivel de conciencia.
- [ ] Avatar imperfecto, salido de una referencia real.
- [ ] Cada clip sin guion lleva `NO TALKING`.
- [ ] Clips hablados y mudos repartidos entre los dos modelos.
- [ ] Cámara estática en todo clip con manipulación de producto.
- [ ] Cada gesto que señala fuera de plano tiene su superposición planificada.
- [ ] Packaging blindado en todo prompt de imagen con etiqueta de marca.
- [ ] Espacios muertos cortados, velocidad 1.12–1.20.
- [ ] Capa de realismo con los ocho valores exactos.
- [ ] Volumen bajado en los clips duplicados.
- [ ] Rótulo fijo de retención presente.

---

## 11 · TRACK ANIMADO

Método completo del segundo curso. **No es una variante del anterior**: no hay avatar humano, ni Omni, ni Grok,
ni capa de realismo. Cada clip es una **transición animada entre dos imágenes fijas**, nunca un plano generado
desde texto.

### 11.1 · Reglas invariables del track animado

1. **La planificación es una cadena de 8 pasos en orden.** Cada uno da por hecho lo que cerró el anterior; no
   se salta ninguno ni se cambia el orden.
2. **El estilo de animación se fija en el paso 1** —Pixar 3D, Apple realista, Sci-fi, Claymation o Wes
   Anderson— junto al producto y el mercado. Cambiarlo después invalida guion, storyboard y prompts.
3. **Un solo estilo en el Style Lock.** Si quedan varios, las imágenes salen incoherentes entre sí.
4. **El ángulo se construye sobre un dato duro**, no sobre una emoción: el anuncio abre con una cifra antes de
   nombrar el producto. Es la diferencia deliberada con el track realista.
5. **Toda imagen en 9:16 y 2K.** 1K cuesta lo mismo que 2K.
6. **Nombrar las imágenes `P1`, `P2`, `P3`… por el número de prompt del que salen.** Es lo que mantiene el
   orden de los pares primer/último frame.
7. **Cada clip es la transición entre dos imágenes consecutivas.** Número de clips = número de imágenes − 1.
8. **Todo prompt de clip termina en `sound effects (no talking)`.** Es el equivalente animado del `NO TALKING`.
9. **No se aplica la capa de realismo.** En un anuncio animado sobra por definición: no se busca que parezca
   real, se busca que parezca animado.
10. **Iterar es parte del método, no un plan B.** La IA aporta el 80 %; el 20 % restante es criterio. El punto
    donde más hay que iterar es el storyboard.

### 11.2 · Pipeline

`Avatar → Datos duros → Ángulos → Guion → Storyboard → Prompts de imagen → Auditoría → Marca`
`→ Imágenes → Clips → Voz → Montaje`

Los ocho primeros pasos son la cadena de planificación. Ejecútalos siempre en este orden, arrastrando el
contexto de los anteriores:

| # | Paso | Entrada | Salida |
|---|---|---|---|
| 1 | **Avatar + research** | Producto (3-4 frases: qué es, cómo funciona, en qué se diferencia, qué promete), mercado, estilo | Avatar hiperespecífico (quién es · 3 dolores concretos y observables · 3 cosas que ya probó y por qué le fallaron · el miedo que no admite · lo que quiere sentir) + 3 líneas de investigación de **datos duros** |
| 2 | **Insights** | Las 3 líneas de investigación | **5 insights con cifras reales**: estudios, estadísticas, mecanismos. Nunca opiniones ni experiencias personales |
| 3 | **Ángulos** | Los 5 insights | **3 ángulos**, cada uno sobre un dolor distinto. Elegir uno y decir por qué |
| 4 | **Guion** | El ángulo elegido | Guion del anuncio |
| 5 | **Storyboard** | El guion | Estructura visual escena a escena + **metáfora visual** |
| 6 | **Prompts de imagen** | El storyboard | Un prompt por escena, en inglés, con el estilo bloqueado |
| 7 | **Auditoría** | Todo lo anterior | Diagnóstico + guion definitivo + **2 variantes distintas** + storyboard y prompts corregidos |
| 8 | **Marca** | Nombre de producto y marca | El entregable final con la marca real inyectada |

Los dolores del paso 1 tienen que ser **observables**, no abstractos: "se despierta con la boca seca y siente
que no ha descansado", no "no duerme bien"; "nota la mandíbula menos definida en fotos recientes", no "le
preocupa su aspecto".

### 11.3 · Producción de imágenes

Modelo: **Nano Banana Pro**, texto a imagen, **9:16**, **2K**. Si hay producto real, va como imagen de
referencia. Las generaciones son independientes: pueden lanzarse en paralelo.

### 11.4 · Clips

Modelo: **Kling 3**, **720p**, **9:16**, modo **primer + último frame** (no texto→vídeo, no imagen única).
Se suben la primera y la última imagen del par y se genera la transición. Duración **3-5 s**, por defecto 4.

El prompt del clip es siempre el del estilo elegido, idéntico para todos los clips del anuncio:

**Realista (Apple)**
```
Seamless Apple-style cinematic transition. Minimal studio environment. Soft natural lighting. Clean, neutral tones. Ultra-clean. Minimal. Engineered. Apple keynote energy. Sound effects (no talking)
```

**Sci-fi**
```
Create a sci fi seamless transition between the first shot and the second shot in a sci fi animation style with sound effects (no talking)
```

**Pixar**
```
Create a seamless Pixar animated transition between the first shot and the second shot in a Pixar animation style with sound effects (no talking)
```

**Claymation**
```
create a seamless Claymation animated transition between the first shot and the second shot in a Claymation animation style with sound effects (no talking)
```

**Wes Anderson**
```
Create a Wes Anderson style cinematic transition between the first frame and the end frame with sound effects (no talking)
```

### 11.5 · Voz y montaje

**Voz** — ElevenLabs. Voz del catálogo → modelo **Eleven Multilingual V2**. Voz clonada propia → **V3**.

**Montaje en CapCut** — se coloca **primero el audio** y se monta el vídeo contra él. Valores exactos:

| Velocidad de los clips | Transición | Duración transición | Música | SFX de los clips | Voz |
|---|---|---|---|---|---|
| **1,20** (1,20-1,30) | **Mix**, aplicada a todas | **0,5-0,7 s** | **−25 a −30** | **−8** | **+5** |

Quitar los silencios largos de la narración. Balancear clip a clip de oído al final.
**Ojo: la velocidad 1.12-1.20 y los ocho valores de la capa de realismo son del track realista. Aquí no.**

### 11.6 · Formato de salida

Cuando se pida un anuncio animado, devolver en este orden:

1. **Avatar** en el formato del paso 1 (dolores observables, no abstractos).
2. **Los 5 insights con sus cifras**, y de dónde sale cada una. Si no tienes datos verificables, dilo: no
   inventes estadísticas.
3. **Los 3 ángulos**, y cuál eliges con el porqué.
4. **Guion definitivo + 2 variantes.**
5. **Storyboard**: tabla de escenas con la metáfora visual.
6. **Prompts de imagen** en inglés, en bloque de código, numerados `P1`, `P2`, `P3`…, todos con el mismo
   estilo bloqueado.
7. **Lista de clips**: `P1→P2`, `P2→P3`… con su duración y el prompt de estilo que les corresponde.
8. **Plan de montaje** con los valores exactos de §11.5.

### 11.7 · Antes de dar nada por bueno

- [ ] Los 8 pasos ejecutados en orden, arrastrando el contexto.
- [ ] Los insights llevan cifras reales y citadas, no inventadas.
- [ ] El ángulo elegido abre con un dato duro antes de nombrar el producto.
- [ ] Un solo estilo, el mismo en storyboard, prompts de imagen y prompts de clip.
- [ ] Imágenes en 9:16 y 2K, numeradas P1…Pn.
- [ ] Clips = imágenes − 1, cada uno definido como par primer/último frame.
- [ ] Todos los prompts de clip terminan en `sound effects (no talking)`.
- [ ] Montaje: 1,20 · Mix 0,5-0,7 · música −25/−30 · SFX −8 · voz +5.
- [ ] Ninguna referencia a la capa de realismo, a Omni, a Grok ni a un avatar hablando.
