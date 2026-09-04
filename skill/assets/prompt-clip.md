# Plantilla · prompt de clip

Copiar y rellenar. Prompts en inglés; el guion, en español.

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

**Colocación del gesto** — antes de hablar va delante del `says:`; mientras habla, detrás:

```
The person [acción], then looks at the camera and says: "[guión]"
The person says: "[guión]" [acción]
```

**Modificadores de tiempo:**
- `While speaking, {acción}` — durante el habla.
- `{acción} while saying in the first 3 seconds of the video:` — acotado.

**Si el avatar no habla, el prompt empieza por `NO TALKING.`** y no lleva GUION, VOZ ni ACENTO.

---

## Cámara

**★ Cámara quieta + gestos — el más usado**
```
(static camera, no movement) realistic arm movements and subtle micro-movements. Single continuous take, no cuts or scene changes.
```

**Plano fijo**
```
Locked-off static shot, camera completely still on a tripod, no movement at all. Single continuous take, no cuts or scene changes.
```

**Zoom lento a la cara** — el del CTA
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

**Seguimiento al caminar**
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

**Bokeh**
```
Shallow depth of field with a creamy bokeh background, slow push-in on the in-focus subject, then holding. Single continuous take, no cuts or scene changes.
```

**Cámara lenta**
```
Slow-motion delivery, smooth and cinematic, with a subtle camera drift. Single continuous take, no cuts or scene changes.
```

**Plano propio** — pegar al final para que no meta un corte:
```
single continuous take, no cuts or scene changes — the camera holds steady on the framing after the move
```

**Añadir cámara en mano a cualquier clip:**
```
Add subtle handheld camera movement throughout the shot, as if another person is casually filming. Keep the movement minimal, natural, and realistic, with slight handheld sway only.
```

---

## Micro-acciones

| Inglés | Español |
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
| `points up` / `points up to the left` / `points to the right` | señala arriba / izquierda / derecha |
| `crosses their arms` | cruza los brazos |
| `shrugs` | se encoge de hombros |
| `gives a thumbs up` | pulgar arriba |
| `claps once` | da una palmada |
| `tilts their head curiously` | inclina la cabeza con curiosidad |
| `taps their chin thoughtfully` | se toca la barbilla |
| `snaps their fingers` | chasquea los dedos |
| `rolls their eyes playfully` | pone los ojos en blanco, en broma |

Se combinan: `The person adjusts their cap, then says: "[guión]" and smiles.`

---

## Voz

Usar la **misma línea `Voice:`** en todos los clips del mismo personaje y en la misma sesión.

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

Forma corta usada en la práctica: `Voice: light female voice, mid-20s, bright.`

**Para inventar otra**: género + edad + gravedad (`deep, low` | `bright, high`) + textura
(`gravelly, raspy` | `smooth, clean` | `soft, breathy`) + entrega (`calm and slow` | `energetic and fast` |
`warm` | `authoritative`).

---

## Acento

El latino neutro sale por defecto. **El de España hay que pedirlo siempre.**

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

## Dualcast · doble bloque

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

Sin el segundo bloque el modelo hace hablar a los dos o congela al que escucha.

## Podcast · reacciones del que escucha

```
[He nods in agreement with what she has just heard and says:]
[She pauses for a moment as if thinking about her answer, then says]:
[She nods in agreement while saying:]
```

## UGC a cámara · variantes cortas

Cuando no hace falta el bloque completo de arriba.
```
(static camera, no movement) he/she's looking directly at the camera, realistic arm movements, clear influencer tone: "[inserta el guión aquí]"
```
```
realistic arm movements, the woman/man says exactly with direct clear energy: "[inserta el guión aquí]"
```

Con el producto dentro del clip:
```
Using the product from the reference image, the person holds the product in one hand and shows it to the camera while talking, looking at the camera with natural, realistic gestures. Keep the product's label and packaging clearly visible and unchanged. Single continuous take, no cuts.
```
```
Using the product from the reference image, while talking to the camera the person naturally points at the product and glances down at it a couple of times, then back to the camera, with relaxed, realistic gestures. Keep the product's label and packaging clearly visible and unchanged. Single continuous take, no cuts.
```
```
Using the product from the reference image, a clean beauty shot of the product on a [surface: marble counter / wooden table / neutral backdrop], slow gentle camera move, soft natural lighting, the product in sharp focus with its label clearly visible and unchanged. No people. Single continuous take, no cuts.
```

## Clips sin habla · plantilla y banco de planos

Plantilla:
```
[movimiento de cámara], cinematic, no talking. Keep the SAME person from the reference. She [acción]. [sitio + luz]. No text, no watermark.
```

Seis planos de apoyo listos para copiar:
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

## Skincare · extender la crema

La IA deja la crema flotando o la multiplica. Hay que pedir que la cantidad visible decrezca:
```
While speaking, she gradually blends the visible cream into the [aquí el sitio] until it is smoothly absorbed into the skin. The amount of visible cream continuously decreases throughout the clip, leaving no residue, streaks, or buildup.
```

## Podcast · clip base y candado

Una intervención:
```
(static camera, no movement) the person talks naturally with realistic micro-movements and subtle arm gestures, authentic conversational energy. They say: "[inserta el guión aquí]"
```

Si en la imagen se ve a los dos, el modelo tiende a hacer hablar a ambos. Candado:
```
Single speaker: only the person from the reference image talks.
```

El ángulo de mirada se pide en **la imagen**, no en el clip:
```
She/he is looking to the right/left side of the frame, as if talking to someone sitting next to her/him.
```
