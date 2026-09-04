# avatarhype - Manual completo

Generado con `python pipeline/build_manual.py avatarhype` a partir de `knowledge/avatarhype/`. No editar a mano: los cambios se hacen en los documentos de origen y se regenera.

Las referencias entre corchetes (`[M4-L4.1.1]`) apuntan a la leccion de origen en `sources/avatarhype/notes/`.

## Indice

**[Parte 1 - El proceso](#parte-1---el-proceso)** - El metodo completo, de la idea al archivo montado, en el orden en que se ejecuta.

- [Fase 0 · Stack](#fase-0--stack)
- [Fase 1 · Estrategia](#fase-1--estrategia)
- [Fase 2 · Guion (agente El Estratega)](#fase-2--guion-agente-el-estratega)
- [Fase 3 · Imagen](#fase-3--imagen)
- [Fase 4 · Clips](#fase-4--clips)
- [Fase 5 · Limpieza](#fase-5--limpieza)
- [Fase 6 · Edición en CapCut](#fase-6--edición-en-capcut)
- [Fase 7 · Variantes de montaje por formato](#fase-7--variantes-de-montaje-por-formato)
- [Track Animados · el segundo método](#track-animados--el-segundo-método)
- [Fase A0 · Stack del track animado](#fase-a0--stack-del-track-animado)
- [Fase A1 · Planificación · los 8 prompts encadenados](#fase-a1--planificación--los-8-prompts-encadenados)
- [Fase A2 · Producción](#fase-a2--producción)
- [Fase A3 · Montaje en CapCut](#fase-a3--montaje-en-capcut)

**[Parte 2 - Practicas e insights](#parte-2---practicas-e-insights)** - Reglas duras, criterios de decision y errores caros.

- [Reglas duras (romperlas rompe el resultado)](#reglas-duras-romperlas-rompe-el-resultado)
- [Criterios de decisión](#criterios-de-decisión)
- [Realismo: por qué un vídeo canta a IA](#realismo-por-qué-un-vídeo-canta-a-ia)
- [Estrategia](#estrategia)
- [Trabajar con los agentes](#trabajar-con-los-agentes)
- [Escribir prompts de clip](#escribir-prompts-de-clip)
- [Encadenar imágenes](#encadenar-imágenes)
- [Edición](#edición)
- [Costes y economía](#costes-y-economía)
- [Errores que salen caros](#errores-que-salen-caros)
- [Hueco conocido](#hueco-conocido)
- [Track Animados · reglas y criterios [M6-*]](#track-animados--reglas-y-criterios-m6-)

**[Parte 3 - Prompts](#parte-3---prompts)** - Kit operativo: plantillas parametrizadas y menus.

- [1 · Estructura del prompt de clip](#1--estructura-del-prompt-de-clip)
- [2 · Menú de cámara](#2--menú-de-cámara)
- [3 · Menú de micro-acciones](#3--menú-de-micro-acciones)
- [4 · Menú de voz](#4--menú-de-voz)
- [5 · Menú de acento](#5--menú-de-acento)
- [6 · Imagen · el método 6C](#6--imagen--el-método-6c)
- [7 · Imagen · plantillas de continuidad](#7--imagen--plantillas-de-continuidad)
- [8 · Imagen · pipeline de moda](#8--imagen--pipeline-de-moda)
- [9 · Imagen · estética iPhone (voz en off y trends)](#9--imagen--estética-iphone-voz-en-off-y-trends)
- [10 · Clips sin habla (Grok)](#10--clips-sin-habla-grok)
- [11 · Formatos con estructura de prompt propia](#11--formatos-con-estructura-de-prompt-propia)
- [12 · Prompts de entrada a los agentes](#12--prompts-de-entrada-a-los-agentes)
- [13 · Ads animados · el sistema de 8 prompts [M6-L6.2]](#13--ads-animados--el-sistema-de-8-prompts-m6-l62)

**[Parte 4 - Ejemplos](#parte-4---ejemplos)** - Los casos completos del curso, con sus guiones y cifras.

- [Índice de casos](#índice-de-casos)
- [1 · UGC sin producto — piel / acné [M4-L4.1.1]](#1--ugc-sin-producto--piel--acné-m4-l411)
- [2 · UGC con producto — BLUME Greens [M4-L4.1.2]](#2--ugc-con-producto--blume-greens-m4-l412)
- [3 · Moda — DAM PROJECT [M4-L4.1.3]](#3--moda--dam-project-m4-l413)
- [4 · App / SaaS — Monalisa [M4-L4.1.4]](#4--app--saas--monalisa-m4-l414)
- [5 · Podcast — clase media / invertir [M4-L4.2]](#5--podcast--clase-media--invertir-m4-l42)
- [6 · Voz en off — "Un día conmigo" (BLUME) [M4-L4.3]](#6--voz-en-off--un-día-conmigo-blume-m4-l43)
- [7 · Dualcast — leggings reductores [M4-L4.4]](#7--dualcast--leggings-reductores-m4-l44)
- [8 · Trend viral [M4-L4.5]](#8--trend-viral-m4-l45)
- [9 · Imágenes estáticas [M4-L4.6]](#9--imágenes-estáticas-m4-l46)
- [10 · Estrategia — los 12 ángulos (champú de pelo rizado) [M3-L3.3.1]](#10--estrategia--los-12-ángulos-champú-de-pelo-rizado-m3-l331)
- [11 · Salidas de El Estratega [M3-L3.3.3]](#11--salidas-de-el-estratega-m3-l333)
- [12 · Ejemplos menores](#12--ejemplos-menores)
- [Los tres agentes [M1-L1.4.4]](#los-tres-agentes-m1-l144)
- [Hueco](#hueco)
- [13 · Track Animados — los tres anuncios de referencia [M6-L6.2]](#13--track-animados--los-tres-anuncios-de-referencia-m6-l62)

---

# Parte 1 - El proceso

_El metodo completo, de la idea al archivo montado, en el orden en que se ejecuta. Origen: `knowledge/avatarhype/proceso.md`._

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

---

# Parte 2 - Practicas e insights

_Reglas duras, criterios de decision y errores caros. Origen: `knowledge/avatarhype/practicas.md`._

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

# Parte 3 - Prompts

_Kit operativo: plantillas parametrizadas y menus. Origen: `knowledge/avatarhype/prompts.md`._

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

---

# Parte 4 - Ejemplos

_Los casos completos del curso, con sus guiones y cifras. Origen: `knowledge/avatarhype/ejemplos.md`._

Casos completos del curso, con sus cifras y sus guiones. Sirven de patrón: cada uno enseña una decisión distinta.
Los prompts literales de cada caso están en `prompts.md`; aquí van los guiones, las estructuras y los recuentos.

---

## Índice de casos

| Caso | Formato | Producción | Fuente |
|---|---|---|---|
| Piel / acné (sin producto) | UGC 1 persona | 3 imágenes · 4 clips Omni | [M4-L4.1.1] |
| BLUME Greens | UGC con producto | 5 imágenes (4 usadas) · 3 Omni + 1 Grok | [M4-L4.1.2] |
| DAM PROJECT (tienda de ropa) | Moda | avatar + sheet + 4 outfits · 3 Omni + 4 Grok | [M4-L4.1.3] |
| Monalisa (app de entrenamiento) | App / SaaS | **1 imagen** · 3 Omni + screen recording | [M4-L4.1.4] |
| Clase media / invertir | Podcast 2 personas | 2 avatares · 8 clips | [M4-L4.2] |
| Un día conmigo (BLUME) | Voz en off | sheet + muchas imágenes · Grok + ElevenLabs | [M4-L4.3] |
| Leggings reductores | Dualcast | **1 imagen** con las dos · 4 clips Omni | [M4-L4.4] |
| "It always looks worse…" | Trend viral | 3 imágenes · 1 clip | [M4-L4.5] |
| Juguete Montessori / webs 500 € | Imágenes estáticas | 7 prompts por producto | [M4-L4.6] |
| Champú de pelo rizado | (estrategia) | 12 ángulos · mecanismo nivel 3 | [M3-L3.3.1], [M3-L3.3.2] |
| Digestión +35 · webs · SaaS patrimonio | (estrategia) | 3 salidas de El Estratega | [M3-L3.3.3] |
| Cloudy · Sleepy · FitMind | **Track animado** | 3 anuncios de referencia, sin guion publicado | [M6-L6.2] |

---

## 1 · UGC sin producto — piel / acné [M4-L4.1.1]

**Es el caso de referencia del curso**: el único que enseña la edición completa.

**Producción**: 1 imagen de avatar (referencia de Pinterest) + 2 imágenes de estado (con acné / sin acné, en 1:1 para
superponer) · 4 clips Omni.

**Guion, clip a clip:**

| Clip | Cámara | Guion |
|---|---|---|
| 1 · Hook | Seguimiento al caminar | "Esta era mi piel hace 3 meses `[Points up to the right]` y esta es mi piel ahora. `[points up to the left]`" |
| 2 · Problema | Seguimiento al caminar | "Pensaba que necesitaba una rutina de 10 pasos para quitarme el acné. Tenía un producto para los granos, otro para las manchas, otro para la grasa… y cada vez que otro se ponía de moda, lo compraba." |
| 3 · Giro | **Estática** | "Cuanto más hacía, peor estaba mi piel. Hasta que entendí que el problema no era que me faltaran productos, sino lo contrario. Así que simplifiqué por completo mi rutina y me enfoqué en lo que realmente necesitaba." |
| 4 · CTA | Zoom lento a la cara | "Y, sinceramente, no esperaba ver un cambio así en solo tres semanas. Si quieres que te mande exactamente qué eliminé de mi rutina, qué empecé a usar y por qué, comenta «ACNÉ»." |

**Lo que enseña**: los gestos del clip 1 (`points up to the right` / `to the left`) **reservan el hueco** donde en
edición entran las imágenes de antes y después. El gesto y el montaje se diseñan juntos.

**Montaje**: importar → orden → cortar espacios muertos → velocidad 1.12–1.20 clip a clip → capa de realismo de
punta a punta → transiciones Mix → superponer las dos imágenes detrás del avatar (duplicar + quitar fondo + bajar
volumen) con animación Zoom/Shake/Slide Up → música.

---

## 2 · UGC con producto — BLUME Greens [M4-L4.1.2]

**Producción**: 5 imágenes generadas, **4 usadas** · 3 clips Omni (hablados) + 1 Grok (producto solo).

**Secuencia de imágenes**, cada una editando la anterior: avatar con el producto en mano → mismo encuadre con el
vaso ya en la encimera → guardando el bote en el armario → producto solo sin persona.

**Guion:**

| Clip | Micro-acción | Guion |
|---|---|---|
| 1 · Hook | `[While speaking, she pours one scoop of BLUME Greens into the glass, then uses the same scoop to stir the drink]` | "Si todos los días te viene este pensamiento a la cabeza quizá ha llegado el momento de prestar más atención a tu cuerpo." |
| 2 | `[she start drinkin the glass of greens]` | "No todo consiste en hacer cambios enormes. A veces empiezas por pequeños hábitos que puedes mantener en el tiempo." |
| 3 · CTA | `[While speaking, she puts the BLUME container away in the kitchen cabinet.]` | "Si quieres conocer todos sus ingredientes y cómo incorporarlo a tu rutina, te lo dejo aquí abajo." |
| 4 | — (Grok, `No talking, mouth closed`) | Producto solo con partículas |

**Lo que enseña — patrón reutilizable**: el clip 4 **traduce los ingredientes en metáfora visual**:
fibra → hebras finas · extractos vegetales → fragmentos de hoja translúcidos · probióticos → micro-esferas
suspendidas · vitamina → puntos dorados de luz. Sirve para cualquier producto con lista de ingredientes.

**Montaje**: el más simple del curso — clips, capa de realismo, **rótulo fijo de retención**, música.
Sin transiciones ni superposiciones.

---

## 3 · Moda — DAM PROJECT [M4-L4.1.3]

**Producción**: avatar → character sheet → cuerpo entero → pared blanca → 4 outfits (cada uno sobre el anterior) ·
3 clips Omni hablados (reutilizando **la misma imagen**) + 4 clips Grok de pose, 6 s a 720p.

**Guion:**

| Clip | Guion |
|---|---|
| 1 · Hook | "Si te gusta el estilo vintage `[points to the left]` o streetwear `[points to the right]` de verdad que tengo que enseñarte todo lo que me he comprado en esta tienda porque estoy obsesionada" |
| 2 | "Es una tienda de ropa donde todo cuesta $15. Y cuando digo todo, es todo. Desde chaquetas y vaqueros hasta camisetas, vestidos… y un montón de prendas únicas que no ves en todos lados" |
| 3 · CTA | "De verdad que si te gusta vestir diferente y encontrar auténticos chollos, tienes que echarle un vistazo. Se llama DAM PROJECT. Te dejo la tienda aquí abajo." |

**Clips de pose**: A · de pie girando ligeramente (outfits 1 y 2) · B · andando hacia cámara (3) · C · giro de 360° (4).

**Lo que enseña**:
- El **reparto por clip**: 3 Omni + 4 Grok en el mismo anuncio, ~0,048 US$ cada clip Grok.
- La **inversión de planos** en el montaje: los clips de pose ocupan el fotograma completo y el clip hablado va
  recortado y pequeño **abajo a la derecha**.
- Los micro-gestos del clip 1 reservan hueco para las dos imágenes de estilo, igual que en el caso 1.
- El nombre aparece como **DAM PROJECT** en el documento; los subtítulos lo transcriben "Dumb Project" — vale el
  documento.

---

## 4 · App / SaaS — Monalisa [M4-L4.1.4]

**Producción**: **una sola imagen** de avatar · 3 clips Omni + una grabación de pantalla de la app.

**Guion:**

| Clip | Micro-acción | Guion |
|---|---|---|
| 1 · Hook | `She tucks her hair behind their ear while saying in the first 3 seconds of the video:` | "Si llevas tiempo queriendo empezar a entrenar, necesito enseñarte porque me está encantando. Se llama Monalisa. No se quien me la ha estado ocultando, pero…" |
| 2 · Qué es | — | "Es una app de entrenamiento super fácil de usar que te dice exactamente que hacer en cada sesión. Si eres como yo y muchas veces llegas al gimnasio sin saber por donde empezar, esto te viene genial." |
| 3 · CTA | — | "Lo mejor es que tienes tu rutina lista. Solo tienes que abrir la app y entrenar, sin complicarte ni perder el tiempo. De verdad, si todavía no la conocías, dale una oportunidad porque está super super bien." |

**Salida de El Estratega para este caso** (entrada: `es una app de entrenamiento para mujeres`):
- **Dolores**: "no sé qué ejercicio hacer" · "empiezo con ganas y abandono a las dos semanas" · "me tiro horas
  viendo rutinas en TikTok y sigo sin resultados".
- **Deseos**: sentirse más fuerte y segura · glúteos y piernas tonificados · bajar grasa sin vivir a dieta · que
  alguien le diga exactamente qué hacer.
- **Objeción principal**: "otra app más de entrenamiento, ya he probado mil".
- Además: 10 ángulos, mecanismo propuesto y nivel de conciencia recomendado.

**Lo que enseña**:
- El anuncio más barato del curso: **una imagen** para los tres clips.
- **`while saying in the first 3 seconds of the video`** para acotar el gesto.
- **El guion se retoca al montar**: el documento dice "necesito enseñarte porque me está encantando" y el vídeo
  final dice "necesito enseñarte **esta app** porque me está encantando".
- Orden de montaje estricto: avatar solo → logo → app a pantalla completa con el avatar abajo a la derecha.

---

## 5 · Podcast — clase media / invertir [M4-L4.2]

**Producción**: 2 avatares en encuadres distintos de la misma habitación (el segundo lo crea el prompt de la
biblioteca, que **adapta el fondo**) · **8 clips**, uno por intervención.

**Diálogo:**

| Clip | Quién | Guion |
|---|---|---|
| 1 | Ella (lee el móvil, levanta la cabeza, sorpresa sutil) | "8 de cada 10 españoles dicen que les cuesta llegar a fin de mes." |
| 2 | Él (asiente) | "Una pregunta rápida. ¿Tú te consideras clase media?" |
| 3 | Ella (piensa antes de responder) | "mm yo diría que sí" |
| 4 | Él | "Es curioso porque en España todos se consideran clase media, pero casi nadie vive con la tranquilidad que asociábamos a la clase media hace unos años, ¿no?" |
| 5 | Ella | "O sea que hemos normalizado de alguna manera el ir tan justos, ¿verdad?" |
| 6 | Él | "Hoy mucha gente se considera clase media… y aun así no consigue ahorrar más de 100 euros al mes. Y cuando no consigues ahorrar, tampoco puedes hacer que ese dinero empiece a crecer." |
| 7 | Ella (asiente) | "Sí sí, totalmente" |
| 8 | Él · CTA | "Por eso aprender a gestionar e invertir tu dinero ya no es algo solo para quien quiere hacerse rico. Es una habilidad básica. Si quieres aprender, comenta «INVERTIR» aquí abajo." |

**Estructura**: dato impactante → pregunta al otro → respuesta dubitativa → contraste → reformulación → dato con
mecanismo → validación → CTA.

**Lo que enseña**:
- **El clip 7 son dos palabras.** En podcast merece la pena generar clips cortísimos solo para el *reaction shot*.
- La cámara **nunca se mueve** y las micro-acciones son reacciones del que escucha.
- En el montaje, los clips se **apilan solapándose** para que la cámara corte a la otra persona antes de que la
  primera termine de hablar.

---

## 6 · Voz en off — "Un día conmigo" (BLUME) [M4-L4.3]

**Producción**: character sheet → **todas** las imágenes primero (coche, conduciendo, gimnasio, cocina, plato en
primera persona, producto, sushi, impresora de tickets, paseo) → después los clips en Grok, todos con `NO TALKING`
→ narración en ElevenLabs.

**Narración**: entrenar → tostadas con aguacate y huevo → *"y hay una cosa que nunca falta en mi rutina, Blume"* →
estrés de tener un negocio → trabajar → pausa para comer → paseo → CTA con descuento.

**Salida de El Estratega**: ángulos **"el culpable oculto"** (*no es la comida, es cómo la estás digiriendo*) y
**"el antes y el después"**; rótulo propuesto **"Un día conmigo como dueña de un negocio"**; apertura
*"Acompáñame en un día normal, porque siempre me preguntáis cómo organizo todo"*.

**Lo que enseña**:
- **Cualquier objeto sirve de plano de apoyo**: el clip de la impresora de tickets no lleva persona y narra el
  negocio.
- Estética iPhone explícita (`no cinematic grading`), no cinematográfica.
- **El audio manda**: los clips de 6 s se recortan a 2–3 s y los cortes se cuadran con la narración.
- El **zoom falso con fotogramas clave** (rombo en *Escalar*, 100 % → 150 %) sustituye a generar clips con zoom.

---

## 7 · Dualcast — leggings reductores [M4-L4.4]

**Producción**: **una sola imagen** con las dos personas en el mismo plano · 4 clips Omni, cada uno con **doble
bloque de micro-acción**.

| Clip | Habla | Guion |
|---|---|---|
| 1 · Hook | LEFT | "Yo me miro al espejo con estos leggings y digo: joder qué buena estoy" `[se echa a reír]` |
| 2 · Mecanismo | RIGHT | "Han desarrollado una tecnología que es otro nivel, te levanta, te encoge la cintura y te hace la forma de reloj de arena" |
| 3 · Prueba + objeción | LEFT | "Es que voy a dejar una foto aquí arriba `[She points to the top of the screen]` porque si no no van a entenderlo. Y fabricado en España, que la mierda que compramos en Shein está llena de microplásticos" |
| 4 · CTA | RIGHT | "Sí sí, calidad precio son una pasada. Vamos a dejar aquí abajo el link que luego siempre nos lo preguntáis y así podéis echarle un ojo." `[They both wave goodbye to the camera.]` |

**Estructura**: hook emocional exagerado → mecanismo → prueba visual + ataque a la competencia → validación + CTA.

**Lo que enseña**:
- El **doble bloque de micro-acción** (`actively speaking` / `only listening, occasionally nodding slightly… no
  interruption`) con `LEFT`/`RIGHT` en mayúsculas.
- `[She points to the top of the screen]` **reserva el sitio** de la imagen superpuesta — tercer caso del mismo
  truco.
- El clip 4 cierra con **las dos despidiéndose**: una acotación compartida para las dos personas en un solo clip.
- Este formato es el único cuya edición va **dentro del propio vídeo de la lección**, no en un bloque aparte.

---

## 8 · Trend viral [M4-L4.5]

**Frase del trend**: *"Just remember, it always looks worse, before it looks better."*

**Producción**: 3 imágenes (el "antes" con acné desde otro ángulo · selfie en el coche con estética *photo dump* ·
el "después" con el producto en la mano) · 1 clip. **El avatar no habla**: el audio original del TikTok sostiene el
anuncio.

**Lo que enseña**:
- Descargar el TikTok (clic derecho → copiar enlace → buscador "download TikTok from link"). **Da igual si lleva
  marca de agua**: es solo la base.
- El TikTok va en la pista principal, cortado por sus propios cambios de plano; el texto del trend se **traduce al
  español** encima; el producto entra al final.

---

## 9 · Imágenes estáticas [M4-L4.6]

**A · Producto físico — juguete Montessori de madera, 1 a 3 años.** Paleta pedida: **blanco y verde militar**.
Formatos destacados de los 7 que devuelve el agente:
- **Progresión temporal** — "de 4 minutos a 28 en 12 semanas" (tiempo de atención del niño).
- **Ticket comparativo** — lo que se gasta en juguetes con luces frente a un solo juguete Montessori.
- **Foro** — alguien pregunta si los juguetes Montessori valen lo que cuestan o es puro marketing.
- **Antes/después** — el niño rodeado de juguetes hiperestimulantes vs. jugando con uno solo.
- **Podcast de Spotify** con el nombre de marca en la carátula.

**B · Servicio digital — creación de páginas web por 500 €**, **sin ninguna referencia visual**: testimonio,
antes/después, características, ticket de ahorro, foro, búsqueda, **presupuesto tipo Excel**, comparación y
progresión.

**Lo que enseña**: el formato funciona igual para producto físico que para servicio sin nada que fotografiar.
Antes de generar, **sustituir el marcador `marca`**.

---

## 10 · Estrategia — los 12 ángulos (champú de pelo rizado) [M3-L3.3.1]

Del mismo producto, sin tocar el producto:

| # | Ángulo | Ejemplo |
|---|---|---|
| 1 | Problema / dolor | "¿Te despiertas con el pelo encrespado todas las mañanas?" |
| 2 | Identidad | "Para la chica de pelo rizado que ya lo ha probado todo y no consigue definir sus rizos" |
| 3 | Mecanismo | "El culpable de tener el pelo rizado tan mal es el sulfato que llevan los champús tradicionales" |
| 4 | Beneficio | "Rizos todo el día definidos, habiéndotelo hecho por la mañana en cinco minutos" |
| 5 | Romper objeciones | Contra "todos los champús son iguales, todo es marketing" |
| 6 | Emocional | "Por fin dejo de plancharme el pelo para ocultar mis rizos" |
| 7 | Estatus | "El secreto de las chicas que siempre llevan el pelo rizado perfecto" |
| 8 | Miedo / pérdida | "Un champú con sulfatos está dañando cada vez más tu pelo de forma irreversible" |
| 9 | Comodidad | "Te lo haces por la mañana en cinco minutos y ya estás lista para todo el día" |
| 10 | Precio / valor | "Por menos de lo que vale un desayuno tienes el champú para todo el mes" |
| 11 | Comparación | "Lo que en la peluquería te tienes que hacer cada semana, desde tu casa y a un cuarto del precio" |
| 12 | Rompe mitos | "El rizo no se define poniendo más y más producto" |

**Mecanismo para nivel 3** (mismo producto) [M3-L3.3.2]:

> "Todos los champús de pelo rizado que tienes actualmente en el mercado y que probablemente usas tienen
> **sulfatos**, que con cada lavado te están deteriorando tu rizo de forma irreversible. En cambio, mi champú,
> además de no tener sulfatos, tiene una **capa de aloe vera** que actúa como barrera y protege la hidratación que
> produce tu propio rizo."

**Estructura del mecanismo**: culpable → daño irreversible → mi producto no lo tiene → **y además** un
diferenciador propio.

---

## 11 · Salidas de El Estratega [M3-L3.3.3]

### A · Suplemento para digestión / inflamación — mujeres +35

- **Dolores**: "acabo de comer y ya parece que estoy de varios meses" · "me levanto bien pero por la tarde no me
  abrocho ni el pantalón" · "cada comida me cae súper pesada" · "evito ciertos alimentos porque sé cómo voy a
  acabar".
- **Deseos**: comer sin miedo a la hinchazón · volver a ponerse la ropa sin sentirse incómoda · digestión más
  tranquila · recuperar confianza con su cuerpo.
- **Objeciones**: "seguro que es otro suplemento que no hace nada" · "ya he probado probióticos y no noté nada" ·
  "no quiero depender de pastillas" · "¿cuánto tardaré en notar algo?".
- **Ángulos**: *no es grasa, es inflamación* · *el culpable está en tu digestión* · *el problema puede no ser lo que
  comes sino cómo lo digieres*.
- **Hooks**: "Después de los 35 todo cambia" · "Si después de los 35 notas que todo te sienta peor, no te lo estás
  imaginando" · "Antes de eliminar el pan, la pasta o los lácteos, escucha esto" · "La rutina de los 30 segundos" ·
  "La barriga que aparece durante el día".

**Anuncio desarrollado — ángulo "no es grasa, es inflamación"** (formato de salida del agente: rótulo · visual ·
guion):

| Clip | Rótulo / visual | Guion |
|---|---|---|
| 0 · hook | Mujer intentando abrocharse el pantalón después de comer | "Si por la mañana te queda bien la ropa y por la tarde parece que has engordado, puede que no sea grasa." |
| 1 · problema | Se toca la barriga con incomodidad después de comer | "Muchas mujeres después de los 35 viven con el vientre hinchado casi todos los días y acaban pensando que es normal." |
| 2 · mecanismo | — | "Muchas veces el problema no es cuánto comes, sino cómo haces la digestión." |
| 3 · demostración | Tomando el suplemento antes de comer | "Por eso empecé a apoyar mi digestión antes de las comidas y dejé de sentir esa pesadez constante." |
| 4 · beneficio | Caminando, riéndose, ropa ajustada, sin incomodidad | "La diferencia no fue verme más delgada, sino volver a sentirme ligera durante todo el día." |
| 5 · CTA | Primer plano del producto | "Si tú también acabas cada comida sintiéndote inflamada, te lo dejo aquí abajo para que le eches un vistazo." |

### B · Servicio de creación de páginas web

- **Dolores**: "mi negocio ni siquiera aparece en Google" · "la gente me pregunta por Instagram pero no compra" ·
  "mi web parece de hace 10 años".
- **Ángulos**: *tu negocio pierde clientes cada día* · *Instagram no es tu negocio* · *parecer profesional vende
  más* · *la web trabaja mientras duermes* · rompe mitos · mecanismo · comparación · tiempo · identidad.
- **Mecanismo**: "No pierdes clientes por tu precio, los pierdes porque no transmites confianza."
- **Recomendación del propio agente**: **no empezar diciendo "hacemos páginas web"**; empezar mostrando el dinero
  que se pierde por no transmitir confianza online y presentar la web como la solución lógica.
- **Guion**: hook "Estás perdiendo clientes" (visual: alguien busca el negocio en Google, entra en Facebook e
  Instagram y no encuentra web) → "Cada día hay personas buscando exactamente lo que vendes y terminan comprando a
  otro" → "Cuando quieren saber si pueden confiar en ti, solo encuentran un perfil de redes" → "Y si dudas tú,
  imagina un cliente que no te conoce" → mecanismo → "Una web profesional trabaja por ti las 24 horas" → CTA.

### C · SaaS de gestión de patrimonio — clientes de alto patrimonio

- **Dolores**: patrimonio repartido entre varios bancos sin foto completa · tiempo perdido consolidando informes en
  Excel · no saber cuánto se gana después de comisiones e impuestos.
- **Objeciones**: "ya tengo un asesor financiero" · "¿mis datos van a estar seguros?" · "parece demasiado complejo".
- **Guion**: "El problema no es cuánto patrimonio tienes, es que está repartido por todas partes. Cuando tienes que
  abrir cinco plataformas para entender cómo vas, ya estás tomando decisiones con información incompleta… La
  diferencia es tener todo tu patrimonio consolidado en un solo lugar: bancos, inversiones, inmuebles y liquidez."

---

## 12 · Ejemplos menores

**Micro-acción** [M1-L1.4.1] — la demostración del vídeo (min 2:30): el avatar dice "hey, hola" y **se ajusta las
gafas**; segunda variante, se ajusta la gorra. Es todo el argumento de por qué la micro-acción importa.

**Quitamarcas** [M1-L1.4.2] — los cuatro casos mostrados: (1) encimera de cocina, fondo fijo → muy bueno con el modo
**general**; (2) persona caminando por detrás → modo **avanzado**, buen resultado; (3) pijama + cama → se nota un
poco; (4) ordenador justo detrás de la marca → se nota "un pelín más", **se resuelve reprocesando con el otro modo**.

---

## Los tres agentes [M1-L1.4.4]

| Agente | `name:` | Qué hace | ChatGPT |
|---|---|---|---|
| **Prompts Método 6C** | `avatarhype-6c-prompt-engine` | Prompts de imagen hiperrealista con las 6C. **Nunca genera imágenes**: solo prompts, en inglés, en un bloque de código | `chatgpt.com/g/g-6975edfa30b8819183d350d8b87358d4-avatarhypetm-prompts-metodo-6c` |
| **Imágenes estáticas** | `ads-image-architect` | Convierte un producto (físico, infoproducto, servicio o SaaS) en un kit de **7 prompts visuales** para Meta Ads | `chatgpt.com/g/g-6a159bcaea488191bf5e504e8c1787d4-ads-visual-architect-avatarhype-e-com` |
| **El Estratega** | — | Guiones UGC sobre palancas + niveles de conciencia | `chatgpt.com/g/g-6a4b04b0408c8191a13b4d1dbd520923-estrategaavatarhype` |

Ficheros descargados en `sources/avatarhype/raw/adjuntos/skills/` (no versionados en git):
`avatarhype-prompts-metodo-6c.md` (3,7 KB) · `avatarhype-imagenes-estaticas.md` (153 KB) ·
`avatarhype-el-estratega.md` (23 KB).

---

## Hueco

`4.7-ugly-ads` no tiene contenido publicado en la plataforma: no hay ejemplo de ese formato [M4-L4.7].

---

## 13 · Track Animados — los tres anuncios de referencia [M6-L6.2]

El curso de *Creativos Animados* abre enseñando tres anuncios ya terminados con el método, antes de explicar nada.
No publica ni sus guiones ni sus recuentos de producción: lo que se ve es el resultado y la estructura.

| Caso | Producto |
|---|---|
| **Cloudy** (marca Sleepy) | Almohada ergonómica de viscoelástica que mantiene la columna alineada en cualquier postura |
| **Sleepy** | Tira bucal para dormir con la boca cerrada |
| **FitMind** | Suplemento cognitivo |

**Cloudy es el ejemplo que recorre el curso entero**: viene ya escrito dentro del Prompt 1 como muestra de cómo
describir un producto en 3-4 frases (qué es, cómo funciona, en qué se diferencia, qué promete). Copiar esa
descripción como plantilla es la forma rápida de arrancar la cadena.

**Estructura común de los tres:** abren con un **dato duro** antes de nombrar el producto. Es el output directo de
la cadena **Prompt 2 (insights de NotebookLM) → Prompt 3 (ángulos)**: el ángulo se construye sobre una cifra. Ahí
está la diferencia deliberada con el track realista, que arranca por identificación con el avatar [M3-L3.3.1].

### Comparativa de estilo sobre el mismo storyboard

El curso genera el mismo anuncio en **Wes Anderson** y en **Pixar** para enseñar que el estilo no cambia el guion ni
la estructura visual: solo cambian el bloque Style Lock del Prompt 6 y el prompt de transición de cada clip
(`prompts.md` § 13.2). El resto del pipeline es idéntico.

### Por qué este formato, según el curso

Retiene mucho, engancha desde el primer segundo y *"permite vender de una forma menos agresiva"* que el UGC a
cámara [M6-L6.2]. El curso no lo plantea como sustituto del track realista, sino como el segundo camino de la
academia.

---
