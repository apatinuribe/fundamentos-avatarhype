# Proceso — avatarhype

El método completo, de la idea al archivo montado, en el orden en que se ejecuta.
Reordenado por tarea a partir de las 28 lecciones; cada afirmación cita su lección de origen.

**Dos tracks.** Las fases 0-7 son el **track realista** (UGC con avatar humano, curso *Avatar Hype Academy*).
A partir de "Track Animados" está el **track animado** (curso *Creativos Animados*, `[M6-*]`): otro método, otra
cadena de herramientas, otro resultado. Se elige uno de los dos al empezar el proyecto, no se mezclan.

Regla que gobierna todo el pipeline: **primero se genera la imagen, después se anima esa imagen** [M1-L1.2].
El curso nunca genera vídeo desde texto. Todo el peso del realismo cae en la fase de imagen.

---

## Fase 0 · Stack

Dos herramientas bastan para el método entero: una de generación y una de edición [M1-L1.3.5].

| Función | Herramienta | Notas |
|---|---|---|
| Generación (imagen + vídeo) | **Google Flow** | Vía barata. La imagen cuesta **0 créditos**; solo el vídeo consume [M1-L1.3.2] |
| Generación (pago por uso) | **ApiMart** | 10 créditos = 1 US$, recarga mínima 1 US$. Ruta: perfil → Facturación [M1-L1.3.3]. Aquí viven VEO 3.1, Omni Flash y Grok |
| Generación (alternativa) | **Kie** | Equivalente a ApiMart. Recarga mínima **5 US$** [M1-L1.3.4] |
| Edición | **CapCut escritorio, plan gratuito** | Solo una función del curso exige Pro: quitar el fondo [M1-L1.3.5], [M4-L4.1.1] |
| Voz en off | **ElevenLabs** | 10.000 créditos gratis/mes [M4-L4.3] |
| Audio | Biblioteca AvatarHype (392 pistas sin copyright) o Epidemic Sound [M1-L1.4.3] |

**Modelos por defecto:** imagen realista → **Nano Banana Pro** (en Flow) o **GPT Image 2** [M1-L1.3.2], [M4-L4.1.1].
Vídeo → **Omni Flash** [M1-L1.3.2].

**Regla de reparto de modelo de vídeo, la más rentable del curso:**
**el avatar habla → Omni · el avatar no habla → Grok** [M4-L4.1.1], [M4-L4.7].
No es una decisión por proyecto, es **por clip**: un mismo vídeo puede usar los dos [M4-L4.1.3].
Grok Imagine 1.5 cuesta ~**0,048 US$** por clip de 6 s a 720p [M4-L4.1.3].

**Acceso barato a Flow** (opcional, es un atajo, no una dependencia): pack de plantillas en contentplanner.store,
12 US$ pago único → enlace de activación → 18 meses de Google AI Pro. **Activar el enlace el mismo día**: caduca en
pocos días [M1-L1.3.2].

---

## Fase 1 · Estrategia

Se decide **antes** de generar nada. El anuncio es un sistema de tres palancas, en este orden de importancia [M3-L3.3.1]:

1. **Ángulo** — a quién le hablas y desde qué dolor entras. **≈80 % del resultado.**
2. **Oferta** — qué le das y cómo lo empaquetas.
3. **Creatividad** — hook, edición, música. Amplifica, pero no salva un anuncio con mal ángulo.

**Un ángulo por vídeo** [M3-L3.3.1]. Del mismo producto salen 12 anuncios distintos sin tocar el producto
(matriz completa en `ejemplos.md`).

Cruzar el ángulo con el **nivel de conciencia** del que va a ver el anuncio [M3-L3.3.2]:

| Nivel | Estado del espectador | Qué toca hacer |
|---|---|---|
| 1 · Inconsciente | No sabe que tiene el problema | Abrirle los ojos con una historia. **No vender** |
| 2 · Consciente del problema | Siente el dolor, no sabe que hay solución | Remover el problema y enseñar que hay salida |
| 3 · Consciente de la solución | Conoce soluciones, no la tuya | **Explicar el mecanismo**: señalar un culpable primero |
| 4 · Consciente del producto | Te conoce, tiene objeciones | Prueba social y comparativas, **un vídeo por objeción** |
| 5 · Súper consciente | Quiere comprar | Aquí sí: oferta, urgencia, garantía |

**En Meta el tráfico es frío: priorizar niveles 1, 2 y 3.** Lanzar oferta y urgencia a nivel 1 es el error más
caro y más común [M3-L3.3.2].

---

## Fase 2 · Guion (agente El Estratega)

1. Abrir El Estratega (GPT o skill de Claude) [M3-L3.3.3].
2. **Describir el producto en una frase vaga.** No hace falta más — el instructor insiste en ello [M3-L3.3.3].
3. El agente pide el **avatar**; otra frase vaga basta ("mujeres de más de 35 años").
4. **Fase 2 del agente** — devuelve: voz del cliente (dolores), deseos, objeciones, menú de ángulos, ideas de hook,
   mecanismo propuesto y nivel de conciencia recomendado por plataforma.
5. Propone tres ángulos y pregunta cuáles desarrollar → responder **"elige los tres mejores"** y dejarle decidir
   [M3-L3.3.3]. Si buscas un formato concreto, pídeselo en su lugar: *"quiero hacer un día conmigo"* [M4-L4.3].
6. **Fase 3** — tres anuncios desglosados **clip a clip**. Cada clip trae tres campos:
   **rótulo en pantalla** (texto sobreimpreso) · **visual** (qué se ve) · **guion** (qué se dice).
7. Ajustar ingredientes y beneficios a los reales del producto — el agente avisa de que lo hagas [M3-L3.3.3].

Estructura de anuncio que produce siempre: **clip 0 (hook) → problema → agitación → mecanismo → demostración →
beneficio → CTA** [M3-L3.3.3]. La numeración empieza en 0: el "clip cero" es el hook.

**El guion es lo importante de cada clip; la parte visual es negociable** [M3-L3.3.3].
De ahí sale el reparto: la parte visual alimenta el prompt de imagen, el guion alimenta el prompt de vídeo.

---

## Fase 3 · Imagen

### 3.1 · La referencia

Nunca se imagina el avatar de cero: se parte de **una foto de una persona real** de Pinterest, TikTok o Instagram
[M3-L3.2], [M4-L4.1.1].

- Captura de pantalla del reel o del pin (en Mac, **Cmd + Shift + 4**) [M4-L4.1.1].
- Alternativa que evita llenar el disco: **clic derecho → copiar imagen** y pegarla directamente en el chat del
  agente, sin descargarla [M4-L4.2].
- Consulta de inspiración que da el curso: **"podcast setup"** en Pinterest para el formato podcast [M4-L4.2].

### 3.2 · Referencia → prompt

**Vía A · Agente 6C.** Adjuntar la imagen; el agente pregunta *"¿igual o con cambios?"*, responde con el prompt
estructurado en inglés y en un único bloque de código [M3-L3.2]. Iterar sobre el prompt (que sea rubia, otra ropa)
antes de generar.

Las seis C: **Character · Camera · Clothing · Context · Cinematic Light · Consistency Anchors** [M3-L3.2].

**Vía B · Sin agente.** Ir a la biblioteca → "cambiar el avatar en base a una descripción", adjuntar la referencia
en GPT Image 2 y rellenar la descripción [M3-L3.2]. Más rápido cuando ya sabes qué quieres.

**Instalación de las skills en Claude:** `+ → Skills → Manage skills → Añadir → Subir skill`, subiendo el `.md`
descargado. Para usarla: `+ → Skills → seleccionarla` en cada conversación [M3-L3.2], [M4-L4.6].

### 3.3 · Generar el avatar

- Modelo: **GPT Image 2** o **Nano Banana Pro**. Con imagen de referencia, en Kie hay que elegir la entrada
  **imagen a imagen**, no texto a imagen [M4-L4.1.1].
- **Aspect ratio 9:16. Calidad siempre 2K** [M4-L4.1.1].
- Comparar el mismo prompt entre Flow, ApiMart y Kie y quedarse con el mejor [M4-L4.1.1].

**Diseñar el avatar contra la limitación del modelo** [M3-L3.1]: Omni añade siempre una capa sutil de textura en la
piel al animar. Evitar piel impoluta, cara simétrica, cero defectos, guapísimo/a. Buscar el avatar **más humano,
imperfecto y real** posible. Avatar perfecto + capa de textura = "canta" a IA.

### 3.4 · Character sheet — solo cuando hace falta

Se genera con el prompt de la **parte A de la biblioteca**, en GPT Image 2, tamaño 9:16 [M4-L4.1.3].

**Obligatorio** cuando el avatar aparece de cuerpo entero, lejos o girando, y en formatos con muchos planos y
ángulos distintos [M4-L4.1.3], [M4-L4.3]: sin él el modelo **se inventa las facciones que no ve**.
**Innecesario** para busto parlante: *"yo no lo suelo utilizar para vídeos normales"* [M4-L4.1.3].

### 3.5 · Imágenes de estado y de apoyo

**Una imagen por estado**, no una imagen animada varias veces [M4-L4.1.2], [M4-L4.2].
Cada prompt **edita la imagen anterior** y pide que el resultado parezca *"the next frame of the same video"*.

Patrón que mantiene la continuidad [M4-L4.1.2]:
`Keep everything exactly the same` + lista explícita de lo que NO cambia (cara, ropa, escenario, luz, ángulo,
encuadre, composición, packaging) + el cambio concreto.

Para producto de marca, bloquear el packaging: `without changing the branding, colors, typography, or label`
[M4-L4.1.2]. Sin eso el modelo reescribe la etiqueta.

**Reciclar el encuadre** en vez de generar escenas nuevas (`Edit the reference image… Replace X with Y`) ahorra
generaciones y mantiene la coherencia [M4-L4.3].

Pipeline encadenado de moda, en este orden exacto [M4-L4.1.3]:
`avatar → cuerpo entero → pared blanca → outfit 1 → outfit 2 → …`, cada outfit sobre el resultado anterior.

Imágenes que se van a **superponer** en edición: generarlas en **1:1**, no en vertical [M4-L4.1.1].

**Genera de más y descarta**: en el caso BLUME se generaron 5 imágenes y se usaron 4 [M4-L4.1.2].

---

## Fase 4 · Clips

### 4.1 · La estructura del prompt

Todo clip hablado se monta con las piezas de la **parte B de la biblioteca** [M1-L1.4.1], [M4-L4.1.1]:

```
CÁMARA + MOVIMIENTO + MICRO-ACCIÓN + GUION + VOZ + ACENTO
```

- **Cámara**: estática, zoom lento a la cara, zoom rápido al hablar, retroceso que revela el ambiente, órbita lenta,
  seguimiento al caminar, push-in a los ojos [M1-L1.4.1].
- **Micro-acción**: tocarse las gafas, ajustarse la gorra, dar un trago de café. **Es lo que hace humano al avatar**
  — sin micro-gesto, se lee como IA [M1-L1.4.1].
- **Voz**: hombre/mujer × joven / mediana edad / mayor. No se controla con precisión, depende del modelo [M1-L1.4.1].
- **Acento**: España, latino neutro, Colombia, Argentina, México. Para **latino neutro no hace falta pedirlo** (la IA
  tiende a él por defecto); para **español de España sí hay que pedirlo explícitamente** [M4-L4.1.1].

Los prompts van **en inglés**; el guion y la descripción pueden ir en español [M1-L1.4.1], [M3-L3.2].

### 4.2 · Reglas de escritura del prompt de clip

- **Las micro-acciones van incrustadas dentro del guion**, entre corchetes y en inglés, en el punto exacto de la
  frase: `[Points up to the right]` [M4-L4.1.1].
- **`While speaking, …`** hace que la acción ocurra *durante* el habla. Sin ella el modelo las separa [M4-L4.1.2].
- **Se puede acotar en el tiempo**: `while saying in the first 3 seconds of the video` [M4-L4.1.4].
- **Cámara estática obligatoria cuando hay manipulación de producto.** Si la cámara se mueve, la acción se rompe
  [M4-L4.1.2].
- **`NO TALKING` en todo clip sin guion.** Sin él *"el modelo tiende a hacer a la persona hablando aunque no le des
  ningún guion"* [M4-L4.3]. También `No talking, mouth closed` [M4-L4.1.2].
- **Coreografiar la micro-acción con la superposición**: si el avatar señala arriba a la derecha al decir "hace 3
  meses", es porque **ahí** va la imagen del antes. El gesto reserva el hueco [M4-L4.1.1], [M4-L4.1.3], [M4-L4.4].
- `Photorealistic, realistic hands` cuando manipula objetos: es donde falla el modelo [M4-L4.1.2].

### 4.3 · Generación

- Configuración: **9:16**, modelo según hable o no, duración según guion.
- **La duración se elige midiendo el guion**, no por defecto [M4-L4.1.1], [M4-L4.2], [M4-L4.4].
  Flow ofrece 4 / 6 / 8 / 10 s [M1-L1.3.2]. Guion corto → 6 s; guion largo → 8 s. Mejor pasarse y recortar en edición.
- Cargar la imagen que corresponde a **ese** clip → **Añadir al prompt** → generar.
- En clips hablados sin cambio de postura se reutiliza **siempre la misma imagen** [M4-L4.1.3].
- **En Grok: resolución 720, nunca 480 — cuesta exactamente lo mismo** [M4-L4.1.3]. Duración mínima 6 s.
- En ApiMart se pueden lanzar **varias generaciones en paralelo** sin esperar [M4-L4.6].

### 4.4 · Voz en off (solo cuando el avatar no habla)

ElevenLabs → *Voces* (filtrar idioma, categoría, género, edad) → *texto a audio* → pegar el guion → Generar →
Descargar [M4-L4.3].

---

## Fase 5 · Limpieza

**Los clips de Flow con plan Pro salen con marca de agua; los de ApiMart, no** [M4-L4.1.1].

Herramienta del curso (`/academy/tools/quitar-marca`), dos modos [M1-L1.4.2]:

- **Recomendada / avanzada** — empezar **siempre** por esta. Para fondo complejo: gente moviéndose, estampados.
- **General** — para marca sobre **fondo estático** que no cambia en todo el clip.

El criterio es **el fondo detrás de la marca**, no la calidad del vídeo. Flujo: arrastrar el vídeo →
**esperar a que localice la marca automáticamente** antes de pulsar nada → ajustar el recuadro a mano si falla →
Quitar marca → comparar → **si no convence, reprocesar con el otro modo** (es parte del flujo normal, no un plan B).
Se ejecuta en el navegador, no sube el archivo, y mantiene el audio.

---

## Fase 6 · Edición en CapCut

El montaje de **[M4-L4.1.1] es la edición de referencia de todo el curso**; el resto de formatos la dan por sabida.

### 6.1 · Montaje base

1. **Media → Importar** todos los clips y todas las imágenes de superposición.
2. Arrastrar los clips a la timeline en orden.
3. **Cortar los espacios muertos** del final de cada clip, donde el avatar acaba y se queda callado. Con los dos
   botones de recorte: **la mitad que queda coloreada es la que se conserva**.
4. **Subir la velocidad clip a clip, de oído.** La IA habla demasiado lento — es sistemático, no puntual [M4-L4.2].
   Rango **1.12–1.20**, "1.20 como máximo". Cada clip pide la suya; no aplicar la misma a todos.
5. **Capa de realismo** como capa de ajuste que recorre el vídeo entero (pista `Adjust1` de punta a punta).
6. Música y efectos de sonido.

### 6.2 · La capa de realismo

Es el centro de la edición: sin ella la cara sale con "demasiada luz, demasiado flash"; con ella parece grabado con
un iPhone. Es lo que separa el resultado de un vídeo con pinta de IA [M4-L4.1.1].

CapCut → pestaña **Ajuste / Adjust** → *Basic*, valores exactos leídos del vídeo de edición:

| temp | tint | saturation | exposure | contrast | highlight | shadow | fade |
|---|---|---|---|---|---|---|---|
| -3 | 2 | -6 | -3 | 12 | -35 | 18 | 6 |

**Se configura una sola vez**: seleccionar un clip → Ajuste → meter los valores → **Save as preset** → queda en
Ajustes → **Yours / Tuyos** → clic derecho → renombrar. A partir de ahí se arrastra a cualquier proyecto.

### 6.3 · Recursos de montaje

- **Transiciones: pocas y discretas.** La única que usa el instructor es **Mix**. Las llamativas están descartadas
  por diseño: el objetivo es que parezca grabado, no editado [M4-L4.1.1].
- **Imágenes superpuestas detrás del avatar** — hacen falta **dos cosas juntas**: duplicar el clip original,
  colocarlo encima de las imágenes, **quitarle el fondo** (función Pro) **y bajarle el volumen**. Si se olvida el
  volumen, el audio se oye doble [M4-L4.1.1].
- **Animación de entrada** de las imágenes: **Zoom**, **Shake**, **Slide Up** [M4-L4.1.1].
- **Rótulo fijo de retención** — una frase corta en pantalla durante todo el vídeo que diga de qué va. Quien llega
  scrolleando la lee y es más probable que se quede. No es decorativo [M4-L4.1.2].
- **Zoom falso con fotogramas clave** — cada propiedad del panel tiene un **icono de rombo** que la fija en la
  posición del cursor. Cursor al principio → rombo en *Escalar* a **100 %**; cursor al final → **150 %**. Funciona
  igual con cualquier otra propiedad [M4-L4.3].

---

## Fase 7 · Variantes de montaje por formato

Todo lo anterior es común. Lo que distingue a cada formato es esto:

| Formato | Producción | Lo que cambia en el montaje |
|---|---|---|
| **UGC sin producto** [M4-L4.1.1] | 1 imagen avatar + imágenes antes/después (1:1) · 4 clips Omni | El montaje de referencia completo: transiciones Mix, superposiciones detrás del avatar, animaciones de entrada |
| **UGC con producto** [M4-L4.1.2] | 1 imagen por estado del producto · 3 clips Omni + 1 Grok | El más simple: clips, capa de realismo, **rótulo fijo**, música. **Sin transiciones ni superposiciones** |
| **Moda** [M4-L4.1.3] | Avatar + character sheet + 1 imagen por outfit · 3 clips Omni + 4 Grok | **Inversión de planos**: los clips de pose ocupan el fotograma; el clip hablado va **recortado y pequeño abajo a la derecha** |
| **App / SaaS** [M4-L4.1.4] | **1 sola imagen** · 3 clips Omni + screen recording | Orden estricto: avatar solo → logo → **app a pantalla completa con el avatar abajo a la derecha** |
| **Podcast** [M4-L4.2] | 2 avatares en encuadres distintos · 1 clip por intervención | **Apilar cada clip encima del anterior, solapándolos**, para que la cámara corte a la otra persona antes de que la primera termine. Sin transiciones |
| **Dualcast** [M4-L4.4] | **1 sola imagen** con las dos personas · 4 clips Omni | Montaje normal + superponer imágenes de lo que se menciona. La edición va dentro del propio vídeo de la lección |
| **Voz en off** [M4-L4.3] | Character sheet + muchas imágenes · clips Grok + narración ElevenLabs | **Recortar cada clip de 6 s a 2–3 s** y cuadrar los cortes con el audio. **El audio manda.** Sin transiciones |
| **Trend viral** [M4-L4.5] | Igual que voz en off | El **TikTok descargado va en la pista principal**, cortado por sus propios cambios de plano; **su música sostiene el anuncio**; texto del trend **traducido al español** encima; el producto entra al final |
| **Imágenes estáticas** [M4-L4.6] | Agente Ads Visual Architect → 7 prompts → ApiMart | No hay montaje: son imágenes fijas |

### Detalle de los formatos con procedimiento propio

**Podcast** [M4-L4.2] — el segundo interlocutor se crea con el prompt de la biblioteca (apartado Podcast), que
genera a la otra persona **y adapta el fondo**: misma habitación, encuadre distinto. El método viejo (duplicar la
imagen, cambiar la persona y voltearla) queda raro porque el fondo es idéntico. En podcast **la cámara nunca se
mueve** y las micro-acciones son las **reacciones del que escucha**: asentir, pensar antes de responder, levantar la
cabeza sorprendido.

**Dualcast** [M4-L4.4] — dos personas en el **mismo plano**. La clave es un **doble bloque de micro-acción**: se
describe al que habla **y** al que escucha (`only listening, occasionally nodding slightly… no interruption`). Sin
eso el modelo hace hablar a los dos o congela al segundo. Se identifican por posición, **`LEFT` / `RIGHT` en
mayúsculas**.

**Voz en off** [M4-L4.3] — **orden estricto: todas las imágenes primero, animación después.** Estética de foto de
móvil (`Authentic iPhone photography, subtle iPhone HDR, no cinematic grading`), no cinematográfica. Cada imagen
ancla la ropa al character sheet para que la rutina parezca un mismo día.

**Trend viral** [M4-L4.5] — descargar el TikTok: clic derecho → copiar enlace → buscar "download TikTok from link"
→ pegar → Descargar. **Da igual si lleva marca de agua**: solo es la base sobre la que van los clips propios.

**Imágenes estáticas** [M4-L4.6] — describir el producto en una frase → el agente devuelve análisis y **7 formatos**
→ darle **precio, mercado y paleta** (si no dices mercado, **asume España**) → confirmar → el agente pide una **foto
limpia del producto sobre fondo neutro** → devuelve los prompts → **sustituir el marcador `marca`** por el nombre
real → generar en ApiMart. Pedir más con "dame más formatos".

---

## Track Animados · el segundo método

Todo lo anterior es el **track realista** (UGC con avatar humano). Lo que sigue es el **track animado**, un método
distinto del segundo curso de la academia (*Creativos Animados*): anuncios en estilo Pixar, claymation, Wes Anderson,
sci-fi o realista-Apple, sin persona a cámara [M6-L6.1].

No es una variante del anterior: cambia la cadena entera. **Aquí no hay Omni, ni Grok, ni avatar hablando, ni capa
de realismo.** Lo que sí comparten: el principio de que el resultado se decide en la planificación (~80 %), el
formato 9:16 en 2K, el acceso vía ApiMart/KIE, la voz en ElevenLabs y el montaje en CapCut con transición Mix.

> El curso avisa de que **se está regrabando entero** [M6-L6.1]. Este track es una foto a 2026-09-03.

## Fase A0 · Stack del track animado

| Función | Herramienta | Notas |
|---|---|---|
| Planificación | **ChatGPT** | Los 8 prompts encadenados, **todos en la misma conversación** [M6-L6.2] |
| Investigación | **NotebookLM** | Gratis. Datos duros del producto a partir de fuentes reales [M6-L6.2] |
| Imagen | **Nano Banana Pro** vía ApiMart (**0,05 US$/img**) o KIE (**0,09 US$/img**) | 9:16, **2K siempre**: cuesta lo mismo que 1K [M6-L6.2] |
| Vídeo | **Kling 3** (volumen 3) en ApiMart | 720p, 9:16, modo primer+último frame, 3-5 s por clip [M6-L6.2] |
| Voz | **ElevenLabs** | 10.000 créditos gratis/mes. Catálogo → Multilingual V2 · voz clonada propia → V3 [M6-L6.2] |
| Música y SFX | **Epidemic Sound** | 30 días gratis, ilimitado [M6-L6.2] |
| Montaje | **CapCut** gratuito | Sin After Effects ni Premiere [M6-L6.2] |

El curso se desmarca explícitamente de HeyGen, Freepik, Arcads, Wavy y Higgsfield: **mínimo 0,15 US$/imagen** frente
a los 0,05 de ApiMart [M6-L6.2].

## Fase A1 · Planificación · los 8 prompts encadenados

Una sola conversación de ChatGPT de principio a fin. Cada prompt da por hecho lo que cerró el anterior, así que al
llegar al 7 el contexto completo ya está dentro y se puede iterar sin reexplicar nada [M6-L6.2].
Los textos literales están en `prompts.md` § 13 y en `sources/avatarhype-animados/raw/_documento-8-prompts.md`.

| # | Prompt | Dónde se pega | Devuelve |
|---|---|---|---|
| 1 | Avatar + research | ChatGPT | Avatar de cliente + **3 búsquedas** para NotebookLM |
| 2 | Auto-research + insights | **NotebookLM** | **5 insights** con cifras reales |
| 3 | Ángulos | ChatGPT | **3 ángulos**, uno por dolor distinto |
| 4 | Guion | ChatGPT | El guion del anuncio |
| 5 | Storyboard | ChatGPT | Estructura visual + metáfora visual |
| 6 | Prompts NB | ChatGPT | Los prompts de imagen, con bloque **Style Lock** |
| 7 | Auditoría completa | ChatGPT | Diagnóstico + guion definitivo + **2 variantes** + storyboard y prompts auditados |
| 8 | Introducción al producto | ChatGPT | Lo anterior con la marca real inyectada |

Paso a paso [M6-L6.2]:

1. **Prompt 1** con tres datos: producto (3-4 frases), mercado y **estilo de animación**. El estilo se elige aquí,
   al principio, no al final: los prompts posteriores lo dan por fijado [M6-L6.1].
2. **NotebookLM** → cuaderno nuevo → *Discover Sources* → pegar las tres búsquedas **una a una**, esperando a que
   cada una termine, y darle a **Importar**.
3. **Prompt 2 en el chat de NotebookLM** (no en ChatGPT) → 5 insights. Iterar hasta que convenzan.
4. **Prompt 3** de vuelta en ChatGPT, sustituyendo el marcador por esos insights → 3 ángulos → **elegir uno**.
5. **Prompt 4** con el ángulo elegido escrito arriba → guion.
6. **Prompt 5** → storyboard. Es el punto de iteración fuerte: aquí se decide la metáfora visual.
7. **Prompt 6** → prompts de imagen. **En el bloque Style Lock hay que dejar solo el estilo escogido** y borrar
   los demás.
8. **Prompt 7** → auditoría global de todo lo anterior.
9. **Prompt 8** → nombre de producto, marca y 2-3 frases → entregable final.

## Fase A2 · Producción

**Voz** [M6-L6.2] — ElevenLabs. Voz del catálogo → **Eleven Multilingual V2**; voz clonada propia → **V3**. El
instructor clona una voz de TikTok y la modifica un poco.

**Imágenes** [M6-L6.2] — Nano Banana Pro, texto a imagen, **9:16 y 2K**. Se abren varias pestañas y se lanzan en
paralelo. Si hay producto real, se adjunta como imagen de referencia. **Nombrar los archivos P1, P2, P3, P4…** por
el número de prompt del que salen: sin eso, emparejar los frames en el paso siguiente se vuelve inmanejable.

**Clips** [M6-L6.2] — ApiMart → **Kling volumen 3**, 720p, 9:16. Cambiar el modo de «base» a **«Future»** y subir
**la primera imagen y la última**: el clip generado es la **transición animada entre las dos**. Duración **3, 4 o
5 s** (el curso usa 4), audio opcional. El prompt del clip sale del menú de estilos (`prompts.md` § 13.2), uno de
los cinco según el estilo elegido en el Prompt 1.

**Regla estructural del track:** cada clip es una transición entre dos imágenes consecutivas, no un plano generado
de cero. **El número de clips es el número de imágenes menos uno** [M6-L6.2].

## Fase A3 · Montaje en CapCut

Arrastrar todos los clips y la voz de ElevenLabs; **colocar el audio primero** y montar el vídeo contra él
[M6-L6.2]. Valores exactos:

| Ajuste | Valor |
|---|---|
| Velocidad de todos los clips | **1,20** (rango probado 1,20-1,30) |
| Transición | **Mix** → añadir → **aplicar a todas** |
| Duración de la transición | **0,5-0,7 s** |
| Música | **−25 a −30** |
| Efectos de sonido de los propios clips | **−8** |
| Voz | **+5** |

Además: **quitar los silencios largos** de la narración. Después, balancear clip a clip de oído. Track de música
que usa el curso: «Curiosity Kills» (Epidemic Sound) [M6-L6.2].

**No hay capa de realismo en este track.** No se busca que parezca real, se busca que parezca animado — es la
diferencia operativa más visible con el track realista, donde la capa de 8 valores es obligatoria [M4-L4.1.1].
