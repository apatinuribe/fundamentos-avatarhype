# Prácticas e insights — avatarhype

Lo que separa un vídeo que funciona de uno que huele a IA. Reglas, criterios de decisión y errores caros,
extraídos de las 28 lecciones. `proceso.md` dice *qué* hacer; este documento dice *por qué* y *cuándo*.

Las secciones hasta "Hueco conocido" son del **track realista**; el bloque final, del **track animado** (`[M6-*]`).

---

## Reglas duras (romperlas rompe el resultado)

| # | Regla | Por qué | Fuente |
|---|---|---|---|
| 1 | **Imagen primero, vídeo después. Nunca texto → vídeo** | Todo el control del realismo está en la imagen. Texto→vídeo no deja anclar cara, ropa ni escenario | [M1-L1.2] |
| 2 | **Un ángulo por vídeo** | Dos ángulos en el mismo anuncio diluyen los dos | [M3-L3.3.1] |
| 3 | **`NO TALKING` en todo clip sin guion** | Sin él el modelo hace hablar al avatar aunque no le des guion | [M4-L4.3] |
| 4 | **9:16 y calidad 2K en toda imagen de avatar** | Es el formato final; generar en otro obliga a recortar y pierde resolución | [M4-L4.1.1] |
| 5 | **Cámara estática siempre que haya manipulación de producto** | Si la cámara se mueve, la acción con el producto se rompe | [M4-L4.1.2] |
| 6 | **En Grok, 720 y nunca 480** | Cuesta exactamente lo mismo. Usar 480 es tirar calidad gratis | [M4-L4.1.3] |
| 7 | **La capa de realismo se aplica siempre, de punta a punta** | Sin ella la cara sale con "demasiada luz, demasiado flash" y canta a IA | [M4-L4.1.1] |
| 8 | **Bajar el volumen del clip duplicado** en superposiciones | Si no, el audio se oye doble | [M4-L4.1.1] |
| 9 | **Voz en off: todas las imágenes primero, animar después** | Mezclar los dos pasos rompe la continuidad de ropa y escenario | [M4-L4.3] |
| 10 | **En Meta, no lanzar oferta ni urgencia a tráfico frío** | Nivel 1-2 no sabe que tiene el problema; la oferta rebota | [M3-L3.3.2] |
| 11 | **Sustituir el marcador `marca`** en los prompts de imágenes estáticas | Si no, el modelo escribe literalmente "marca" en el diseño | [M4-L4.6] |
| 12 | **Activar el enlace de Google AI Pro el mismo día de la compra** | Caduca en pocos días | [M1-L1.3.2] |

---

## Criterios de decisión

### ¿Qué modelo de vídeo uso?

**Por clip, no por proyecto** [M4-L4.1.3]:

- **El avatar habla → Omni Flash.** Es el que sincroniza labios y voz.
- **El avatar no habla → Grok Imagine 1.5.** ~0,048 US$ por clip de 6 s a 720p, mucho más barato.

Un mismo anuncio de moda usa 3 clips Omni (los hablados) y 4 Grok (las poses) [M4-L4.1.3]. El de UGC con producto,
3 Omni y 1 Grok [M4-L4.1.2].

### ¿Necesito character sheet?

| Sí | No |
|---|---|
| El avatar aparece **de cuerpo entero** | Busto parlante, plano fijo |
| **Gira** o cambia de ángulo | Todos los clips desde el mismo encuadre |
| Muchos planos distintos (voz en off, moda) | Anuncio de 4 clips hablados |

Sin character sheet, el modelo **se inventa las facciones que no ve** [M4-L4.1.3].
*"Yo no lo suelo utilizar para vídeos normales"* [M4-L4.1.3].

### ¿Qué modo de quitamarcas?

El criterio es **el fondo detrás de la marca**, no la calidad del vídeo [M1-L1.4.2]:

- Fondo complejo (gente moviéndose, estampados) → **recomendada / avanzada**.
- Fondo estático que no cambia en todo el clip → **general**.

**Empezar siempre por la avanzada.** Reprocesar con el otro modo si no convence es flujo normal, no un plan B.

### ¿Cuánto dura el clip?

**Se mide el guion, no se elige por defecto** [M4-L4.1.1], [M4-L4.2], [M4-L4.4].
Guion corto → 6 s. Guion largo → 8 s. Flow ofrece 4/6/8/10 s [M1-L1.3.2].
**Mejor pasarse y recortar en edición** que quedarse corto y perder la última frase.

### ¿Flow, ApiMart o Kie?

- **Flow** — la vía barata: la imagen cuesta **0 créditos**, solo el vídeo consume [M1-L1.3.2]. Pero **el plan Pro
  saca marca de agua** [M4-L4.1.1].
- **ApiMart** — pago por uso, 10 créditos = 1 US$, mínimo 1 US$. **Sin marca de agua.** Permite lanzar varias
  generaciones **en paralelo** [M1-L1.3.3], [M4-L4.6].
- **Kie** — equivalente a ApiMart pero con mínimo de 5 US$ [M1-L1.3.4].

Comparar el mismo prompt en las tres y quedarse con la mejor salida es práctica normal [M4-L4.1.1].

---

## Realismo: por qué un vídeo canta a IA

**El realismo no se pide en el prompt, se diseña.** Tres capas, en orden de impacto [M3-L3.1], [M4-L4.1.1]:

**1. El avatar (fase de imagen).** Omni añade siempre una capa sutil de textura de piel al animar. Un avatar
perfecto + esa textura = resultado de IA evidente. Por eso se diseña **contra** la limitación: piel con
imperfecciones, cara no simétrica, nada de "guapísimo/a". Buscar el avatar **más humano y real** posible, no el más
atractivo [M3-L3.1].

**2. La micro-acción (fase de clip).** Tocarse las gafas, ajustarse la gorra, dar un trago de café. **Es lo que hace
humano al avatar** — un plano hablado sin micro-gesto se lee como IA aunque la cara sea perfecta [M1-L1.4.1].

**3. La capa de realismo (fase de edición).** Los 8 valores de CapCut. Convierte "grabado con flash" en "grabado con
un iPhone" [M4-L4.1.1].

Una cuarta, menor pero visible: **subir la velocidad 1.12–1.20**. La IA habla sistemáticamente demasiado lento; a
velocidad nativa el ritmo delata el origen [M4-L4.1.1], [M4-L4.2].

---

## Estrategia

- **El ángulo es ≈80 % del resultado.** Oferta y creatividad amplifican, pero no salvan un mal ángulo [M3-L3.3.1].
- **Del mismo producto salen 12 anuncios distintos sin tocar el producto**, solo cambiando ángulo × nivel de
  conciencia [M3-L3.3.1], [M3-L3.3.2].
- **Nivel 3 (consciente de la solución) pide señalar un culpable antes de explicar el mecanismo** — es la estructura
  que convierte en frío [M3-L3.3.2].
- **Nivel 4 = un vídeo por objeción.** No meter todas las objeciones en un anuncio [M3-L3.3.2].
- **El rótulo fijo de retención no es decoración**: quien llega scrolleando lee de qué va el vídeo y es más probable
  que se quede [M4-L4.1.2].
- **El hook es el clip 0.** La numeración del agente empieza en 0 justamente porque el hook es una pieza aparte, no
  el principio del primer clip [M3-L3.3.3].

---

## Trabajar con los agentes

- **Describir el producto en una frase vaga es suficiente.** El instructor insiste: no hace falta un briefing
  [M3-L3.3.3], [M4-L4.6].
- **Delegar la elección**: cuando El Estratega propone ángulos y pregunta cuáles desarrollar, responder
  **"elige los tres mejores"** [M3-L3.3.3].
- **Pedir el formato explícitamente** si buscas uno concreto: *"quiero hacer un día conmigo"* [M4-L4.3].
- **Iterar sobre el prompt, no sobre la imagen.** Con el agente 6C se ajusta el texto (que sea rubia, otra ropa)
  antes de gastar una generación [M3-L3.2].
- **Los agentes preguntan lo que les falta.** El de imágenes estáticas pide precio, mercado y paleta; **si no dices
  mercado, asume España** [M4-L4.6].
- **Verificar siempre ingredientes y beneficios** que el agente escribe: los inventa plausibles. El propio agente
  avisa de que los ajustes [M3-L3.3.3].
- **Copiar la imagen y pegarla en el chat** en vez de descargarla evita llenar el disco de capturas [M4-L4.2].

---

## Escribir prompts de clip

- **La micro-acción va dentro del guion, entre corchetes y en inglés**, en el punto exacto de la frase donde debe
  ocurrir. No en un párrafo aparte [M4-L4.1.1].
- **`While speaking, …`** fuerza que la acción ocurra *durante* el habla; sin ella el modelo las separa en el tiempo
  [M4-L4.1.2].
- **Se puede acotar en el tiempo**: `while saying in the first 3 seconds of the video` [M4-L4.1.4].
- **Coreografiar el gesto con la superposición.** Si el avatar señala arriba a la derecha al decir "hace 3 meses", es
  porque ahí va la imagen del antes: el gesto **reserva el hueco** en pantalla [M4-L4.1.1], [M4-L4.1.3], [M4-L4.4].
- **`Photorealistic, realistic hands`** siempre que manipule objetos: las manos son donde falla el modelo
  [M4-L4.1.2].
- **Acento**: el latino neutro sale solo, no hace falta pedirlo. **El español de España hay que pedirlo
  explícitamente** [M4-L4.1.1].
- **Prompts en inglés; guion y descripción pueden ir en español** [M1-L1.4.1], [M3-L3.2].
- La voz no se controla con precisión — solo género y franja de edad, y depende del modelo [M1-L1.4.1].

---

## Encadenar imágenes

- **Una imagen por estado**, no una imagen animada varias veces [M4-L4.1.2], [M4-L4.2].
- Cada prompt **edita el resultado anterior** y pide que parezca `the next frame of the same video`: eso mantiene la
  continuidad mejor que describir la escena de nuevo [M4-L4.1.2].
- **Listar explícitamente lo que NO cambia** (cara, ropa, escenario, luz, ángulo, encuadre, composición, packaging).
  `Keep everything exactly the same` a secas es demasiado débil [M4-L4.1.2].
- **Blindar el packaging de marca**: `without changing the branding, colors, typography, or label`. Sin eso el
  modelo reescribe la etiqueta [M4-L4.1.2].
- **Reciclar el encuadre** (`Edit the reference image… Replace X with Y`) ahorra generaciones y mantiene coherencia
  [M4-L4.3].
- **Generar de más y descartar** es normal: en BLUME se generaron 5 imágenes y se usaron 4 [M4-L4.1.2].
- Imágenes que se van a superponer en edición: **1:1**, no vertical [M4-L4.1.1].
- El **orden del pipeline de moda importa**: `avatar → cuerpo entero → pared blanca → outfit 1 → outfit 2`. Saltarse
  la pared blanca hace que los outfits hereden el fondo original [M4-L4.1.3].

---

## Edición

- **Cortar los espacios muertos** del final de cada clip, donde el avatar termina y se queda callado. Con los
  recortes: **la mitad coloreada es la que se conserva** [M4-L4.1.1].
- **La velocidad se ajusta clip a clip y de oído**, no la misma para todos. Rango 1.12–1.20, "1.20 como máximo"
  [M4-L4.1.1].
- **Transiciones: pocas y discretas.** La única que usa el instructor es **Mix**. Las llamativas están descartadas por
  diseño — el objetivo es que parezca grabado, no editado [M4-L4.1.1].
- **La capa de realismo se guarda como preset una sola vez** (`Save as preset` → Ajustes → Yours/Tuyos → clic
  derecho → renombrar) y se arrastra a todos los proyectos siguientes [M4-L4.1.1].
- **Superponer detrás del avatar necesita dos cosas juntas**: quitar el fondo del clip duplicado (Pro) **y** bajarle
  el volumen [M4-L4.1.1].
- **El zoom falso con fotogramas clave** sustituye a generar un clip con zoom: rombo en *Escalar*, 100 % al principio
  → 150 % al final. Funciona con cualquier propiedad del panel [M4-L4.3].
- **En voz en off manda el audio**: los clips de 6 s se recortan a 2–3 s y los cortes se cuadran con la narración
  [M4-L4.3].
- **En podcast los clips se apilan solapándose**, para que la cámara corte a la otra persona antes de que la primera
  termine de hablar. Es lo que da el ritmo de podcast real [M4-L4.2].
- **En trend viral la música del TikTok sostiene el anuncio** y el texto del trend se traduce al español encima
  [M4-L4.5].

---

## Costes y economía

- Flow: **la imagen no cuesta créditos**, solo el vídeo [M1-L1.3.2].
- Grok 1.5: **~0,048 US$** por clip de 6 s a 720p [M4-L4.1.3]. De ahí que la regla habla→Omni / no habla→Grok sea la
  decisión más rentable del método.
- ApiMart: 10 créditos = 1 US$, **recarga mínima 1 US$** (perfil → Facturación) [M1-L1.3.3].
- Kie: **recarga mínima 5 US$** [M1-L1.3.4].
- CapCut: **el plan gratuito basta** para todo salvo quitar el fondo [M1-L1.3.5].
- ElevenLabs: **10.000 créditos gratis al mes** [M4-L4.3].
- Biblioteca de audio del curso: **392 pistas sin copyright** [M1-L1.4.3].
- Atajo de Flow: 12 US$ pago único → 18 meses de Google AI Pro [M1-L1.3.2].

---

## Errores que salen caros

1. **Generar el avatar de cero, sin foto de referencia real.** El resultado es el rostro promedio del modelo
   [M3-L3.2], [M4-L4.1.1].
2. **Elegir un avatar guapo y perfecto.** Se lleva mal con la textura que añade Omni [M3-L3.1].
3. **Olvidar `NO TALKING`** en un clip de producto o de pose: el avatar habla sin guion [M4-L4.3].
4. **Mover la cámara en un clip con producto en las manos** [M4-L4.1.2].
5. **Olvidar bajar el volumen** del clip duplicado en la superposición: audio doble [M4-L4.1.1].
6. **Saltarse la capa de realismo.** Es el paso individual con más impacto de toda la edición [M4-L4.1.1].
7. **Dejar la velocidad a 1.0.** El ritmo lento es una firma de IA [M4-L4.1.1].
8. **En dualcast, describir solo al que habla.** El modelo hace hablar a los dos o congela al segundo: hace falta el
   **doble bloque de micro-acción** [M4-L4.4].
9. **Usar 480 en Grok** cuando 720 cuesta lo mismo [M4-L4.1.3].
10. **Lanzar oferta a tráfico frío en Meta** [M3-L3.3.2].
11. **No sustituir el marcador `marca`** en los prompts de imágenes estáticas [M4-L4.6].
12. **Dejar caducar el enlace de activación de Google AI Pro** [M1-L1.3.2].

---

## Hueco conocido

`4.7-ugly-ads` está listada en el curso pero **no tiene contenido publicado**: la nota es un marcador. Nada de este
documento cubre ese formato [M4-L4.7].

---

## Track Animados · reglas y criterios [M6-*]

Todo lo anterior es el track realista. Este bloque cubre el **track animado** (curso *Creativos Animados*).
Comparte la filosofía, no la ejecución.

### Reglas duras del track animado

| # | Regla | Por qué | Fuente |
|---|---|---|---|
| A1 | **Los 8 prompts van en una sola conversación de ChatGPT, en orden** | Cada uno da por hecho lo que cerró el anterior; al llegar al 7 el contexto ya está dentro y se audita sin reexplicar | [M6-L6.2] |
| A2 | **El Prompt 2 se pega en NotebookLM, no en ChatGPT** | Es el único que cambia de herramienta. Pegarlo en GPT devuelve insights inventados en vez de datos de las fuentes | [M6-L6.2] |
| A3 | **En el Prompt 6, Style Lock con un solo estilo** | Si quedan varios, los prompts de imagen salen mezclados y el anuncio pierde coherencia visual | [M6-L6.2] |
| A4 | **El estilo se elige en el Prompt 1, no al final** | Es dato de entrada del método entero; cambiarlo a mitad invalida guion, storyboard y prompts | [M6-L6.1] |
| A5 | **Las 3 búsquedas se importan en NotebookLM una a una** | Discover Sources no acepta prompts largos: son búsquedas cortas tipo Google, y hay que esperar a que cada una termine | [M6-L6.2] |
| A6 | **9:16 y 2K siempre en Nano Banana Pro** | 1K y 2K cuestan lo mismo; generar en 1K es tirar calidad gratis | [M6-L6.2] |
| A7 | **Nombrar las imágenes P1, P2, P3… por número de prompt** | Es lo único que mantiene el orden primer/último frame al montar los pares | [M6-L6.2] |
| A8 | **En Kling, modo «Future» (primer + último frame), no «base»** | El método no genera planos: genera la transición entre dos imágenes ya fijadas | [M6-L6.2] |
| A9 | **`sound effects (no talking)` en todo prompt de estilo** | Equivalente animado del `NO TALKING` del track realista: sin él el modelo mete voces | [M6-L6.2] |
| A10 | **No quedarse con la primera respuesta de GPT** | *"La IA lo que te va a dar a la primera, ni a la segunda, ni a veces a la tercera, es lo mejor"* | [M6-L6.2] |

### Criterios de decisión del track animado

**¿Qué estilo elijo?** Cinco disponibles: Realista (Apple keynote), Sci-fi, Pixar, Claymation y Wes Anderson. Se
decide en el Prompt 1 junto al producto y el mercado, y condiciona storyboard y prompts de imagen [M6-L6.1].

**¿ApiMart o KIE para las imágenes?** Nano Banana Pro cuesta **0,05 US$/imagen en ApiMart** y **0,09 US$ en KIE**.
Casi la mitad en ApiMart. Como referencia de lo que evita el método: HeyGen, Freepik, Arcads, Wavy y Higgsfield
parten de **0,15 US$/imagen** [M6-L6.2].

**¿Qué modelo de voz en ElevenLabs?** No es intercambiable: **voz del catálogo → Eleven Multilingual V2**; **voz
clonada propia → V3** [M6-L6.2].

**¿Cuántos clips necesito?** Uno por cada par de imágenes consecutivas: **número de imágenes − 1**. Duración 3, 4 o
5 s cada uno (el curso usa 4) [M6-L6.2].

### Qué comparten los dos tracks

| Comparten | Difieren |
|---|---|
| El resultado se decide en la planificación (~80 %) [M3-L3.3.1], [M6-L6.2] | Realista: ángulo + niveles de conciencia · Animado: cadena de 8 prompts + NotebookLM |
| 9:16 en 2K [M4-L4.1.1], [M6-L6.2] | Realista: imagen→vídeo con avatar hablando · Animado: transición entre dos imágenes |
| ApiMart / KIE como acceso barato a los modelos | Realista: Omni y Grok · Animado: Nano Banana Pro y Kling 3 |
| ElevenLabs, 10.000 créditos gratis/mes | Realista: voz en off solo cuando el avatar no habla · Animado: siempre voz en off |
| Montaje en CapCut gratuito, transición **Mix** | Realista: velocidad 1,12-1,20 + capa de realismo de 8 valores · Animado: velocidad 1,20 y **sin capa de realismo** |
| Prohibición de que el modelo hable por su cuenta | Realista: `NO TALKING` · Animado: `sound effects (no talking)` |

### Errores caros del track animado

1. **Pegar el Prompt 2 en ChatGPT.** Se pierden los datos duros, que son lo que sostiene el guion.
2. **Dejar todos los estilos en el Style Lock** del Prompt 6.
3. **Generar imágenes sin nombrarlas por prompt**: al montar los pares en Kling se pierde el orden.
4. **Dejar Kling en «base»** y subir una sola imagen: sale un plano animado, no la transición.
5. **Quedarse con el primer storyboard**, que es donde el método dice que hay que iterar más.
6. **Generar en 1K** pudiendo generar en 2K al mismo precio.
7. **Aplicar la capa de realismo del track realista** a un anuncio animado: sobra por definición.

### Advertencia de vigencia

El curso **se está regrabando entero** — literal: *"ahora mismo estamos regrabando desde cero todo el apartado de
Ads Animados"*, con las actualizaciones incluidas de por vida [M6-L6.1]. Lo recogido aquí es una foto a
**2026-09-03**. Los nombres de los controles de las interfaces (en particular el selector «Future» de Kling en
ApiMart) son los que se ven en el vídeo y pueden haber cambiado.

---

## Anexo · dirección entre guion e imagen [ANEXO · no es del curso]

> **Nada de esta sección lleva cita `[M…]` porque no sale del curso.** Es la capa de dirección de la
> `Fase 2.5` de `proceso.md`. Si contradice algo citado, manda lo citado.

### Por qué no se importa un director audiovisual al uso

Un agente genérico de dirección trae oficio de rodaje real. Con estos modelos, la mitad de ese oficio **empeora**
el resultado, porque asume un plató, un operador de cámara y un montaje que aquí no existen.

| Lo que trae un director al uso | Por qué no entra aquí |
|---|---|
| Dirección en prosa cinematográfica | La fórmula del clip es por ranuras y seca: `CÁMARA + MOVIMIENTO + MICRO-ACCIÓN + GUION + VOZ + ACENTO` [M1-L1.4.1]. El párrafo literario diluye las ranuras |
| Listas de *negative prompt* / bloques "EVITAR" | El método no usa negativos: usa **positivos incrustados** — `NO TALKING`, `No talking, mouth closed`, `Photorealistic, realistic hands` [M4-L4.1.1] |
| Cambios de plano dentro de un clip | Un clip es **una** generación desde **una** imagen. Cambiar de plano es otro clip y otra imagen [M3-L3.2] |
| Movimiento de cámara por espectáculo | Con producto en mano la cámara va **estática, sin excepción** [M4-L4.1.1] |
| Dirigir tono, ritmo y pausas de cualquier voz | Solo se dirige la voz cuando la pone ElevenLabs [M4-L4.3]. La de Omni sale de las ranuras `VOZ` y `ACENTO` y no se controla |
| Reescribir el guion para que "suene mejor" | El guion es lo importante del clip; lo negociable es la parte visual [M3-L3.3.3] |
| Diseñar escenografía, fotografía y composición aparte | Ya son cuatro de los seis bloques del 6C: `Context`, `Cinematic Light`, `Camera`, `Clothing` [M3-L3.2]. Duplicarlo genera dos fuentes de verdad que se contradicen |

### Lo que sí aporta la fase, y no estaba

- **Una biblia de continuidad escrita antes del primer clip.** Las anclas de consistencia se piden clip a clip
  [M3-L3.2]; nada dice de dónde salen. Escritas una vez y reutilizadas literalmente, el avatar no deriva.
- **Decidir la ruta de voz antes de escribir nada.** Omni o ElevenLabs cambia qué se puede dirigir.
- **Una función declarada por clip**, contrastada contra la estructura hook → problema → agitación → mecanismo →
  demostración → beneficio → CTA [M3-L3.3.3]. Es verificación, no generación: la estructura ya la da El Estratega.
- **Anotar los gestos que reservan hueco** para una superposición, para que el montaje sepa dónde va [M4-L4.1.1].

### Regla de arbitraje

Si la ficha de dirección y un documento citado dicen cosas distintas, se hace lo citado y **se corrige la ficha**.
La plantilla es un ayudante de decisión, no una fuente.
