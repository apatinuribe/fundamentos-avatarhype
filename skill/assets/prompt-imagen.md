# Plantillas · prompts de imagen

Siempre **9:16 y 2K**. Las imágenes que se van a superponer en edición, en **1:1**.
Con imagen de referencia, elegir la entrada **imagen a imagen**.

---

## Método 6C — estructura de una descripción de avatar

```
C1 Character           — personaje: edad, vibe, atractivo, detalles de cara
C2 Camera              — cámara: POV, ángulo, lente, encuadre (realismo de iPhone)
C3 Clothing            — ropa: outfit, styling, accesorios
C4 Context             — escena: localización y detalles de fondo
C5 Cinematic Light     — luz: tipo de flash, sombras, grano, mood
C6 Consistency Anchors — anclajes de realismo, restricciones y limpieza
```

Diseñar el avatar **imperfecto**: piel con textura, cara no simétrica. Omni añade su propia capa de textura al
animar, y un avatar impoluto acaba cantando a IA.

---

## Cambiar el aspecto de la misma persona

```
Using this image as reference, keep the SAME person — same face and identity — and make [DESCRIPCIÓN]. Photorealistic, natural skin texture and lighting.
```

`[DESCRIPCIÓN]` admite español: *en el baño una foto muy cerca de su cara con acné, lleva una camiseta blanca.*

---

## Siguiente estado de la misma escena

Patrón: editar la anterior + listar **explícitamente** lo que no cambia + pedir el fotograma siguiente.

```
Edit the reference image. Keep everything exactly the same.
{lo que cambia}
Do not change her face, outfit, {escena}, lighting, camera angle, framing, composition, or the {producto} packaging.
The result should look like the next frame of the same video.
```

**Blindaje de packaging de marca** — añadir siempre que haya etiqueta:
```
without changing the branding, colors, typography, or label
```

---

## Quitar a la persona y dejar el producto

```
Edit the reference image. Remove the woman and everything she is using. Keep the kitchen, lighting, camera angle, framing, and composition exactly the same. Place the closed {PRODUCTO} container in the center of the countertop where she was standing, using the exact packaging from the reference without changing the branding, colors, typography, or label. The countertop should look naturally clean, with no artifacts.
```

---

## Reciclar el encuadre para otra escena

```
Edit the reference image.

Keep the exact same woman, {escena}, clothing, countertop, camera angle, framing, perspective, lighting, shadows, background, and overall composition.

Replace {objeto A} with {objeto B} placed naturally in the same area.

{detalle de B}

{qué hace ahora la persona}

Everything else must remain identical. The final image should look like the next natural moment in the same scene, captured with the same iPhone camera, without changing the environment or composition.
```

---

## Insertar el packaging real sobre una escena generada

Tres referencias: character sheet + escena + producto.
```
Use the provided character sheet as the exact identity reference for the woman. Preserve her facial features, proportions, skin tone, hairstyle, and overall appearance exactly.

Use the {escena} reference image for the exact scene, composition, camera angle, lighting, pose, outfit, layout, and overall framing.

Replace the placeholder product with the exact {PRODUCTO} container from the product reference. Keep the packaging identical, including the logo, typography, colors, proportions, lid, and label design. Do not redesign or modify the packaging in any way.

{qué hace la persona con el producto}

Authentic iPhone photography, vertical 9:16, ultra realistic, natural indoor lighting, subtle iPhone HDR, no cinematic grading.
```

---

## Pipeline de moda

Orden estricto: `avatar → cuerpo entero → pared blanca → outfit 1 → outfit 2 …`

**Cuerpo entero**
```
Using this image as reference, keep the SAME person (same face and identity), the same outfit and the same setting. Render a full-body shot from head to toe, the person standing naturally. Photorealistic, natural skin texture and lighting.
```

**Pared blanca (solo el fondo)**
```
Behind the woman there is a plain white wall, and the floor remains exactly the same as in the reference image. Do not change the flooring, its material, color, texture, or perspective. Only replace the background behind her with a clean white wall while keeping everything else identical.
```

**Vestir con un outfit de referencia** — dos imágenes: 1 = persona, 2 = ropa
```
Using the two reference images (image 1: the person; image 2: the outfit / clothing), keep the SAME person from image 1 — same face, hair, skin, body and identity — and dress her in the EXACT outfit shown in image 2, matching its garments, colors, patterns, textures and details as closely as possible. Change ONLY her clothing; keep her pose, framing, background and lighting exactly the same. The outfit fits her body realistically, with natural fabric folds and realistic lighting. The person is image 1, the clothes are image 2 — do NOT copy the face or body from image 2. Photorealistic. Single image.
```

**Producto en la mano** — dos referencias: persona + producto
```
Using the two reference images (the person and the {producto}), place the {producto} in the person's hand so they are holding it up and showing it to camera while talking about it, gesturing naturally, engaged expression. Keep the person's face and identity unchanged, keep the label exactly the same. Realistic hands, photorealistic, natural skin texture, visible pores. No text, no watermark, no distortion.
```

---

## Cambiar solo la ropa o solo el fondo

Retoque básico sobre una imagen ya buena. Nunca regenerar de cero.
```
Using this image as reference, keep the SAME person — same face, hair, body, pose, background and lighting. Change ONLY their clothing to [escribe el outfit aquí]. Keep everything else exactly the same. Photorealistic, natural fabric, realistic fit and lighting.
```
```
Replace the background behind the person with [describe el sitio: a cozy kitchen / a modern office / a neutral studio with soft lighting], keeping the person, their pose, lighting and framing exactly the same. Natural, realistic integration.
```
```
Flip the image horizontally
```

## Copiar algo de una segunda imagen

Regla común a todas: decir **cuál es la imagen 1 y cuál la 2**, y prohibir explícitamente traerse a la persona
de la 2. Sin esa frase el modelo mezcla las dos caras.

**Fondo desde una referencia**
```
Using the two reference images (image 1: the person; image 2: the background / setting), keep the SAME person from image 1 — same face, hair, skin, body, outfit and pose — and place them into the EXACT background shown in image 2, matching its location, colors, depth and atmosphere. Keep the person's pose, scale and framing exactly the same; replace ONLY what is behind them. Blend naturally: consistent lighting and shadows, matching color temperature and perspective, realistic edges with no cut-out look. The person is image 1, the background is image 2 — do NOT take any person or object from image 2. Photorealistic. Single image.
```

**Sustituir a la persona**
```
make this woman/man a different one, [DESCRIPCIÓN, OUTFIT...]
```
```
replace the guy from the file 1 with the guy from the file 2 wearing the same outfit as in file 2
```

**Producto real en la mano** — se adjunta su foto en vez de describirlo:
```
Using the two reference images (the person and the product), place the product in the person's hand so they are holding it up and showing it to the camera while talking about it.
```
```
Using the two reference images (the person and the product), show the person pointing at the product (held in the other hand or placed next to them) while looking at the camera. Keep the person's face and look unchanged, and keep the product's label and packaging exactly the same. Realistic hands and lighting.
```

## App o software en pantalla · dos pasos

**El orden no es negociable**: primero el dispositivo con la pantalla negra apagada, después la captura encima.
En un solo prompt el modelo se inventa la interfaz.

**Paso 1 · móvil**
```
Using the reference image, keep the SAME person — same face, hair, skin, body and identity — the SAME outfit, background and lighting.

Change ONLY this: she is now holding up a modern smartphone toward the camera, showing its screen to the viewer, the screen completely OFF and solid black (a blank black rectangle, no reflections, no UI, no icons, no text, no brand logos). She holds it naturally with one hand, the display side facing the camera, at chest height.

Keep both hands realistic and natural, correct number of fingers, natural grip on the phone. Photorealistic, natural skin texture and lighting. Single image.
```

**Paso 2 · móvil**
```
Using the two reference images (image 1: the person holding a smartphone with a black screen; image 2: an app screenshot), keep image 1 EXACTLY the same — same person, face, hair, hands, phone, pose, background and lighting, all unchanged.

Change ONLY this: place the screenshot from image 2 onto the phone's black screen, so it fills the display naturally. Fit it to the exact shape of the screen, matching the perspective and slight tilt of the phone, with realistic screen brightness, subtle glare and rounded screen corners. Do NOT crop or stretch the screenshot, keep its aspect ratio. The screenshot must look like it is really displayed on the phone.

Keep everything else identical to image 1. Photorealistic. Single image.
```

**Paso 1 · portátil**
```
Using the reference image, keep the SAME person — same face, hair, skin, body and identity — the SAME outfit, background and lighting.

Change ONLY this: she is now sitting with an open laptop, turning it and holding the screen toward the camera so the viewer sees the display. The laptop screen is completely OFF and solid black (a blank black rectangle, no reflections, no UI, no icons, no text, no brand logos). Natural, realistic pose tilting the laptop so the screen clearly faces the camera.

Keep both hands realistic and natural, correct number of fingers. Photorealistic, natural skin texture and lighting. Single image.
```

**Paso 2 · portátil**
```
Using the two reference images (image 1: the person holding a laptop with a black screen; image 2: an app or website screenshot), keep image 1 EXACTLY the same — same person, face, hair, hands, laptop, pose, background and lighting, all unchanged.

Change ONLY this: place the screenshot from image 2 onto the laptop's black screen, so it fills the display naturally. Fit it to the exact shape of the screen, matching the perspective and tilt of the laptop, with realistic screen brightness, subtle glare and correct proportions. Do NOT crop or stretch the screenshot, keep its aspect ratio. The screenshot must look like it is really displayed on the laptop.

Keep everything else identical to image 1. Photorealistic. Single image.
```

## Skincare · abrir un bote de tapa abatible

A la IA le cuesta abrir envases. Se adjunta el bote **más** una foto de un mecanismo equivalente, aclarando que
la segunda imagen es solo referencia del mecanismo.
```
Using the two reference images (image 1: the person holding the product bottle; image 2: an open flip-top cap, shown ONLY as a reference for the mechanism), keep the SAME person (same face, hair, skin and identity), the SAME bottle with its label, colors and text exactly unchanged, and the SAME room, background and lighting.

Change ONLY this: the bottle's flip-top cap is now flipped open on its hinge — the small lid tilted up and back and the nozzle opening exposed, exactly like the open flip mechanism in image 2. The hinged lid stays ATTACHED to the bottle; do NOT remove the cap. She raises her other hand beside the bottle, palm cupped and open, fingers relaxed, as if about to squeeze a little product into it.

Keep both hands realistic and natural, correct number of fingers. Photorealistic, natural skin texture and lighting. Single image.
```

## Bloques de realismo reutilizables

Estética iPhone (voz en off, trends):
```
Authentic iPhone photography, vertical 9:16, ultra realistic, natural lighting, subtle iPhone HDR, no cinematic grading.
```
```
Keep skin completely untreated with realistic pores, redness, acne, texture, natural shine, and imperfections. Preserve authentic smartphone realism without any beauty enhancement.
```
```
No text, no watermark, no distortion.
```

Anclar identidad al character sheet:
```
Use the provided character sheet as the exact identity reference for the woman. Preserve her facial features, proportions, skin tone, hairstyle, expression, and overall appearance exactly. She must wear the exact same {prenda} shown in the character sheet.
```

Plantilla general del formato voz en off:
```
Usando esta imagen de referencia, haz a la persona de la imagen sin cambiar absolutamente nada de ella, haciendo la siguiente acción: {acción}. {sitio} · {luz} · {plano}
```
