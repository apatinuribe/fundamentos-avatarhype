# Plantilla · track animado

Los 13 prompts literales están en `references/prompts.md` § 13. Esto es la hoja de ruta para ejecutarlos.

## Datos que hay que tener antes de empezar

```
PRODUCTO: {3-4 frases: qué es, cómo funciona, en qué se diferencia, qué promete}
MERCADO: {país}
ESTILO ANIMACIÓN: {Pixar 3D | Apple realista | Sci-fi | Claymation | Wes Anderson}
```

El estilo se fija aquí y ya no se toca: lo heredan el storyboard, los prompts de imagen y los de clip.

## La cadena

Una sola conversación de ChatGPT, salvo el paso 2.

| Paso | Dónde | Qué haces | Qué sale |
|---|---|---|---|
| 1 | ChatGPT | Prompt 1 con los tres datos de arriba | Avatar + 3 búsquedas |
| 2a | NotebookLM | Cuaderno nuevo → *Discover Sources* → las 3 búsquedas **una a una** → Importar | Fuentes cargadas |
| 2b | **NotebookLM** | Prompt 2 en el chat del cuaderno | 5 insights con cifras |
| 3 | ChatGPT | Prompt 3 pegando esos insights | 3 ángulos → **elegir uno** |
| 4 | ChatGPT | Prompt 4 con el ángulo elegido escrito arriba | Guion |
| 5 | ChatGPT | Prompt 5 | Storyboard — **iterar aquí** |
| 6 | ChatGPT | Prompt 6 **dejando solo tu estilo en el Style Lock** | Prompts de imagen |
| 7 | ChatGPT | Prompt 7 | Auditoría: guion final + 2 variantes |
| 8 | ChatGPT | Prompt 8 con nombre de producto y marca | Entregable final |

## Producción

**Imágenes** — Nano Banana Pro en ApiMart (0,05 US$) o KIE (0,09 US$). Texto a imagen · **9:16** · **2K**.
Varias pestañas en paralelo. Producto real → imagen de referencia.
**Guardar como `P1.png`, `P2.png`, `P3.png`…** por número de prompt.

**Clips** — ApiMart → **Kling volumen 3** · 720p · 9:16 · modo **«Future»** → subir **primera y última imagen**
del par → duración **4 s** (3-5) → prompt de estilo del menú de abajo.
Un clip por par consecutivo: `P1→P2`, `P2→P3`, `P3→P4`… **clips = imágenes − 1**.

**Voz** — ElevenLabs. Catálogo → **Multilingual V2**. Voz clonada propia → **V3**.

## Menú de estilos · prompt de clip

Uno solo, el del estilo elegido, para todos los clips. En inglés, tal cual.

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

## Montaje en CapCut

Arrastrar clips + voz. **Colocar el audio primero** y montar contra él.

| Ajuste | Valor |
|---|---|
| Velocidad de todos los clips | **1,20** (1,20-1,30) |
| Transición | **Mix** → aplicar a todas |
| Duración de la transición | **0,5-0,7 s** |
| Música | **−25 a −30** |
| SFX de los propios clips | **−8** |
| Voz | **+5** |

Quitar los silencios largos de la narración. Balancear clip a clip de oído al final.
**No se aplica la capa de realismo**: es del track realista.

## Antes de dar por bueno

- [ ] El Prompt 2 se pegó en NotebookLM, no en ChatGPT.
- [ ] Un solo estilo en el Style Lock del Prompt 6.
- [ ] Todas las imágenes en 9:16 y 2K, nombradas P1…Pn.
- [ ] Cada clip es una transición entre dos imágenes consecutivas, en modo «Future».
- [ ] Todos los prompts de clip terminan en `sound effects (no talking)`.
- [ ] Velocidad 1,20 · Mix 0,5-0,7 · música −25/−30 · SFX −8 · voz +5.
- [ ] El storyboard se iteró al menos una vez.
