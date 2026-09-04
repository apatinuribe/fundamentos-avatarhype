# Prompts — avatarhype

Kit operativo. Plantillas parametrizadas primero, instancias reales del curso después.
Los prompts van **en inglés** (así los da la fuente); el guion y la descripción del cambio pueden ir en español
[M1-L1.4.1], [M3-L3.2].

Convención: `{variable}` = hueco a rellenar · `[DESCRIPCIÓN]` = texto libre, tal como aparece en la fuente.

Biblioteca completa (86 prompts literales, sin editar): `sources/avatarhype/raw/_biblioteca-prompts.md`
— Parte A · La imagen (29) · Parte B · El vídeo (37) · Parte C · Los formatos (20) [M1-L1.4.1].

Las secciones 1-12 son del **track realista**. La **13 es el track animado** y sigue otra convención: sus 8 prompts
de planificación van **en español** porque los lee ChatGPT, y solo los 5 de estilo van en inglés [M6-L6.2].

---

## 1 · Estructura del prompt de clip

La pieza central del método [M1-L1.4.1], [M4-L4.1.1]:

```
CÁMARA + MOVIMIENTO + MICRO-ACCIÓN + GUION + VOZ + ACENTO
```

Orden de montaje según la biblioteca (la acción es opcional) [M1-L1.4.1]:

| # | Pieza | Ejemplo |
|---|---|---|
| 1 | **Cámara** | `(static camera, no movement) realistic arm movements and subtle micro-movements.` |
| 2 | **Acción** *(opcional)* | `She smiles and holds up the product,` |
| 3 | **Guion** | `then says: "Llevaba meses buscando algo así y mira, lo encontré."` |
| 4 | **Voz** | `Voice: a light, lively female voice — a woman in her mid-20s…` |
| 5 | **Acento** | `Spanish with a neutral Peninsular (Madrid) accent…` |

**Regla de colocación del gesto** [M1-L1.4.1]: la acción de **antes** de hablar va delante del `says:`; la de
**mientras** habla va detrás.

```
The person [acción], then looks at the camera and says: "[guión]"
The person says: "[guión]" [acción]
```

Se pueden combinar: `The person adjusts their cap, then says: "[guión]" and smiles.`

**Plantilla en blanco:**

```
CÁMARA
{movimiento de cámara}

MICRO-ACCIÓN
[{gesto en inglés}]

GUIÓN
she says: "{guion en español}"

VOZ
{línea Voice:}

ACENTO
{línea de acento}
```

---

## 2 · Menú de cámara

Todos llevan ya la coletilla que impide el corte [M1-L1.4.1].

**★ El más usado — cámara quieta + gestos**
```
(static camera, no movement) realistic arm movements and subtle micro-movements. Single continuous take, no cuts or scene changes.
```

**Plano fijo**
```
Locked-off static shot, camera completely still on a tripod, no movement at all. Single continuous take, no cuts or scene changes.
```

**Zoom lento a la cara** — el del CTA en [M4-L4.1.1]
```
Slow, continuous zoom-in toward the subject's face, starting from the very first frame and moving steadily closer, then holding steady on the close-up for the rest of the clip. Single continuous take, no cuts or scene changes.
```

**Zoom rápido al hablar**
```
Fast zoom-in to the subject's face at the very start, settling into a close-up exactly as they begin to speak, then holding steady. Single continuous take, no cuts or scene changes.
```

**En mano sutil**
```
Subtle handheld movement, very slight and natural, for a real human feel without distraction. Single continuous take, no cuts or scene changes.
```

**Acercamiento sutil · podcast**
```
Very gentle, almost imperceptible slow push-in on the speaker, from a medium shot to a medium close-up over the whole clip. Single continuous take, no cuts or scene changes.
```

**Retroceso que revela**
```
Slow pull-back from a close-up, revealing the surrounding environment as the subject starts talking, then holding on the wider shot. Single continuous take, no cuts or scene changes.
```

**Órbita lenta**
```
Slow arc shot, the camera orbiting around the subject in a smooth half-circle, subject stays centered. Single continuous take, no cuts or scene changes.
```

**Seguimiento al caminar** — el de los clips 1 y 2 de [M4-L4.1.1]
```
Tracking shot following alongside the subject as they walk and talk, smooth and steady. Single continuous take, no cuts or scene changes.
```

**Push-in a los ojos**
```
Slow creeping push-in that tightens into an extreme close-up on the eyes right as the key line is delivered, then holds. Single continuous take, no cuts or scene changes.
```

**Contrapicado heroico**
```
Low-angle hero shot looking up at the subject, slow push-in for authority and impact, then holding. Single continuous take, no cuts or scene changes.
```

**Profundidad de campo (bokeh)**
```
Shallow depth of field with a creamy bokeh background, slow push-in on the in-focus subject, then holding. Single continuous take, no cuts or scene changes.
```

**Cámara lenta**
```
Slow-motion delivery, smooth and cinematic, with a subtle camera drift. Single continuous take, no cuts or scene changes.
```

**Si montas un plano propio**, pegar al final [M1-L1.4.1]:
```
single continuous take, no cuts or scene changes — the camera holds steady on the framing after the move
```

**Añadir cámara en mano a cualquier clip** [M4-L4.3]:
```
Add subtle handheld camera movement throughout the shot, as if another person is casually filming. Keep the movement minimal, natural, and realistic, with slight handheld sway only.
```

---

## 3 · Menú de micro-acciones

Es un **gesto**, no lo que dice [M1-L1.4.1]:

| Inglés (lo que se escribe) | Español |
|---|---|
| `adjusts their cap` | se ajusta la gorra |
| `takes a sip of coffee and sets the cup down` | da un sorbo de café y deja la taza |
| `fixes their hair` | se arregla el pelo |
| `tucks hair behind their ear` | se coloca el pelo detrás de la oreja |
| `adjusts their glasses` | se ajusta las gafas |
| `waves hello` | saluda con la mano |
| `laughs` | se ríe |
| `with a surprised look on their face` | con cara de sorpresa |
| `and nods slowly, smiling` | asiente despacio, sonriendo |
| `points up` / `points up to the left` / `points to the right` | señala arriba / a la izquierda / a la derecha |
| `crosses their arms` | cruza los brazos |
| `shrugs` | se encoge de hombros |
| `gives a thumbs up` | pulgar arriba |
| `claps once` | da una palmada |
| `tilts their head curiously` | inclina la cabeza con curiosidad |
| `taps their chin thoughtfully` | se toca la barbilla, pensativo/a |
| `snaps their fingers` | chasquea los dedos |
| `rolls their eyes playfully` | pone los ojos en blanco, en broma |

**Modificadores de tiempo** que el curso usa:

- `While speaking, {acción}` — la acción ocurre *durante* el habla [M4-L4.1.2].
- `{acción} while saying in the first 3 seconds of the video:` — acota el momento exacto [M4-L4.1.4].

**Extender crema mientras habla** [M1-L1.4.1]. La IA deja la crema flotando o la multiplica; hay que pedir
explícitamente que la cantidad visible decrezca:
```
While speaking, she gradually blends the visible cream into the [aquí el sitio] until it is smoothly absorbed into the skin. The amount of visible cream continuously decreases throughout the clip, leaving no residue, streaks, or buildup.
```

---

---

## 4 · Menú de voz

Usar la **misma línea `Voice:`** en todos los clips del mismo personaje y en la misma sesión [M1-L1.4.1].

```
Voice: a deep, warm male voice — a man in his early-to-mid 50s, low and resonant with a slight gravelly texture, calm and unhurried, confident and grounded.
```
```
Voice: a bright, energetic male voice — a guy in his mid-to-late 20s, medium-high pitch, clear and relaxed, friendly and upbeat, casual conversational pace.
```
```
Voice: a youthful male voice — a guy in his mid-20s, bright and fairly high-pitched, light and energetic, casual relaxed pace.
```
```
Voice: a male voice in his mid-30s, medium pitch, a bit fuller and more settled than a twenty-something, calm and confident, friendly but grounded.
```
```
Voice: a warm, mature female voice — a woman in her early 50s, rich and slightly smoky lower-mid tone, calm and measured pacing, confident and reassuring.
```
```
Voice: a light, lively female voice — a woman in her mid-20s, bright and clear with a higher pitch, warm and friendly, natural conversational pace.
```
```
Voice: a youthful female voice — a woman in her mid-20s, bright and fairly high-pitched, light and breezy, casual relaxed pace.
```
```
Voice: a female voice in her mid-30s, medium pitch, a bit fuller and more settled than a twenty-something, calm and confident, warm but grounded.
```

**Fórmula para inventar cualquier voz** [M1-L1.4.1]:
género + edad (`in his/her 20s / 40s / 60s`) + gravedad (`deep, low` | `bright, high`) + textura
(`gravelly, raspy` | `smooth, clean` | `soft, breathy`) + entrega (`calm and slow` | `energetic and fast` | `warm` |
`authoritative`).

Forma abreviada que el curso usa en la práctica: `Voice: light female voice, mid-20s, bright.` [M4-L4.1.2].

---

## 5 · Menú de acento

Se añade al final de cualquier prompt con voz [M1-L1.4.1].
**El latino neutro sale por defecto; el de España hay que pedirlo siempre** [M4-L4.1.1].

```
Spanish with a neutral Peninsular (Madrid) accent, informal and conversational, like a real casual chat in Spain.
```
```
Spanish with an Argentine Rioplatense (Buenos Aires) accent, including the typical "sh" sound for "ll" and "y".
```
```
Spanish with a clear, neutral Colombian (Bogotá) accent.
```
```
Spanish with a Mexican (central, Mexico City) accent.
```
```
Spanish with a neutral Latin American accent.
```

---

## 6 · Imagen · el método 6C

Estructura interna del agente al describir una imagen de avatar [M3-L3.2]:

```
C1 Character           — personaje: edad, vibe, atractivo, detalles de cara
C2 Camera              — cámara: POV, ángulo, lente, encuadre (realismo de iPhone)
C3 Clothing            — ropa: outfit, styling, accesorios
C4 Context             — escena: localización y detalles de fondo
C5 Cinematic Light     — luz: tipo de flash, sombras, grano, mood
C6 Consistency Anchors — anclajes de realismo, restricciones y limpieza
```

**Vía sin agente — cambiar la persona por descripción** [M3-L3.2]:
usar el prompt de la biblioteca *"cambiar el avatar en base a una descripción"* y rellenar, p. ej.:
`caucásica, rubia, ojos azules, una chica natural, imperfecta, real`.

---

## 7 · Imagen · plantillas de continuidad

### 7.1 · Cambiar el aspecto de la misma persona [M4-L4.1.1]

```
Using this image as reference, keep the SAME person — same face and identity — and make [DESCRIPCIÓN]. Photorealistic, natural skin texture and lighting.
```

Instancias reales (acné, [M4-L4.1.1]):
```
Using this image as reference, keep the SAME person — same face and identity — and make [en el baño una foto muy cerca de su cara con acné, lleva una camiseta blanca.]. Photorealistic, natural skin texture and lighting.
```
```
Using this image as reference, keep the SAME person — same face and identity — and make [en el baño una foto muy cerca de su moflete con la piel muy glowy, lleva una sudadera gris. Lleva un moño]. Photorealistic, natural skin texture and lighting.
```

### 7.2 · Siguiente estado de la misma escena [M4-L4.1.2]

Patrón: `Edit the reference image. Keep everything exactly the same.` + lo que cambia + **lista explícita de lo que
no cambia** + `The result should look like the next frame of the same video.`

```
Edit the reference image. Keep everything exactly the same.
The woman is no longer holding the glass. Place the empty glass on the countertop in front of her. The BLUME container remains open in the same position with the lid beside it. Place the scoop with green powder on the countertop next to the glass. The woman is now looking directly at the camera while talking and naturally gesturing with both hands. Do not change her face, outfit, kitchen, lighting, camera angle, framing, composition, or the BLUME packaging.
```

**Con blindaje de packaging** [M4-L4.1.2]:
```
Edit the reference image. Keep everything exactly the same. The woman is now turned toward the open kitchen cabinet while looking back at the camera. One hand is opening the cabinet door and the other is holding the BLUME container, placing it inside the cabinet. Remove the glass, scoop, lid, and powder from the countertop. Keep the same woman, outfit, kitchen, lighting, camera angle, framing, composition, and the exact BLUME packaging without changing the branding, colors, typography, or label. The result should look like the next frame of the same video.
```

Fragmento reutilizable: `without changing the branding, colors, typography, or label`.

### 7.3 · Producto solo, quitando a la persona [M4-L4.1.2]

```
Edit the reference image. Remove the woman and everything she is using. Keep the kitchen, lighting, camera angle, framing, and composition exactly the same. Place the closed BLUME container in the center of the countertop where she was standing, using the exact packaging from the reference without changing the branding, colors, typography, or label. The countertop should look naturally clean, with no artifacts. The final image should look like the original photo was taken with only the BLUME container on the countertop.
```

### 7.4 · Avatar sosteniendo el producto [M4-L4.1.2]

```
Using this photo, keep the same woman, her white dress with black trim, the kitchen and the lighting. Change the action: she now holds up a tall clear glass of already-mixed smooth opaque green drink (fully dissolved, no powder or clumps) in one hand, looking straight at the camera with a friendly expression. The scoop and the BLUME container are now resting on the counter. With her free hand she makes a natural, relaxed talking gesture. Photorealistic, realistic hands. Single image.
```

### 7.5 · Reciclar el encuadre para otra escena [M4-L4.3]

```
Edit the reference image.

Keep the exact same woman, kitchen, clothing, countertop, camera angle, framing, perspective, lighting, shadows, background, and overall composition.

Replace the {objeto A} with {objeto B} placed naturally in the same area of the countertop.

{detalle del objeto B}

{qué hace ahora la persona}

Everything else must remain identical. The final image should look like the next natural moment in the same scene, captured with the same iPhone camera, without changing the environment or composition.
```

### 7.6 · Insertar el packaging real sobre una escena generada [M4-L4.3]

Se adjuntan **tres** referencias: character sheet + escena + producto.
```
Use the provided character sheet as the exact identity reference for the woman. Preserve her facial features, proportions, skin tone, hairstyle, and overall appearance exactly.

Use the kitchen reference image for the exact scene, composition, camera angle, lighting, pose, outfit, kitchen layout, and overall framing.

Replace the placeholder product with the exact BLUME container from the product reference. Keep the BLUME packaging identical, including the logo, typography, colors, proportions, lid, and label design. Do not redesign or modify the packaging in any way.

The woman is holding the open BLUME container in one hand and a scoop filled with BLUME Greens above a glass of water with the other. The glass is placed on the kitchen countertop, with the BLUME lid resting beside it.

Authentic iPhone photography, vertical 9:16, ultra realistic, natural indoor lighting, subtle iPhone HDR, no cinematic grading.
```

### 7.7 · Cambiar vestuario o fondo por descripción [M1-L1.4.1]

Los dos retoques más básicos de la biblioteca. Se aplican sobre una imagen ya buena, no se regenera de cero.

**Solo la ropa**
```
Using this image as reference, keep the SAME person — same face, hair, body, pose, background and lighting. Change ONLY their clothing to [escribe el outfit aquí]. Keep everything else exactly the same. Photorealistic, natural fabric, realistic fit and lighting.
```

**Solo el fondo**
```
Replace the background behind the person with [describe el sitio: a cozy kitchen / a modern office / a neutral studio with soft lighting], keeping the person, their pose, lighting and framing exactly the same. Natural, realistic integration.
```

### 7.8 · Cambiar fondo o avatar con una segunda imagen de referencia [M1-L1.4.1]

Cuando el destino es difícil de describir con palabras, se adjunta. Misma lógica que el prompt de outfit de moda
(§8): **imagen 1 = persona, imagen 2 = lo que se copia**, y hay que decirlo explícitamente para que el modelo no
se traiga la cara de la segunda.

**Fondo desde imagen de referencia**
```
Using the two reference images (image 1: the person; image 2: the background / setting), keep the SAME person from image 1 — same face, hair, skin, body, outfit and pose — and place them into the EXACT background shown in image 2, matching its location, colors, depth and atmosphere. Keep the person's pose, scale and framing exactly the same; replace ONLY what is behind them. Blend naturally: consistent lighting and shadows, matching color temperature and perspective, realistic edges with no cut-out look. The person is image 1, the background is image 2 — do NOT take any person or object from image 2. Photorealistic. Single image.
```

**Sustituir a la persona, por descripción**
```
make this woman/man a different one, [DESCRIPCIÓN, OUTFIT...]
```

**Sustituir a la persona, por imagen de referencia**
```
replace the guy from the file 1 with the guy from the file 2 wearing the same outfit as in file 2
```

### 7.9 · Producto en la mano con dos referencias [M1-L1.4.1]

Variante genérica de §7.4: en vez de describir el producto, se adjunta su foto. Es lo que se usa cuando el
packaging es real y no puede reinventarse.

**Sostenerlo y enseñarlo**
```
Using the two reference images (the person and the product), place the product in the person's hand so they are holding it up and showing it to the camera while talking about it.
```

**Señalarlo**
```
Using the two reference images (the person and the product), show the person pointing at the product (held in the other hand or placed next to them) while looking at the camera. Keep the person's face and look unchanged, and keep the product's label and packaging exactly the same. Realistic hands and lighting.
```

### 7.10 · Acercar el encuadre sin regenerar [M1-L1.4.1]

**Voltear la imagen** — útil para reutilizar un encuadre sin repetirlo idéntico:
```
Flip the image horizontally
```

```
A closer view of this same image shows less countertop. He's talking to the camera, you can see his teeth well
```

### 7.11 · App o software en pantalla [M1-L1.4.1]

**Dos pasos, siempre en este orden.** Primero se genera al avatar sosteniendo el dispositivo con la **pantalla
negra apagada**, y solo después se incrusta la captura encima. Pedir las dos cosas en un solo prompt hace que el
modelo se invente la interfaz.

**Paso 1 · móvil con pantalla negra**
```
Using the reference image, keep the SAME person — same face, hair, skin, body and identity — the SAME outfit, background and lighting.

Change ONLY this: she is now holding up a modern smartphone toward the camera, showing its screen to the viewer, the screen completely OFF and solid black (a blank black rectangle, no reflections, no UI, no icons, no text, no brand logos). She holds it naturally with one hand, the display side facing the camera, at chest height.

Keep both hands realistic and natural, correct number of fingers, natural grip on the phone. Photorealistic, natural skin texture and lighting. Single image.
```

**Paso 2 · incrustar la captura en el móvil**
```
Using the two reference images (image 1: the person holding a smartphone with a black screen; image 2: an app screenshot), keep image 1 EXACTLY the same — same person, face, hair, hands, phone, pose, background and lighting, all unchanged.

Change ONLY this: place the screenshot from image 2 onto the phone's black screen, so it fills the display naturally. Fit it to the exact shape of the screen, matching the perspective and slight tilt of the phone, with realistic screen brightness, subtle glare and rounded screen corners. Do NOT crop or stretch the screenshot, keep its aspect ratio. The screenshot must look like it is really displayed on the phone.

Keep everything else identical to image 1. Photorealistic. Single image.
```

**Paso 1 · portátil con pantalla negra**
```
Using the reference image, keep the SAME person — same face, hair, skin, body and identity — the SAME outfit, background and lighting.

Change ONLY this: she is now sitting with an open laptop, turning it and holding the screen toward the camera so the viewer sees the display. The laptop screen is completely OFF and solid black (a blank black rectangle, no reflections, no UI, no icons, no text, no brand logos). Natural, realistic pose tilting the laptop so the screen clearly faces the camera.

Keep both hands realistic and natural, correct number of fingers. Photorealistic, natural skin texture and lighting. Single image.
```

**Paso 2 · incrustar la captura en el portátil**
```
Using the two reference images (image 1: the person holding a laptop with a black screen; image 2: an app or website screenshot), keep image 1 EXACTLY the same — same person, face, hair, hands, laptop, pose, background and lighting, all unchanged.

Change ONLY this: place the screenshot from image 2 onto the laptop's black screen, so it fills the display naturally. Fit it to the exact shape of the screen, matching the perspective and tilt of the laptop, with realistic screen brightness, subtle glare and correct proportions. Do NOT crop or stretch the screenshot, keep its aspect ratio. The screenshot must look like it is really displayed on the laptop.

Keep everything else identical to image 1. Photorealistic. Single image.
```

### 7.12 · Skincare · abrir un bote de tapa abatible [M1-L1.4.1]

A la IA le cuesta abrir envases. La solución del curso: adjuntar **el bote cerrado + una foto de un mecanismo de
apertura equivalente**, y dejar claro que la segunda imagen es solo referencia del mecanismo.

```
Using the two reference images (image 1: the person holding the product bottle; image 2: an open flip-top cap, shown ONLY as a reference for the mechanism), keep the SAME person (same face, hair, skin and identity), the SAME bottle with its label, colors and text exactly unchanged, and the SAME room, background and lighting.

Change ONLY this: the bottle's flip-top cap is now flipped open on its hinge — the small lid tilted up and back and the nozzle opening exposed, exactly like the open flip mechanism in image 2. The hinged lid stays ATTACHED to the bottle; do NOT remove the cap. She raises her other hand beside the bottle, palm cupped and open, fingers relaxed, as if about to squeeze a little product into it.

Keep both hands realistic and natural, correct number of fingers. Photorealistic, natural skin texture and lighting. Single image.
```

---

---

## 8 · Imagen · pipeline de moda

Orden estricto: `avatar → cuerpo entero → pared blanca → outfit 1 → outfit 2 …` [M4-L4.1.3].

**Cuerpo entero**
```
Using this image as reference, keep the SAME person (same face and identity), the same outfit and the same setting. Render a full-body shot from head to toe, the person standing naturally. Photorealistic, natural skin texture and lighting.
```

**Pared blanca (solo el fondo)**
```
Behind the woman there is a plain white wall, and the floor remains exactly the same as in the reference image. Do not change the flooring, its material, color, texture, or perspective. Only replace the background behind her with a clean white wall while keeping everything else identical.
```

**Vestir con un outfit de referencia** — se adjuntan **dos imágenes: 1 = persona, 2 = ropa**
```
Using the two reference images (image 1: the person; image 2: the outfit / clothing), keep the SAME person from image 1 — same face, hair, skin, body and identity — and dress her in the EXACT outfit shown in image 2, matching its garments, colors, patterns, textures and details as closely as possible. Change ONLY her clothing; keep her pose, framing, background and lighting exactly the same. The outfit fits her body realistically, with natural fabric folds and realistic lighting. The person is image 1, the clothes are image 2 — do NOT copy the face or body from image 2. Photorealistic. Single image.
```

**Producto en la mano (dos referencias: persona + producto)** [M4-L4.1.3]
```
Using the two reference images (the person and the shampoo), place the shampoo in the person's hand so they are holding it up and showing it to camera while talking about it, gesturing naturally, engaged expression. Keep the person's face and identity unchanged, keep the label exactly the same. Realistic hands, photorealistic, natural skin texture, visible pores. No text, no watermark, no distortion.
```

---

## 9 · Imagen · estética iPhone (voz en off y trends)

Bloque de realismo que el curso repite [M4-L4.3], [M4-L4.5]:
```
Authentic iPhone photography, vertical 9:16, ultra realistic, natural lighting, subtle iPhone HDR, no cinematic grading.
```
```
Keep skin completely untreated with realistic pores, redness, acne, texture, natural shine, and imperfections. Preserve authentic smartphone realism without any beauty enhancement.
```
```
No text, no watermark, no distortion.
```

**Anclar identidad al character sheet** [M4-L4.3]:
```
Use the provided character sheet as the exact identity reference for the woman. Preserve her facial features, proportions, skin tone, hairstyle, expression, and overall appearance exactly. She must wear the exact same {prenda} shown in the character sheet.
```

**Plantilla general del formato voz en off** (la biblioteca no da prompts cerrados) [M4-L4.3]:
```
Usando esta imagen de referencia, haz a la persona de la imagen sin cambiar absolutamente nada de ella, haciendo la siguiente acción: {acción}. {sitio} · {luz} · {plano}
```

**Ejemplos completos** (conduciendo · mirror selfie · cocinando · primera persona) en `ejemplos.md` § Voz en off.

---

## 10 · Clips sin habla (Grok)

**Regla**: todo clip sin guion lleva `NO TALKING` [M4-L4.3]. También `No talking, mouth closed` [M4-L4.1.2].

Ejemplos literales [M4-L4.3]:
```
NO TALKING. She is filming herself selfie-style while naturally walking down a staircase and casually drinking an iced coffee. It feels like a spontaneous TikTok vlog. Nobody else is filming her. Authentic handheld iPhone front-camera movement.
```
```
NO TALKING. She naturally walks up to a black Mercedes G-Class, unlocks it, opens the driver's door, and gets in. Authentic handheld iPhone footage, casual lifestyle aesthetic.
```
```
NO TALKING. She pours one scoop of the greens powder into the glass of water, then uses the same scoop to gently stir the drink until it begins to mix. Natural, unhurried movements.
```
```
NO TALKING. She casually poses for a short post-workout video in the gym locker room. She confidently adjusts her posture, looks at the camera, and makes subtle natural movements as if recording content for social media.
```
```
NO TALKING. She picks up a piece of sushi with chopsticks, takes a bite, chews naturally, then looks directly at the camera with a genuinely satisfied expression. She subtly rolls her eyes back for a brief moment as if thinking, "wow, that's so good," then smiles softly. Authentic iPhone footage with slight handheld camera movement, as if someone else is casually filming.
```

**Clips de pose para moda** (Grok, 6 s) [M4-L4.1.3]. Los tres comparten cabecera:
`Using this image as reference, keep the SAME person (same face and identity) and the SAME location, background and lighting as the reference (do NOT change the setting).`

```
… A full-body shot from head to toe showing the complete outfit, the person standing and turning slightly to show the clothes. Cinematic lighting, no talking, mouth closed. Single continuous take, no cuts.
```
```
… The person walks toward the camera showing the outfit in motion, confident and natural catwalk energy. Cinematic lighting, no talking, mouth closed. Single continuous take, no cuts.
```
```
… The person slowly turns a full 360 degrees on the spot to show the outfit from every side, smooth continuous rotation. Cinematic lighting, no talking, mouth closed. Single continuous take, no cuts.
```

**Clip de producto con partículas** [M4-L4.1.2]:
```
Using this image, keep the Blume jar, its label and the kitchen exactly the same. Camera static with a very slow, subtle push-in. Around the jar, a minimal and refined cloud of abstract particles floats and drifts very slowly in soft slow motion, in green and soft golden tones: fine delicate strands (fiber), a few small translucent green leaf fragments (plant extracts), tiny suspended micro-spheres like living cultures (probiotics), and small glowing golden dots of light (vitamin). Very sparse, elegant and airy, barely-there movement, soft natural window light, shallow depth of field, clean and premium. Do not alter or morph the jar, label or text. No talking, mouth closed. Single continuous take, no cuts. No text, no watermark.
```

**Plantilla genérica de clip mudo** (voz en off, trends) [M1-L1.4.1]:
```
[movimiento de cámara], cinematic, no talking. Keep the SAME person from the reference. She [acción]. [sitio + luz]. No text, no watermark.
```

**Seis clips mudos ya montados** [M1-L1.4.1] — sirven de banco de planos de apoyo tal cual:
```
Slow subtle push-in, cinematic, no talking. Keep the SAME person from the reference. She looks at herself in the bathroom mirror just woken up, messy frizzy curly hair, one hand touching her face, sleepy expression. Soft morning light through the window, shallow depth of field. No text, no watermark.
```
```
Tracking shot following alongside her, cinematic, no talking. Keep the SAME person. She walks down a city street, natural stride, hair moving. Daytime urban background, natural light. No text, no watermark.
```
```
Static close-up, cinematic, no talking. Keep the SAME person. She blends visible cream into her face with gentle circular motions, product decreasing until absorbed. Bright bathroom, soft light. No text, no watermark.
```
```
Slow arc shot orbiting her, cinematic, no talking. Keep the SAME person. She holds a mug of coffee with both hands, relaxed, looking out the window. Warm morning light. No text, no watermark.
```
```
Slow-motion, cinematic, no talking. Keep the SAME person. She moves her defined healthy curly hair, side profile then back view, hair catching the light. Soft natural light. No text, no watermark.
```
```
Slow gentle camera move, cinematic, no talking. Clean beauty shot of the product on a surface, soft natural lighting, product in sharp focus, label visible and unchanged. No people. No text, no watermark.
```

---

---

## 11 · Formatos con estructura de prompt propia

### 11.1 · Dualcast — doble bloque de micro-acción [M4-L4.4]

```
CÁMARA
(static camera, no movement) realistic arm movements and subtle micro-movements. Single continuous take, no cuts or scene changes.

MICRO-ACCIÓN
The person on the {LEFT|RIGHT} is actively speaking in a natural conversation.

GUIÓN
"{guion}"

MICRO-ACCIÓN
The person on the {la otra} is only listening, occasionally nodding slightly, reacting naturally and looking at HIM/HER while he/she talks. Casual realistic interaction, subtle facial reactions, authentic conversational energy, no interruption.

ACENTO
{acento}
```

`LEFT` / `RIGHT` **en mayúsculas**. Sin el segundo bloque, el modelo hace hablar a los dos o congela al que escucha.

### 11.2 · Podcast [M4-L4.2]

Las micro-acciones son **reacciones del que escucha**:
```
[He nods in agreement with what she has just heard and says:]
[She pauses for a moment as if thinking about her answer, then says]:
[She nods in agreement while saying:]
[She is reading the news article displayed on her phone to the person in her right. After finishing reading, she lifts her head, and reacts with a naturally surprised expression. The reaction is subtle and realistic, not exaggerated.]
```

**Cambiar el ángulo de mirada** (quitar el móvil de la escena):
```
She is no longer looking at her phone. Instead, she is looking to her right at the other podcast host.
```

**Encuadre de podcast · mirar al otro interlocutor** [M1-L1.4.1]. Se pide en la imagen, no en el clip:
```
She/he is looking to the right/left side of the frame, as if talking to someone sitting next to her/him.
```

**Clip base de una intervención** [M1-L1.4.1]:
```
(static camera, no movement) the person talks naturally with realistic micro-movements and subtle arm gestures, authentic conversational energy. They say: "[inserta el guión aquí]"
```

**Candado contra el segundo hablante** [M1-L1.4.1] — si en la imagen se ve a los dos, el modelo tiende a hacer
hablar a ambos:
```
Single speaker: only the person from the reference image talks.
```

### 11.3 · UGC a cámara · variantes cortas [M1-L1.4.1]

Versiones de una línea, para cuando no hace falta el bloque completo de §1.

```
(static camera, no movement) he/she's looking directly at the camera, realistic arm movements, clear influencer tone: "[inserta el guión aquí]"
```
```
realistic arm movements, the woman/man says exactly with direct clear energy: "[inserta el guión aquí]"
```

**Con el producto en el clip** [M1-L1.4.1]:
```
Using the product from the reference image, the person holds the product in one hand and shows it to the camera while talking, looking at the camera with natural, realistic gestures. Keep the product's label and packaging clearly visible and unchanged. Single continuous take, no cuts.
```
```
Using the product from the reference image, while talking to the camera the person naturally points at the product and glances down at it a couple of times, then back to the camera, with relaxed, realistic gestures. Keep the product's label and packaging clearly visible and unchanged. Single continuous take, no cuts.
```
```
Using the product from the reference image, a clean beauty shot of the product on a [surface: marble counter / wooden table / neutral backdrop], slow gentle camera move, soft natural lighting, the product in sharp focus with its label clearly visible and unchanged. No people. Single continuous take, no cuts.
```

**Bloque completo de ejemplo**, con cámara, voz y acento en un solo prompt [M1-L1.4.1]:
```
The person looks directly at the camera with natural gestures and a clear, friendly influencer tone. Slow zoom-in toward their face from the first frame, holding once close. Single continuous take, no cuts. They say: "[tu guión]"
Voice: a bright, energetic male voice — a guy in his mid-to-late 20s, clear and relaxed, friendly and upbeat.
Spanish with a neutral Peninsular (Madrid) accent, informal and conversational, like a real casual chat in Spain.
```

---

---

## 12 · Prompts de entrada a los agentes

### El Estratega [M3-L3.3.3]
```
{producto en una frase}
→ el agente pregunta por el avatar
{avatar en una frase}
→ fase 2: estrategia (dolores, deseos, objeciones, ángulos, hooks, mecanismo, nivel de conciencia)
→ propone 3 ángulos y pregunta cuáles desarrollar
"elige los tres mejores"
→ fase 3: los anuncios desglosados clip a clip (rótulo · visual · guion)
```

Para forzar un formato concreto, decírselo en lugar de dejarle elegir: *"quiero hacer un día conmigo"* [M4-L4.3].
Instancia real: `es una app de entrenamiento para mujeres` → `"elige los tres mejores"` [M4-L4.1.4].

### Ads Visual Architect · imágenes estáticas [M4-L4.6]
```
{producto en una frase}
→ el agente devuelve análisis + 7 formatos y pregunta si encaja
"me encaja" + {paleta de colores} + {mercado} + {precio}
→ pide una foto limpia del producto sobre fondo neutro
→ devuelve los prompts, uno por formato
→ "dame más formatos" para ampliar
```

**Antes de generar: reemplazar el marcador `marca` por el nombre real.** Si no se indica mercado, asume España.

---

## 13 · Ads animados · el sistema de 8 prompts [M6-L6.2]

Kit completo del **track animado** (ver `proceso.md` § Track Animados). Son 13 prompts: 8 encadenados de
planificación, en español, para ChatGPT — y 5 de estilo, en inglés, para el modelo de vídeo.

Reglas de uso [M6-L6.2]:

- **Los 8 van en una sola conversación de ChatGPT**, en orden, sin saltarse ninguno.
- **El 2 es la excepción: se pega en NotebookLM**, no en ChatGPT. Es el error más fácil de la secuencia.
- **En el 6, Style Lock: dejar únicamente el estilo elegido** en el Prompt 1.
- Iterar es parte del método: los 5 insights, el ángulo, el guion y sobre todo el storyboard se rehacen hasta
  que convenzan. *"La IA hace el 80 % del trabajo; ese 20 % —el criterio, el ojo humano— es lo que hace que el
  anuncio sea bueno o no."*

Copia sin editar: `sources/avatarhype-animados/raw/_documento-8-prompts.md`.

### 13.1 · Los 8 prompts de planificación

| # | Prompt | Dónde se pega |
|---|---|---|
| 1 | Avatar + research | ChatGPT |
| 2 | Auto-research + insights | **NotebookLM**, no ChatGPT |
| 3 | Ángulos | ChatGPT |
| 4 | Guion | ChatGPT |
| 5 | Storyboard (escenas) | ChatGPT |
| 6 | Prompts de imagen (NB) | ChatGPT |
| 7 | Auditoría completa FINAL | ChatGPT |
| 8 | Introducción al producto | ChatGPT |

#### 13.1.1 · Prompt 1 — Avatar + research

Se pega en: ChatGPT. Rellenar `PRODUCTO` (3-4 frases), `MERCADO` y `ESTILO ANIMACIÓN`. Devuelve el avatar y **3 búsquedas** para NotebookLM.

```
Eres un estratega senior de marketing de respuesta directa especializado en anuncios animados de ecommerce.

Vamos a construir un anuncio animado. Te paso el contexto:

PRODUCTO: [PEGA AQUÍ EL PRODUCTO con 3-4 frases que describan: qué es, cómo funciona, cómo se diferencia de la competencia, y qué promete. Ejemplo: "Cloudy. Una almohada ergonómica de viscoelástica diseñada para mantener la columna alineada durante toda la noche, independientemente de la postura (boca arriba, de lado, boca abajo). A diferencia de otras almohadas cervicales del mercado, Cloudy se adapta dinámicamente al peso del cuello y la cabeza. Promesa: menos dolor de cuello, espalda y hombros, menos ronquidos y prevención de arrugas prematuras por presión facial."]
MERCADO: [Ej: España]
ESTILO ANIMACIÓN ELEGIDO: [Pixar 3D / Apple realista / Sci-fi / Claymation / Wes Anderson]

Tu primera tarea: construir un avatar HIPER-específico del cliente, y luego prepararme 3 búsquedas cortas para pegar en NotebookLM Discover Sources. Las búsquedas tienen que enfocarse a traer DATOS DUROS (estadísticas, estudios, mecanismos), no opiniones ni experiencias personales. Porque el anuncio final será de conversión con datos, no de identificación emocional.

Devuélveme TODO con esta estructura exacta:

═══════════════════════════════
<<AVATAR>>
═══════════════════════════════

QUIÉN ES (1 línea): edad, sexo, situación de vida.

3 PUNTOS DE DOLOR concretos relacionados con este problema (cada uno descrito en 1-2 líneas, específico y observable, no abstracto). El anuncio atacará uno de estos dolores con datos. Ejemplos de bueno vs malo:
✅ "Se despierta con la boca seca cada mañana y siente que no ha descansado de verdad"
❌ "No duerme bien"
✅ "Nota la mandíbula menos definida en fotos recientes comparado con hace 2 años"
❌ "Le preocupa su aspecto"

LO QUE YA HA PROBADO antes (3 cosas concretas que le fallaron y por qué le fallaron).

EL MIEDO PROFUNDO que no admite (el "y si nunca…").

LO QUE QUIERE SENTIR (resultado emocional, no funcional).

═══════════════════════════════
<<BUSQUEDAS_NOTEBOOKLM>>
═══════════════════════════════

NotebookLM Discover Sources NO funciona con prompts largos. Funciona con búsquedas cortas tipo Google (2-3 frases máximo, con palabras clave específicas).

Dame 3 BÚSQUEDAS DISTINTAS para pegar una a una en Discover Sources. Cada búsqueda tiene que traer DATOS DUROS utilizables en un guión de conversión, NO opiniones o experiencias subjetivas.

Cada búsqueda debe:
- Tener 2-3 frases como máximo
- Estar en el idioma del mercado
- Atacar un ángulo DIFERENTE de datos duros (no repetir enfoque)
- Priorizar fuentes como: estudios científicos, revistas médicas, artículos con cifras, investigaciones, datos históricos, papers académicos, contenido especializado con estadísticas

Devuelve cada búsqueda en su propio bloque de código para copiar con un click.

BÚSQUEDA 1 — Ángulo: ESTADÍSTICAS Y CIFRAS DEL PROBLEMA
Ejemplo de enfoque: "qué porcentaje de la población tiene este problema", "cuántas horas al día/año ocurre", "cuánto tiempo se tarda en aparecer", "qué % de mejora se consigue resolviéndolo". Buscar datos duros que cuantifiquen la magnitud.

BÚSQUEDA 2 — Ángulo: MECANISMO BIOLÓGICO / CIENTÍFICO
Ejemplo de enfoque: "cómo funciona biológicamente", "qué pasa en el cuerpo cuando...", "por qué ocurre este proceso", "qué dicen los estudios sobre el mecanismo". Buscar explicaciones de causa-efecto respaldadas por ciencia.

BÚSQUEDA 3 — Ángulo: EVIDENCIA HISTÓRICA / EVOLUTIVA / COMPARATIVA
Ejemplo de enfoque: "desde cuándo existe este problema", "cómo era en poblaciones antiguas o culturas distintas", "por qué ha aumentado en la sociedad moderna", "qué cambió para que esto apareciera". Buscar contexto que dé perspectiva y sirva de gancho narrativo.

REGLAS:
- Las búsquedas apuntan a DATOS, no a foros de quejas.
- Si es posible, priorizar palabras clave como "study", "research", "statistics", "percentage", "data", "estudio", "investigación", "estadísticas", "porcentaje" según el idioma.
- Cada búsqueda es autónoma y trae un tipo distinto de munición.

═══════════════════════════════

REGLAS FINALES:
- Nada genérico. Si una respuesta vale para cualquier producto, está mal.
- El avatar describe al cliente con precisión, pero NO recolecta frases literales suyas. El contenido del guión vendrá de los datos de NotebookLM, no del lenguaje del cliente.
- Las búsquedas van al PROBLEMA con enfoque de datos, no a experiencias subjetivas.
```

#### 13.1.2 · Prompt 2 — Auto-research + insights

Se pega en: **NotebookLM**, no ChatGPT. Se pega en el chat del cuaderno una vez importadas las 3 búsquedas. Devuelve **5 insights** con cifras.

```
Basándote ÚNICAMENTE en las fuentes cargadas, devuélveme los 5 INSIGHTS más fuertes para construir un anuncio animado de CONVERSIÓN con datos.

Un insight ATÓMICO cumple 3 condiciones:
1. Es específico y está respaldado por DATOS DUROS (cifras, estudios, mecanismos biológicos)
2. Es contraintuitivo o sorprendente (rompe una creencia común del cliente)
3. Está respaldado literalmente por las fuentes (cita la fuente)

Este anuncio no va a vender con frases emocionales del cliente. Va a vender demostrando el problema con datos. Por tanto, prioriza insights que tengan MUNICIÓN DURA.

Devuelve cada insight con esta estructura exacta:

═══════════════════════════════
<<INSIGHT 1>>
═══════════════════════════════

TITULAR: una frase que captura el insight con una cifra o dato incluido.

LO QUE EL CLIENTE CREE: la creencia común que este insight rompe.

LO QUE EL INSIGHT REVELA: la verdad incómoda detrás, con datos concretos.

DATOS DUROS QUE LO RESPALDAN: lista de cifras, porcentajes, duraciones, estudios o estadísticas que aparecen en las fuentes, cada una con referencia a su fuente. Copia literal. Si una fuente dice "el 87% de adultos…", cópialo tal cual con la referencia.

MECANISMO BIOLÓGICO / CIENTÍFICO: explica paso a paso la cadena causa-efecto que hace que este insight sea cierto, tal y como lo explican las fuentes. Ejemplo: "al ocurrir X, se activa Y, lo que provoca Z".

CONTEXTO HISTÓRICO / COMPARATIVO (si aplica): cualquier dato sobre cuándo empezó este problema, cómo era antes, o comparativas con otras poblaciones/épocas que aparezca en las fuentes.

POR QUÉ SE PUEDE VENDER CON ESTO: 3 líneas explicando cómo se usaría este insight en un anuncio de conversión, qué cifra metería en el hook y qué mecanismo explicaría.

═══════════════════════════════

Repite la estructura para <<INSIGHT 2>>, <<INSIGHT 3>>, <<INSIGHT 4>> e <<INSIGHT 5>>.

REGLAS:
- No inventes cifras. Solo las que aparezcan literalmente en las fuentes.
- Si un insight es bueno pero no tiene dato duro, márcalo como "INSIGHT SIN DATO DURO — NECESITA REFUERZO" y sugiere qué tipo de cifra habría que buscar para robustecerlo.
- Prioriza insights con más munición de datos. Los insights emocionales sin datos van al final.
- Ordena los insights del más cargado de datos al menos cargado.
```

#### 13.1.3 · Prompt 3 — Ángulos

Se pega en: ChatGPT. Sustituir el marcador por los insights de NotebookLM. Devuelve **3 ángulos**, uno por dolor. Elegir uno.

```
Perfecto. He hecho el research en NotebookLM con el prompt que me diste. Aquí están los 5 insights atómicos:

[PEGA AQUÍ LOS 5 INSIGHTS COMPLETOS DE NOTEBOOKLM con sus etiquetas <<INSIGHT 1>>, <<INSIGHT 2>>, etc.]

Ahora, combinando el <<AVATAR>> que ya tienes en memoria con estos insights, dame 3 ÁNGULOS de venta DISTINTOS para el anuncio animado.

Devuelve cada ángulo con esta estructura exacta:

═══════════════════════════════
<<ANGULO 1>>
═══════════════════════════════

TITULAR (1 frase, en lenguaje del cliente).

DOLOR ATACADO: situación concreta del avatar donde este dolor le golpea (recupéralo del avatar).

REFRAME: "Antes el cliente piensa X. Después de ver este anuncio piensa Y."

INSIGHT BASE: cuál de los <<INSIGHT_X>> es el motor de este ángulo (cita el titular del insight).

METÁFORA VISUAL CENTRAL: la imagen mental que carga el ángulo entero. Tiene que ser DIBUJABLE en estilo [pega tu estilo elegido]. No abstracciones poéticas: una imagen concreta.
✅ Ejemplo válido (Pixar): "una columna vertebral que se ilumina en rojo donde duele cuando el personaje duerme mal"
❌ Ejemplo inválido: "la sensación de pesadez del cansancio"

POR QUÉ ESTE ÁNGULO PARARÍA EL SCROLL (3-4 líneas).

═══════════════════════════════

Repite la estructura para <<ANGULO 2>> y <<ANGULO 3>>.

Al final, recomiéndame cuál de los 3 elegir y por qué (1 párrafo).

REGLAS:
- Los 3 ángulos atacan dolores DISTINTOS o usan reframes DISTINTOS. Si los 3 dicen lo mismo con palabras distintas, fallaste.
- Cada metáfora visual tiene que ser DIBUJABLE. Si yo no puedo imaginarla en mi cabeza, no vale.
- Cada ángulo debe beneficiarse específicamente del estilo elegido. Si uno funcionaría mejor en otro estilo, no lo propongas.
```

#### 13.1.4 · Prompt 4 — Guion

Se pega en: ChatGPT. Indicar arriba el ángulo elegido. Devuelve el guion.

```
Vamos con el ángulo elegido: [DI CUÁL: ANGULO 1, 2 o 3].

Construye ahora el GUIÓN del anuncio animado. Storytelling reflexivo, no copywriting agresivo. Voz en off, lectura natural, en español de [MERCADO].

DURACIÓN: 50-60 segundos (140-180 palabras leídas a ritmo natural).
ESTILO: [PEGA TU ESTILO]
ÁNGULO: el que acabamos de elegir.

═══════════════════════════════
LEE PRIMERO ESTOS 2 EJEMPLOS REALES DE GUIONES QUE FUNCIONAN
═══════════════════════════════

────── EJEMPLO 1 — Cloudy (almohada) ──────

"¿Sabías que la primera almohada se inventó hacia el año 7.000 a.C.? Eso son más de 9.000 años. Y, de alguna forma… apenas la hemos cuestionado desde entonces.

Siendo algo en lo que pasamos casi un tercio de nuestra vida, algo que afecta a cómo respiramos, cómo nos recuperamos, y cómo descansa nuestra columna… ¿cómo es que no ha evolucionado de verdad?

En Sleepy nos hicimos exactamente esa misma pregunta. Y decidimos replantear la almohada desde cero.

Presentamos Cloudy. Una almohada ergonómica diseñada de verdad para tu columna. Duermas boca arriba, de lado, o como sea. Cloudy está pensada para mantener tu columna alineada de forma natural toda la noche.

Porque cuando tu columna está bien apoyada, todo cambia. Menos dolor de cuello, espalda y hombros. Menos ronquidos. Incluso ayuda a prevenir arrugas prematuras.

Y es curioso… Algo tan simple que marca una diferencia tan grande.

Si pudiéramos volver 9.000 años atrás y dársela al que inventó la primera almohada, lo haríamos. Pero de momento, te la llevamos directamente a casa.

Prueba Cloudy hoy, sin compromiso."

────── EJEMPLO 2 — FitMind (suplemento cerebral) ──────

"Dicen que eres lo que comes. Pero en realidad… piensas según lo que comes.

Tu cerebro apenas representa un 2% de tu cuerpo, pero consume cerca del 20% de tu energía diaria. Es lo que usas todo el día. Y, aun así, casi nadie se preocupa de alimentarlo bien.

Luego pasa lo de siempre: falta de claridad, poca concentración, esa sensación de estar 'espeso' sin motivo. Y no es casualidad.

Tu cerebro necesita buen combustible. Comida real. Grasas saludables. Omega 3. Nutrientes que de verdad marcan diferencia.

Y también influye el intestino. Si eso no está bien, la cabeza tampoco.

Por eso creamos FitMind. Una forma sencilla de darle a tu cerebro lo que necesita, sin complicarte. Ingredientes respaldados. Energía mental limpia. Sin ingredientes raros.

Lo notas en el día a día. Más claridad. Más enfoque.

Porque cuando el cerebro funciona bien, todo lo demás va detrás."

═══════════════════════════════
LOS 9 PATRONES QUE TIENES QUE REPLICAR
═══════════════════════════════

PATRÓN 1 — HOOK OBLIGATORIAMENTE "verdad MÁS GRANDE que el cliente"

El hook NUNCA habla del cliente directamente. Habla de una verdad externa, anterior, que lo rodea:
- Historia / tiempo transcurrido (9.000 años, 7.000 a.C., décadas)
- Biología / anatomía con cifra (cerebro 20% de energía, 2.500 horas al año)
- Creencia colectiva que se rompe ("dicen que eres lo que comes…")
- Dato científico o contraintuitivo (con cifra concreta)

✅ HOOKS VÁLIDOS (replican el patrón):
- "¿Sabías que tu cara responde a la presión muscular 8 horas cada noche?"
- "Dicen que la estructura facial es genética. Pero en realidad…"
- "Respiramos 25.000 veces al día. Y la mayoría lo hacemos mal."

❌ HOOKS INVÁLIDOS (hablan del cliente directamente, PROHIBIDOS):
- "Estás perdiendo tu cara cada noche" ← habla del tú
- "Tu mandíbula está cambiando" ← habla del tú
- "No sabes por qué te ves peor" ← habla del tú
- "Cada noche empeoras" ← habla del tú

Si tu hook empieza con "Estás…", "Tu…", "Te…", "No sabes…" → MAL. Reescribe.

PATRÓN 2 — DATO TÉCNICO con CIFRA CONCRETA. Nunca "mucho", siempre "20%" o "9.000 años" o "2.500 horas". Si no tienes cifra, invéntala razonable basándote en el insight.

PATRÓN 3 — PREGUNTA REFLEXIVA, no pregunta de venta. La pregunta es la que el cliente se hace a sí mismo, no la que el publicista le lanza.

PATRÓN 4 — PUNTOS SUSPENSIVOS en 3-4 momentos reflexivos ("Y, de alguna forma…", "Pero en realidad…", "Y es curioso…"). Marcan al locutor pensando en alto.

PATRÓN 5 — FRASE PUENTE al producto: "Por eso creamos…" / "En [marca] nos hicimos esa pregunta…". Nunca un corte abrupto al producto.

PATRÓN 6 — PRODUCTO descrito por FUNCIÓN, no por adjetivos. Cero "innovador", "revolucionario", "único". Solo qué es y qué hace.

PATRÓN 7 — BENEFICIOS en 3-4 frases telegráficas paralelas.

PATRÓN 8 — BISAGRA REFLEXIVA OBLIGATORIA antes del cierre: "Y es curioso…", "Al final es simple…", "Y también influye…". NO es opcional. Sin esto suena a anuncio.

PATRÓN 9 — CIERRE con UNA de estas 3 opciones:
A) Vuelta poética al hook + invitación: "Si pudiéramos volver 9.000 años atrás… Pero de momento, te la llevamos a casa. Prueba [X] hoy."
B) Conclusión filosófica corta: "Porque cuando [X] funciona bien, todo lo demás va detrás."
C) Reflexión + invitación suave: "Algo tan simple… que da rabia no haberlo sabido antes. Prueba [X] esta noche."

═══════════════════════════════
ESTRUCTURA OBLIGATORIA DEL GUIÓN
═══════════════════════════════

BLOQUE 1 — HOOK (0-5s, ~12 palabras) → Patrón 1 (verdad MÁS GRANDE)
BLOQUE 2 — DEVELOPMENT (5-18s, ~35 palabras) → Patrones 2 + 3 (dato + pregunta reflexiva)
BLOQUE 3 — INSIGHT/REFRAME (18-30s, ~35 palabras) → Patrón 4 (puntos suspensivos)
BLOQUE 4 — PRODUCTO (30-40s, ~30 palabras) → Patrones 5 + 6 (frase puente + función)
BLOQUE 5 — BENEFICIOS (40-48s, ~20 palabras) → Patrón 7 (frases telegráficas)
BLOQUE 6 — BISAGRA + CIERRE (48-58s, ~25 palabras) → Patrones 8 + 9 (bisagra reflexiva + cierre)

═══════════════════════════════
AUTO-VERIFICACIÓN ANTES DE DEVOLVER
═══════════════════════════════

Antes de devolverme el guión, verifica:

☐ ¿El HOOK habla de algo MÁS GRANDE que el cliente (historia, biología, creencia colectiva)?
☐ ¿El HOOK evita empezar con "Estás…", "Tu…", "Te…", "No sabes…"?
☐ ¿Hay al menos UN dato con cifra concreta en el BLOQUE 2?
☐ ¿Uso puntos suspensivos en 3-4 momentos reflexivos?
☐ ¿La frase puente al producto suena natural (Patrón 5)?
☐ ¿El producto se describe por FUNCIÓN sin adjetivos vacíos?
☐ ¿Los beneficios son 3-4 frases telegráficas paralelas?
☐ ¿Hay una BISAGRA REFLEXIVA obligatoria antes del cierre?
☐ ¿El cierre usa UNA de las 3 opciones del Patrón 9?

Si alguna casilla está sin marcar, REESCRIBE antes de devolverme.

═══════════════════════════════
FORMATO DE SALIDA
═══════════════════════════════

<<GUION>>

[HOOK · 0-5s]
[texto exacto]
(intención emocional)

[DEVELOPMENT · 5-18s]
[texto]
(intención emocional)

[INSIGHT/REFRAME · 18-30s]
[texto]
(intención emocional)

[PRODUCTO · 30-40s]
[texto]
(intención emocional)

[BENEFICIOS · 40-48s]
[texto]
(intención emocional)

[BISAGRA + CIERRE · 48-58s]
[texto]
(intención emocional)

CONTEO TOTAL: [X palabras]
DURACIÓN ESTIMADA: [X segundos]

</<GUION>>

<<HOOKS_ALTERNATIVOS>>
3 hooks alternativos al del guión. TODOS tienen que cumplir el Patrón 1 (verdad MÁS GRANDE que el cliente). Cada uno con una fórmula DISTINTA:
1. [HOOK con fórmula "¿Sabías que [dato histórico/biológico]?"]
2. [HOOK con fórmula "Dicen que [creencia]. Pero en realidad [reframe]."]
3. [HOOK con fórmula "[Dato biológico/científico/histórico]" sin pregunta, frase directa]
</<HOOKS_ALTERNATIVOS>>

REGLAS BRUTALES:
- Cero exclamaciones. Cero MAYÚSCULAS para énfasis.
- Palabras prohibidas: "descubre", "transforma tu vida", "revolucionario", "el futuro de", "única en el mercado", "increíble", "asombroso", "no creerás".
- Si una frase no aporta dato, mecanismo, reframe o reflexión, BÓRRALA.
- Las palabras del avatar y de los insights deben aparecer LITERALMENTE en al menos 2 puntos del guión.
- El locutor habla como un amigo más informado. Nunca como un publicista.
- TEST FINAL: si lees el guión en voz alta y suena a anuncio, está mal. Si suena a alguien contándote algo en una cena, está bien.
```

#### 13.1.5 · Prompt 5 — Storyboard (escenas)

Se pega en: ChatGPT. Devuelve la estructura visual y la metáfora visual. Punto de iteración fuerte.

```
Vamos a construir el STORYBOARD del anuncio a partir del <<GUION>> que acabamos de cerrar.

⚠️ IMPORTANTE: en este paso NO vamos a escribir prompts de NanoBanana todavía. Solo storyboard. Cinematográfico. Bien pensado. Con la metáfora visual del ángulo clavada en el centro.

Quiero que trates este paso como un director de arte trabajando con un storyboard artist. No como un asistente generando contenido rápido.

═══════════════════════════════════════════════════════════
PASO 0 (OBLIGATORIO) — PLAN VISUAL ANTES DE ESCRIBIR ESCENAS
═══════════════════════════════════════════════════════════

Antes de describir ninguna escena, piensa EN VOZ ALTA (devuélvemelo escrito) sobre estas 5 preguntas:

1. METÁFORA VISUAL CENTRAL: ¿cuál era la metáfora visual del <<ANGULO>> elegido? ¿En qué 2-3 escenas concretas se va a manifestar? (Si solo la usas 1 vez, la desperdicias. Si la usas en todas, la saturas.)

2. MOMENTO ICÓNICO (THE MONEY SHOT): ¿cuál va a ser LA imagen de este anuncio? La que si la vieras fija en un feed te haría parar. Diséñala explícitamente. Esta escena tiene que ser visualmente distinta y memorable. Sitúala entre la escena 2 y la 4.

3. PROGRESIÓN VISUAL: ¿cómo evoluciona visualmente el anuncio? Escribe una frase que describa el ARCO VISUAL completo (ej: "empieza íntimo y real → se vuelve conceptual y abstracto → acaba volviendo a lo real pero transformado"). Si no hay arco, hay planitud.

4. CONTRASTE DE PLANOS: lista qué tipos de plano vas a usar y en cuántas escenas cada uno. Tiene que haber al menos: 1 wide shot, 2 close-ups, 1 macro/detalle, 1 overhead/cenital, 1 conceptual sin personaje. Si todos los planos son del mismo tipo, el anuncio es plano.

5. ESCENAS CONCEPTUALES (MODE A): identifica 1-2 escenas que van a ser puramente simbólicas/conceptuales (sin personaje), para romper la linealidad narrativa. ¿Qué simbolizan y dónde van situadas en la secuencia?

Devuélveme esto en un bloque titulado:

<<PLAN_VISUAL>>
1. Metáfora visual central: [cómo la vas a usar y en qué escenas]
2. Momento icónico: [descripción de LA imagen clave, en qué escena va]
3. Arco visual: [una frase describiendo la progresión]
4. Contraste de planos: [lista concreta con conteos]
5. Escenas conceptuales: [cuáles y qué simbolizan]
</<PLAN_VISUAL>>

Si al pensarlo detectas que la metáfora visual del ángulo es floja o poco explotable, AVISA antes de seguir. Si todo está sólido, continúa.

═══════════════════════════════════════════════════════════
REGLAS DE ESCRITURA DEL STORYBOARD
═══════════════════════════════════════════════════════════

REGLA 1 — UNA ESCENA = UNA IDEA VISUAL
Si una escena tiene dos ideas, divídela en dos escenas. Mejor 14 escenas claras que 8 escenas cargadas.

REGLA 2 — CADA DESCRIPCIÓN VISUAL ES DIBUJABLE
No escribas "siente frustración". Escribe "frunce el ceño, aprieta los puños sobre la sábana, respira profundo".

REGLA 3 — DURACIÓN POR ESCENA = 4-6 SEGUNDOS
Cada clip Kling es de 5 segundos. Cada escena cubre 4-6 segundos del guión. Si un bloque del guión dura 12 segundos, son 2-3 escenas, no una.

REGLA 4 — COHERENCIA DE PERSONAJE Y ENTORNO
El personaje principal aparece IDÉNTICO en cada escena (mismo pelo, ropa, edad). Los entornos repetidos (dormitorio, baño, oficina) también son idénticos entre escenas.

REGLA 5 — TRANSICIONES PENSADAS
Cada escena propone cómo conecta visualmente con la siguiente (fade, match cut, zoom-in al detalle, cambio de plano, fade a negro).

REGLA 6 — DOS TIPOS DE ESCENA:
- NARRATIVA: con personaje en su mundo (dormitorio, baño, etc.)
- CONCEPTUAL / MODE A: simbólica, sin personaje o con personaje en contexto abstracto (mecanismo interno, infografía estilizada, símbolo aislado)

Debe haber mezcla de ambas.

REGLA 7 — LA ESCENA FINAL VUELVE AL INICIO TRANSFORMADA
El cierre visual suele funcionar mejor si retoma un elemento de la primera escena pero con un cambio (misma persona pero más segura, mismo espejo pero con otra luz, misma cama pero con el producto).

═══════════════════════════════════════════════════════════
FORMATO DE SALIDA DEL STORYBOARD
═══════════════════════════════════════════════════════════

Después del <<PLAN_VISUAL>>, devuélveme cada escena con este formato EXACTO:

───────────────────────────────
ESCENA [N]
───────────────────────────────

BLOQUE DEL GUIÓN: [HOOK / DEVELOPMENT / INSIGHT / PRODUCTO / BENEFICIOS / CIERRE]
VOZ EN OFF QUE CUBRE: [fragmento exacto del guión en español]
DURACIÓN: [4-6 segundos]
TIPO DE ESCENA: [NARRATIVA / CONCEPTUAL]

DESCRIPCIÓN VISUAL (4-6 líneas, cinematográfica y dibujable):
- QUIÉN aparece: [personaje con descripción física concreta O sujeto conceptual]
- DÓNDE: [entorno con paleta de color y elementos clave]
- QUÉ hace: [acción concreta en presente, no emociones abstractas]
- CÓMO se ilumina: [tipo de luz, dirección, temperatura de color]
- PLANO: [close-up / medium shot / wide shot / macro / overhead / low angle / POV]
- DETALLE MEMORABLE: [el elemento visual que hace esta escena única, su "gancho visual"]

MODE DE REFERENCIA: [A / B / C / D]
(A = no reference, B = character reference, C = environment reference, D = full continuity)

FRAME TYPE EN KLING: [SINGLE FRAME / START + END FRAMES]
(START+END si hay movimiento significativo, SINGLE si es estático o el movimiento es mínimo)

TRANSICIÓN A LA SIGUIENTE: [descripción visual concreta de cómo conecta]

───────────────────────────────

Repite para todas las escenas hasta cubrir el guión entero.

═══════════════════════════════════════════════════════════
AL FINAL DEL STORYBOARD
═══════════════════════════════════════════════════════════

Devuélveme un RESUMEN ESTRUCTURAL:

TOTAL ESCENAS: [X]
ESCENAS NARRATIVAS: [X]
ESCENAS CONCEPTUALES (MODE A): [X]
DISTRIBUCIÓN DE PLANOS:

Close-ups: [X]
Medium shots: [X]
Wide shots: [X]
Macro/detalle: [X]
Overhead/cenital: [X]
Otros: [X]

ESCENA DEL MOMENTO ICÓNICO: ESCENA [N]
ESCENAS QUE USAN LA METÁFORA VISUAL CENTRAL: [N, N, N]

═══════════════════════════════════════════════════════════
REGLAS BRUTALES FINALES
═══════════════════════════════════════════════════════════

- Si no hay variedad de planos (ej: todo medium shots) → el storyboard está mal. Rehazlo.
- Si la metáfora visual del ángulo solo aparece en 1 escena → la estás desperdiciando.
- Si no hay escena conceptual MODE A → el anuncio va a ser plano narrativamente.
- Si la escena final no retoma un elemento de la primera → pierdes el cierre circular.
- Si alguna escena tiene descripción vaga tipo "muestra el problema" → MAL, describe exactamente qué se ve.

Pregúntame si algo no está claro ANTES de empezar a escribir. No asumas.
```

#### 13.1.6 · Prompt 6 — Prompts de imagen (NB)

Se pega en: ChatGPT. **En el bloque Style Lock dejar solo el estilo elegido** y borrar los demás.

```
Perfecto. El <<STORYBOARD>> está cerrado. Ahora conviértelo en PROMPTS NANOBANANA PRO.

Una imagen por escena. Cada escena = un prompt.

ESTILO ANIMACIÓN: [PEGA TU ESTILO ELEGIDO]

═══════════════════════════════════════════════════════════
REGLAS GLOBALES
═══════════════════════════════════════════════════════════

1. Todos los prompts 100% en INGLÉS (etiquetas y valores).

2. STYLE LOCK: una sola frase, según el estilo elegido:
- Pixar 3D → "Pixar 3D animation style"
- Apple → "Apple-style cinematic product photography"
- Sci-fi → "Sci-fi 3D animation style"
- Claymation → "Stop-motion claymation style"
- Wes Anderson → "Wes Anderson cinematic style"

3. Cada prompt va en su propio bloque de código independiente (triple backtick) para copiar con un click.

4. Para mantener al personaje consistente entre escenas, pasamos la imagen anterior como referencia. La primera vez que aparece el personaje, lo describes a fondo. Las siguientes, solo dices qué cambia.

═══════════════════════════════════════════════════════════
ADVERTENCIAS TÉCNICAS
═══════════════════════════════════════════════════════════

NanoBanana Pro NO hace bien:
- Texto legible dentro de la imagen → genera sin texto, añádelo en CapCut
- Más de 2 caras detalladas en el mismo frame

SÍ hace bien:
- Split screens y comparativas
- Mecanismos internos estilizados
- Composiciones simétricas

Si el storyboard pide texto legible o multitud de caras, AVISA y propón alternativa.

═══════════════════════════════════════════════════════════
FORMATO DE SALIDA
═══════════════════════════════════════════════════════════

Devuélveme un bloque de código por cada escena del storyboard, en orden. Nada más. Sin títulos de escena, sin descripciones en español, sin notas. Solo los bloques de código con los prompts, uno detrás de otro.

Cada bloque de código con este formato:

[STYLE LOCK]: [paste]
[SUBJECT]: [English]
[ACTION]: [English, present continuous]
[ENVIRONMENT]: [English]
[LIGHTING]: [English]
[CAMERA]: [close-up / medium shot / wide shot / macro / top-down / low angle]
[ASPECT]: 9:16 vertical
[REFERENCE]: [si aplica: "Use image from Scene X. Keep [what] identical. Change [what]." Si no aplica: "none"]
[EXCLUDE]: no text, no logos, no watermarks, no blurry artifacts, no extra limbs, no distorted faces

Al final de todos los bloques, un aviso corto si hay problemas técnicos (texto en imagen o multitud de caras). Si no hay problemas, no escribas nada.

═══════════════════════════════════════════════════════════
AUTO-VERIFICACIÓN
═══════════════════════════════════════════════════════════

☐ ¿Todos los valores en inglés?
☐ ¿Style lock es una sola frase corta?
☐ ¿Cada prompt en su propio bloque de código, sin nada en medio?
☐ ¿Una sola imagen por escena?
☐ ¿La primera vez que aparece el personaje lo describo completo, y después solo lo que cambia con referencia a la escena anterior?
☐ ¿Lo mismo para entornos que se repiten?

Si algo falla, corrige antes de devolvérmelo.
```

#### 13.1.7 · Prompt 7 — Auditoría completa FINAL

Se pega en: ChatGPT. Devuelve diagnóstico + guion definitivo + **2 variantes** + storyboard y prompts auditados.

```
Stop. Antes de generar ninguna imagen en NanoBanana, vamos a hacer la auditoría final. Y esta vez no quiero que te quedes en "mejorar". Quiero que eleves el anuncio al nivel de un CORTOMETRAJE ANIMADO DE AUTOR.

Lee bien esta primera parte porque define el nivel al que vamos a trabajar.

═══════════════════════════════════════════════════════════
EL NIVEL QUE ESTAMOS BUSCANDO — CINE ANIMADO DE VERDAD
═══════════════════════════════════════════════════════════

Esto NO es publicidad animada. Es un mini-cortometraje de 50 segundos que por casualidad vende un producto. El referente son los cortos de Pixar, Laika, Aardman y los ads cinematográficos tipo Apple.

Antes de escribir nada, mete en tu cabeza lo que hacen estos cortos. Son tus referencias obligatorias:

PIPER (Pixar, 2016) — Un pollito aprende del mar. 6 minutos. No hay palabras. Lo que enseña: primeros planos extremos con textura brutal. Emoción transmitida por ojos y movimiento, no por diálogo. La cámara es un personaje más.

BAO (Pixar, 2018) — Una madre crea un dumpling que cobra vida. Lo que enseña: convertir un objeto cotidiano en un personaje emocional. Metáfora pura. El objeto TIENE ALMA y se gana el cariño del espectador en segundos.

INSIDE OUT (Pixar, 2015) — Las emociones como personajes dentro de un mundo interno. Lo que enseña: lo abstracto se vuelve visitable. Un sentimiento es un lugar. Una idea es un edificio. Un problema es una criatura.

LA LUNA (Pixar, 2011) — Un niño descubre que barre estrellas en la luna. Lo que enseña: mundos mágicos con reglas propias. Lo cotidiano se transforma en surreal sin previo aviso.

PAPERMAN (Disney, 2012) — Un hombre persigue a una mujer con aviones de papel. Lo que enseña: metáfora visual sostenida durante todo el corto. Un solo símbolo lleva toda la emoción.

COIN OPERATED (Pixar SparkShorts) — Un niño guarda monedas toda su vida para un viaje espacial. Lo que enseña: narrativa sin palabras, emoción brutal en 5 minutos, personaje que envejece visualmente.

KIWI! (Dony Permedi) — Un kiwi corta árboles en una montaña para simular volar cuando se tira. Lo que enseña: la última escena cambia TODO el significado del corto. El giro visual como moneda emocional.

APPLE "UNDERDOGS" y "THE WHOLE WORKING FROM HOME THING" — Lo que enseña: un anuncio largo puede ser un cortometraje con personajes que te importan. El producto aparece como parte de la vida, no como interrupción.

APPLE "INTENTION" (2022) — Apple + Pride. Lo que enseña: iluminación como narrativa. La luz cuenta la historia antes que los planos.

CHIPOTLE "BACK TO THE START" — Un granjero y su granja industrializada. Stop-motion 2 minutos. Lo que enseña: el arco emocional completo de un cortometraje en 120 segundos. Problema, crisis, redención.

Principios comunes a todos estos cortos:
- La cámara se mueve con intención. No es un testigo, es un narrador.
- Los objetos cotidianos se vuelven metáfora. Una lámpara es esperanza. Un sillón es nostalgia.
- Los primeros planos son brutales, con textura, con imperfección humana.
- Lo abstracto se materializa. Un pensamiento es un lugar. Un sentimiento es una criatura.
- La luz cuenta la mitad de la historia.
- Hay UN momento icónico. Una imagen que si la ves suelta, te dice qué es el corto.
- El final cierra circularmente con el principio, pero transformado.

SI LO QUE VAS A ENTREGAR NO CUMPLE ESTOS PRINCIPIOS, NO LO ENTREGUES. REESCRÍBELO.

═══════════════════════════════════════════════════════════
TU TAREA — DOS AUDITORÍAS Y UNA ENTREGA FINAL
═══════════════════════════════════════════════════════════

Vas a hacer DOS auditorías (guión y visual) y entregar UN output definitivo. En este orden exacto.

───────────────────────────────────────────────────────────
AUDITORÍA 1 — GUIÓN
───────────────────────────────────────────────────────────

Re-lee el <<GUION>> completo de la conversación anterior. Pregúntate:
- ¿El HOOK realmente para el scroll o es solo "correcto"?
- ¿El dato duro es el más potente del research?
- ¿El insight/reframe cambia la cabeza del cliente o solo repite lo que ya sabe?
- ¿La frase puente al producto fluye o suena forzada?
- ¿Los beneficios son concretos o son clichés?
- ¿La bisagra reflexiva tiene peso real?
- ¿El cierre deja algo al espectador?

Entrega el resultado así:

<<GUIÓN DEFINITIVO>>
El guión mejorado entero DENTRO de UN ÚNICO bloque de código (triple backtick). Todo el texto corrido, con los bloques [HOOK · 0-5s], [DEVELOPMENT · 5-18s], etc. visualmente separados por saltos de línea pero dentro del MISMO bloque de código, para copiarlo de un click.

<<VARIANTE DE GUIÓN A>>
Una alternativa COMPLETAMENTE DISTINTA del definitivo. Otro ángulo, otro tono, otra estructura. No una versión retocada. Un guión paralelo, en su propio bloque de código.

<<VARIANTE DE GUIÓN B>>
Otra alternativa también completamente distinta del definitivo y de la variante A. Tercer ángulo, tercera aproximación. En su propio bloque de código.

El usuario elegirá uno de los 3 para producir.

Después de los 3 bloques de código, añade una línea breve explicando en qué se diferencian:
"Definitivo apuesta por [X]. Variante A apuesta por [Y]. Variante B apuesta por [Z]."

───────────────────────────────────────────────────────────
AUDITORÍA 2 — LO VISUAL (prompts y cortometraje global)
───────────────────────────────────────────────────────────

Re-lee las 3 variantes de storyboard y los prompts NanoBanana de la conversación anterior. Audítalo todo desde la mirada de un director de cortometraje Pixar.

Preguntas críticas:
- ¿Este anuncio abriría un corto de Pixar, o abriría un banner de Facebook?
- ¿Hay alguna escena que si la sacara de contexto parecería un frame de Inside Out, Bao o Piper? ¿Cuántas?
- ¿Hay escenas que son INFOGRAFÍA DISFRAZADA (dos almohadas aisladas, un modelo anatómico en fondo neutro, un gráfico con cifras)? Esto es el pecado capital. Marca todas.
- ¿Hay UN momento icónico que justifique el anuncio entero? Si hay que pausar el vídeo en ese frame, ¿funciona como póster?
- ¿La cámara se mueve con intención cinematográfica o es una cámara pasiva que registra?
- ¿La iluminación cuenta historia o es solo "luz bonita"?
- ¿Los objetos cotidianos se convierten en metáfora visual (el pillow tiene alma, el cuello es un paisaje), o todo es literal?
- ¿Hay escenas que podrían ser CUALQUIER anuncio de cualquier producto? Eso es fallo.

Y crítico para tu técnica de producción one-shot:
- ¿Cada par consecutivo de imágenes es visualmente encadenable? Si la imagen 3 es un dormitorio azul y la imagen 4 es un fondo blanco abstracto, el corte es imposible de animar. Identifica los saltos rotos.

Entrega el resultado así:

<<DIAGNÓSTICO VISUAL>>
Máximo 10 líneas. Lista concreta: "Escena X es infografía disfrazada. Propuesta: convertirla en [descripción cinematográfica]". "Entre escena Y y Z hay salto visual imposible. Propuesta: escena puente que [descripción]". "Falta momento icónico. Propuesta: escena [N] reformulada como [descripción tipo Pixar]". Sin decorado.

<<STORYBOARD DEFINITIVO>>
Reconstruye el storyboard desde cero con el nivel de los cortos referenciados arriba. Cada escena con el formato:

───────────────────────────────
ESCENA [N]
───────────────────────────────

BLOQUE DEL GUIÓN: [HOOK / DEVELOPMENT / INSIGHT / PRODUCTO / BENEFICIOS / CIERRE]
VOZ EN OFF QUE CUBRE: [fragmento exacto del guión]
DURACIÓN: [4-6 segundos]
TIPO DE ESCENA: [NARRATIVA / CONCEPTUAL]

QUÉ PASA: descríbelo como si fuera un frame de Pixar. Qué hace la cámara, qué hace el personaje u objeto, qué cambia en la luz. Narrativo, cinematográfico.

CÓMO SE SIENTE: qué emoción transmite esta escena.

REFERENCIA MENTAL: menciona qué corto/escena del mundo real te inspira para esta escena (ejemplo: "similar al primer plano del pollito en Piper cuando ve el mar por primera vez", "composición tipo Inside Out donde las emociones son personajes", etc.).

CONTINUIDAD ONE-SHOT: qué elemento visual de la escena anterior se mantiene al inicio de esta, y qué elemento de esta se traslada a la siguiente. Crítico para la técnica start/end encadenado.

───────────────────────────────

Escribe TODAS las escenas necesarias. No agrupar. No resumir.

<<PROMPTS NANOBANANA DEFINITIVOS>>
Cada prompt en su propio bloque de código independiente. En inglés 100%. Formato:

[STYLE LOCK]: [pega el style lock del estilo elegido]
[SUBJECT]: [detalle visual específico, en inglés, cargado de textura cinematográfica]
[ACTION]: [acción presente continuo con dinamismo, en inglés]
[ENVIRONMENT]: [entorno con paleta de color precisa, en inglés]
[LIGHTING]: [iluminación con intención narrativa, en inglés — no "good lighting", sino "warm golden rim light from the window mimicking early morning melancholy"]
[CAMERA]: [tipo de plano y ángulo específicos, con movimiento si aplica]
[ASPECT]: 9:16 vertical
[REFERENCE]: [si aplica: "Use image from Scene X. Keep [X] identical. Change [Y]." Si no aplica: "none"]
[EXCLUDE]: no text, no logos, no watermarks, no blurry artifacts, no extra limbs, no distorted faces

═══════════════════════════════════════════════════════════
REGLAS ANTI-ATAJO — OBLIGATORIAS
═══════════════════════════════════════════════════════════

PROHIBIDO:
- "(…continúan igual con mejoras consistentes…)"
- "el resto se mantiene parecido"
- Agrupar 2 prompts en un bloque
- Saltarte escenas o prompts
- Frases decorativas al final tipo "esto ya es un mini-cortometraje brutal"

Si te falta espacio: NO resumas. Entrega lo que puedas entero y escribe "CONTINUAR EN SIGUIENTE MENSAJE: prompts del X al Y". Cuando yo diga "continúa", me entregas el resto.

═══════════════════════════════════════════════════════════
AUTO-VERIFICACIÓN FINAL ANTES DE ENVIAR
═══════════════════════════════════════════════════════════

☐ ¿Entregué el guión definitivo en UN solo bloque de código?
☐ ¿Entregué 2 variantes de guión completamente distintas entre sí, cada una en su bloque?
☐ ¿Expliqué en qué se diferencia cada guión?
☐ ¿Diagnóstico visual con máximo 10 líneas de problemas concretos?
☐ ¿Storyboard reconstruido al nivel de los cortos referenciados?
☐ ¿Cada escena del storyboard tiene una REFERENCIA MENTAL a un corto real?
☐ ¿Cada escena tiene CONTINUIDAD ONE-SHOT explicada?
☐ ¿TODOS los prompts NanoBanana entregados uno por uno?
☐ ¿Cada prompt en su bloque de código, en inglés?
☐ ¿Cada par consecutivo de prompts es visualmente encadenable?

Si alguna casilla falla, CORRIGE antes de enviar.

═══════════════════════════════════════════════════════════
PRINCIPIO FINAL
═══════════════════════════════════════════════════════════

Si lo que vas a entregar parece "un anuncio bien hecho", para y reescríbelo. El objetivo es una pieza que un director de Pixar Sparkshorts aceptaría como primer pitch.

No me entregues un anuncio. Entrégame un cortometraje.
```

#### 13.1.8 · Prompt 8 — Introducción al producto

Se pega en: ChatGPT. Inyectar nombre de producto, marca y 2-3 frases. Devuelve el entregable final.

```
Perfecto. Hasta ahora hemos trabajado con placeholder del producto. Te paso el producto REAL. Con la información mínima. El resto lo deduces tú a partir de toda la conversación anterior (avatar, insights, ángulo elegido, guión y storyboard auditados).

PRODUCTO:
NOMBRE: [Ej: Cloudy]
QUÉ ES EN UNA FRASE: [Ej: Una almohada ergonómica de la marca Sleepy diseñada para mantener la columna alineada durante toda la noche]

Con esto y TODO el contexto que ya tienes de nuestra conversación, entrégame AHORA la versión FINAL del anuncio personalizada con este producto. Cero genérico.

Quiero la estructura completa del anuncio premium, pensada, afinada y mejorada. En este formato exacto:

1) <<GUIÓN DEFINITIVO>>
El guión entero dentro de UN ÚNICO bloque de código, con el nombre del producto bien integrado, la frase puente al producto mencionando la marca de forma natural, y todos los beneficios alineados con lo que el producto realmente promete (deducido por ti desde el contexto previo).

2) <<VARIANTE A>>
Un guión alternativo completamente distinto en ángulo y tono. En su propio bloque de código.

3) <<VARIANTE B>>
Otro guión alternativo, distinto del definitivo y de la variante A. En su propio bloque de código.

Después de los 3 bloques, explica en 3 líneas en qué se diferencia cada uno.

4) <<ESTRUCTURA DEL ANUNCIO PREMIUM>>
La estructura narrativa-visual final del anuncio para el guión definitivo. Escena por escena, qué pasa, qué siente el espectador, cómo encadena con la siguiente. Para que yo tenga clarísimo el mini-cortometraje antes de producir.

5) <<PROMPTS NANOBANANA PRO FINALES>>
Cada prompt en su propio bloque de código independiente, en inglés. TODOS. Uno por uno. Sin atajos, sin "el resto igual", sin agrupar.

En cada prompt donde aparezca físicamente el producto, añade al final esta línea:
[REFERENCE IMAGE]: insert real product photo here

Porque yo adjuntaré la foto real del producto en NanoBanana al generar esas imágenes. Así NanoBanana usa la foto real en vez de inventarse el producto.

═══════════════════════════════════════════════════════════
REGLAS ANTI-ATAJO
═══════════════════════════════════════════════════════════

- Entrega TODOS los prompts enteros, uno a uno, sin resumir.
- Prohibido "(continúan igual con ajustes)", "aplicar misma lógica", agrupar 2 en un bloque.
- Si te falta espacio: escribe "CONTINUAR EN SIGUIENTE MENSAJE" y yo te digo "continúa".
- Nada de frases decorativas al final tipo "esto ya es un anuncio premium".

═══════════════════════════════════════════════════════════

AUTO-VERIFICACIÓN ANTES DE ENVIAR:
☐ ¿Integré el nombre del producto con naturalidad en el guión?
☐ ¿Deduje la marca, tono, beneficios y diferenciales desde el contexto previo sin inventar?
☐ ¿Las 3 versiones (definitivo + A + B) son genuinamente distintas?
☐ ¿Los prompts NanoBanana donde aparece el producto físico tienen [REFERENCE IMAGE]?
☐ ¿Entregué TODOS los prompts uno a uno, ninguno agrupado ni resumido?
```

### 13.2 · Menú de estilos y transiciones

Es el prompt del clip en **Kling 3**, uno por cada par de imágenes consecutivas. Va **en inglés a propósito**:
lo lee el modelo de vídeo, no ChatGPT. Se usa el que corresponde al estilo elegido en el Prompt 1, el mismo para
todos los clips del anuncio. Los cinco terminan en `sound effects (no talking)` — el equivalente animado de la
regla `NO TALKING` del track realista [M4-L4.3].

**Realista**

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
