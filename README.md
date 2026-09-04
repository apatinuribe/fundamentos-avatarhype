# Fundamentos AvatarHype

Método completo de producción de anuncios para ecommerce con IA, destilado de los dos cursos de la academia
AvatarHype (28 lecciones) a un formato consumible por una máquina.

Repo **privado y de solo lectura**: aquí no se trabaja, se consume. La fuente de verdad es el pipeline local
(`knowledge-to-skill`), que genera estos archivos; cualquier corrección se hace allí y se vuelve a publicar
aquí. Editar un archivo de este repo se pierde en la siguiente publicación.

---

## Qué archivo usar según la herramienta

| Quieres | Usa | Por qué |
|---|---|---|
| Pegar el método en otro software de creación de contenido (system prompt, agente, GPT personalizado) | **[`system-prompt.md`](system-prompt.md)** | Escrito como instrucciones para un modelo, no como documentación. Se pega entero |
| Leerlo tú, de principio a fin | **[`manual-avatarhype.md`](manual-avatarhype.md)** | Los cuatro documentos en uno, con índice. 159 KB |
| Que Claude conteste consultando la parte que toque | **[`knowledge/`](knowledge/)** | Cuatro documentos separados: se carga solo el que hace falta |
| Prompts sueltos ya escritos, para copiar y pegar | **[`biblioteca/prompts-biblioteca.md`](biblioteca/prompts-biblioteca.md)** | 86 prompts literales de la biblioteca del curso |
| Instalarlo como skill de Claude Code | **[`skill/`](skill/)** | `SKILL.md` + plantillas |

---

## Los dos tracks

El método no es uno, son dos, y **no se mezclan**. Decidirlo es el primer paso de cualquier encargo.

| Track | Cuándo | Cadena |
|---|---|---|
| **Realista** — persona a cámara | UGC, testimonio, demo de producto en mano, moda, podcast, app/SaaS | Ángulo → guion → imagen de referencia → Omni o Grok → limpieza → capa de realismo en CapCut |
| **Animado** — sin persona real | Estilo Pixar, claymation, Wes Anderson, sci-fi o Apple; producto difícil de enseñar con alguien real | 8 prompts encadenados en ChatGPT + NotebookLM → Nano Banana Pro → Kling 3 (primer + último frame) → ElevenLabs → CapCut |

Lo que comparten: el resultado se decide en la planificación (≈80 %), todo en 9:16 y 2K, voz de ElevenLabs,
montaje en CapCut con transiciones **Mix** y nada más, y el modelo de vídeo nunca mete voz por su cuenta.

---

## Estructura

```
system-prompt.md          instrucciones listas para pegar en otro sistema (cubre los dos tracks)
manual-avatarhype.md      el manual completo, con índice — los cuatro documentos en uno

knowledge/
  proceso.md              el pipeline paso a paso, fase a fase, en los dos tracks
  practicas.md            reglas duras, criterios de decisión y errores caros
  prompts.md              todos los prompts literales del curso, en inglés donde el curso los da así
  ejemplos.md             casos completos con sus cifras y sus guiones

biblioteca/
  prompts-biblioteca.md   los 86 prompts sueltos de la Biblioteca de prompts (lección 1.4.1)
  indice-medios.md        qué imagen o vídeo de ejemplo ilustra cada prompt (90 asociaciones)

skill/
  SKILL.md                la skill de Claude Code, por etapas
  assets/                 plantillas rellenables: prompt de imagen, prompt de clip, brief, checklists
                          y direccion-clip.md, la única marcada [ANEXO] (no sale del curso)
```

## Trazabilidad

Cada afirmación de `knowledge/` cita su lección de origen entre corchetes: `[M4-L4.1.1]` es módulo 4,
lección 4.1.1. `[M6-L6.1]` y `[M6-L6.2]` son el curso de animados. Si algo no lleva cita, no sale del curso.

Hay **una sola excepción deliberada**, y va marcada `[ANEXO]` en su propio título: la capa de **dirección**
entre el guion y la imagen — `Fase 2.5` de `knowledge/proceso.md`, el anexo final de `knowledge/practicas.md`,
la § 3.5 de `system-prompt.md` y `skill/assets/direccion-clip.md`. El curso pasa del guion directo a la imagen
y deja lo visual "negociable"; esa capa cierra la costura (continuidad entre clips, qué voz se puede dirigir,
qué se decide antes de escribir un prompt). **No sale del curso, no lleva citas y si contradice algo citado con
`[M…]`, manda lo citado.**

## Lo que no está aquí, a propósito

- **Los archivos de ejemplo de la biblioteca** (53 medios, 88 MB). `biblioteca/indice-medios.md` dice qué
  archivo ilustra cada prompt y cómo recuperarlos, pero los binarios no se versionan: no se renderizan desde
  un repo privado y multiplicarían por 180 el peso del repo.
- **Las transcripciones y el material en bruto** de las 28 lecciones. Viven en el pipeline local.
- **Los 392 audios** de la Biblioteca de audio del curso.

## Vigencia

Consolidado el **2026-09-03**. El curso de Ads Animados se está regrabando entero según su propia lección de
bienvenida, así que el track animado es una foto que va a cambiar. El único dato transcrito de oído y sin
verificar contra la interfaz es el nombre del selector «Future» de Kling en ApiMart.
