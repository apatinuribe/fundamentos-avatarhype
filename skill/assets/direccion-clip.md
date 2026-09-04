# Dirección · biblia de continuidad y ficha por clip

> **[ANEXO] Esto no sale del curso.** Es una capa añadida para cerrar la costura entre el guion de El Estratega
> y los dos prompts. Todo lo demás en `assets/` es material del curso con su cita; esto no la tiene y por eso
> va marcado. Si contradice algo citado con `[M…]`, manda lo citado.

Se rellena **entre la Fase 2 (guion) y la Fase 3 (imagen)**. Produce dos cosas: una biblia de continuidad por
anuncio y una ficha por clip.

**Lo que esta plantilla NO hace**, y no debe intentar:

- No escribe el prompt de imagen — eso es el agente 6C (`assets/prompt-imagen.md`).
- No escribe el prompt final del clip — esa es la fórmula `CÁMARA + MOVIMIENTO + MICRO-ACCIÓN + GUION + VOZ + ACENTO`
  (`assets/prompt-clip.md`).
- No toca el guion. El texto que dice el avatar es intocable salvo que lo pidas tú.

Su trabajo es **decidir**, para que esos dos prompts se escriban con criterio en vez de sobre la marcha. Cada
campo lleva anotado a qué ranura alimenta.

---

## 0 · Antes de dirigir: qué preguntar

Clasifica lo que falta y **pregunta solo lo CRÍTICO de entrada**. Lo OPCIONAL se decide con criterio, no se
consulta. Si el guion ya lo dice, no se pregunta.

| Nivel | Qué es | Ejemplos típicos |
|---|---|---|
| **CRÍTICO** | Sin esto no se puede generar | ¿Hay foto de referencia real del avatar? · ¿El avatar habla o hay voz en off? · ¿Producto físico que se manipula en cámara? · Formato (de los nueve) |
| **IMPORTANTE** | Cambia la producción, pero hay un valor por defecto defendible | Registro del set: casero/UGC o premium · Acento · Duración objetivo del anuncio |
| **OPCIONAL** | Lo decides tú | Color de la taza, si lleva gafas, qué se ve en la estantería del fondo |

Cuando preguntes, **ofrece opciones cerradas y recomienda una** con una línea de porqué. Preguntar en abierto
devuelve respuestas vagas que hay que volver a preguntar.

---

## 1 · Biblia de continuidad

Se escribe **una vez por anuncio, antes del primer clip, y no se renegocia después**. Es lo que impide que el
avatar cambie de cara, de camiseta o de cocina entre el clip 2 y el clip 5.

```
ANUNCIO: ................................................
Formato (de los nueve): .................................
Track: realista
```

| Bloque | Qué fijar | Alimenta |
|---|---|---|
| **Avatar · identidad** | De qué foto real sale. Edad aparente, rasgos, pelo. **Las imperfecciones concretas que se conservan** | `Character` del 6C |
| **Avatar · vestuario** | Prenda, color, textura, accesorios. Uno por uno, no "ropa casual" | `Clothing` del 6C |
| **Set** | Habitación, mobiliario visible, props fijos, qué hay en el fondo | `Context` del 6C |
| **Luz** | Dirección, temperatura, intensidad. Una sola configuración para todo el anuncio | `Cinematic Light` del 6C |
| **Cámara base** | 9:16 siempre. Distancia por defecto (busto / medio) y look (UGC casero, experto, comercial) | `Camera` del 6C |
| **Voz** | Género × edad · acento. **Latino neutro no se pide** (el modelo tiende a él); **español de España sí** | ranuras `VOZ` y `ACENTO` |
| **Energía** | Cómo habla y cómo se mueve esta persona: pausada, nerviosa, cercana, tajante | gobierna las micro-acciones |
| **Anclas** | Los **3-5 rasgos que no pueden cambiar en ningún clip**. Menos de 3 es poco; más de 5 no lo sostiene el modelo | `Consistency Anchors` del 6C |

**Regla de imperfección:** el avatar se diseña contra la limitación del modelo. Piel impoluta y cara simétrica
+ la capa de textura que añade Omni al animar = canta a IA. Las imperfecciones van en la biblia como decisión,
no se dejan al azar.

---

## 2 · Ficha de dirección por clip

Una por clip, en orden. El clip 0 es el hook.

```
CLIP 0 — .......................................
```

| Campo | Cómo se decide | Alimenta |
|---|---|---|
| **Función** | Una sola, de la estructura de El Estratega: hook · problema · agitación · mecanismo · demostración · beneficio · CTA. **Si no sabes cuál es, el clip sobra** | verificación |
| **Guion** | Literal, tal cual salió. No se reescribe | ranura `GUION` |
| **¿Habla?** | Sí → Omni. No → Grok **y `NO TALKING` obligatorio en el prompt** | elección de modelo |
| **Duración** | Se mide contra el guion, no se elige por defecto. Corto → 6 s, largo → 8 s. Mejor pasarse y recortar en edición | configuración |
| **Imagen** | ¿Reutiliza la del clip anterior o hace falta una nueva? En clips hablados sin cambio de postura se reutiliza **siempre la misma** | Fase 3 |
| **Encuadre** | Plano y distancia. Cambiar de plano **es otro clip y otra imagen**: aquí no se corta dentro de un clip | ranura `CÁMARA` |
| **Movimiento de cámara** | Estático · zoom lento a la cara · zoom rápido al hablar · retroceso que revela · órbita lenta · seguimiento · push-in a los ojos. **Si hay manipulación de producto: ESTÁTICA, sin excepción** | ranura `MOVIMIENTO` |
| **Micro-acción** | Qué hace con las manos, la cara o un objeto. **Se escribe ya en inglés y entre corchetes**, y se coloca en el punto exacto de la frase: `[Points up to the right]`. Sin micro-gesto el clip se lee como IA | ranura `MICRO-ACCIÓN` |
| **Coreografía** | Si el gesto reserva hueco para una superposición, decirlo aquí: *señala arriba a la derecha al decir "hace 3 meses" porque **ahí** va el antes* | edición |
| **Dirección de voz** | **Solo si es voz en off de ElevenLabs**: tono, ritmo, pausas, énfasis. Si habla el avatar por Omni, esta fila va en `—`: la voz la pone el modelo y no se dirige | ElevenLabs |
| **Continuidad** | Qué permanece idéntico respecto al clip anterior, y qué cambia **y por qué**. Un cambio sin porqué es un error de continuidad | biblia |
| **Salida** | Cómo conecta con el siguiente. La única transición del método es **Mix** | CapCut |

---

## 3 · Control de calidad antes de generar nada

- [ ] Cada clip tiene **una** función declarada, y entre todos cubren hook → problema → agitación → mecanismo →
      demostración → beneficio → CTA.
- [ ] Las anclas de consistencia aparecen en **todos** los prompts de imagen, con las mismas palabras.
- [ ] Ningún clip cambia vestuario, set o luz sin que la ficha diga por qué.
- [ ] Todo clip sin guion lleva `NO TALKING`.
- [ ] Todo clip con manipulación de producto tiene la cámara estática y `Photorealistic, realistic hands`.
- [ ] Las micro-acciones están en inglés, entre corchetes, dentro del guion y en el punto exacto.
- [ ] Las duraciones se midieron contra el guion, una a una.
- [ ] Las direcciones de voz que no van por ElevenLabs están en `—`, no inventadas.
- [ ] Los gestos que reservan hueco para una superposición están anotados para el montaje.

---

## 4 · Lo que no se importa de un director al uso

Un agente genérico de dirección audiovisual trae cosas que **empeoran** el resultado con estos modelos:

| No hacer | Por qué |
|---|---|
| Dirigir en prosa cinematográfica | La fórmula del clip es por ranuras y seca. El párrafo literario rinde peor en Omni y Grok |
| Listas de *negative prompt* / "EVITAR" | Estos modelos no las toman como se espera. El equivalente aquí son positivos incrustados: `NO TALKING`, `No talking, mouth closed`, `Photorealistic, realistic hands` |
| Cambiar de plano para "sostener la retención" | Un clip es una generación desde una imagen. Cambiar de plano es otro clip |
| Movimiento de cámara por espectáculo | Rompe la acción, y con producto en mano la rompe siempre |
| Dirigir tono y pausas de una voz de Omni | No se controla. Solo se dirige la voz cuando la pone ElevenLabs |
| Reescribir el guion para que "suene mejor" | El guion es lo importante del clip; lo negociable es la parte visual, no al revés |
