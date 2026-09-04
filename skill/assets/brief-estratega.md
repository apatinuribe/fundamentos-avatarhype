# Plantillas · entrada a los agentes

## El Estratega — guion clip a clip

Basta una frase vaga. No hace falta briefing.

```
{producto en una frase}
→ pregunta por el avatar
{avatar en una frase}
→ fase 2: dolores, deseos, objeciones, ángulos, hooks, mecanismo, nivel de conciencia
→ propone 3 ángulos y pregunta cuáles desarrollar
"elige los tres mejores"
→ fase 3: los anuncios desglosados clip a clip (rótulo · visual · guion)
```

Ejemplo real: `es una app de entrenamiento para mujeres` → `"elige los tres mejores"`.

Para forzar un formato concreto, pedirlo en lugar de delegar: *"quiero hacer un día conmigo"*.

**Verificar siempre** ingredientes, precios y beneficios que escriba: los inventa plausibles.

Salida esperada, estructura fija:
**clip 0 (hook) → problema → agitación → mecanismo → demostración → beneficio → CTA**,
cada clip con **rótulo en pantalla · visual · guion**.

---

## Ads Visual Architect — imágenes estáticas

```
{producto en una frase}
→ devuelve análisis + 7 formatos y pregunta si encaja
"me encaja" + {paleta de colores} + {mercado} + {precio}
→ pide una foto limpia del producto sobre fondo neutro
→ devuelve los prompts, uno por formato
→ "dame más formatos" para ampliar
```

**Antes de generar: sustituir el marcador `marca` por el nombre real.**
Si no se indica mercado, **asume España**.

Formatos que devuelve: testimonio · antes/después · características · ticket comparativo · foro · búsqueda ·
progresión temporal · comparación · podcast de Spotify. Funciona igual con producto físico que con un servicio
sin nada que fotografiar.

---

## Agente 6C — prompts de imagen

Adjuntar la referencia real. El agente pregunta *"¿igual o con cambios?"* y devuelve el prompt en inglés en un
único bloque de código. **Nunca genera imágenes**: solo prompts.

Iterar sobre el texto del prompt (que sea rubia, otra ropa) **antes** de gastar una generación.

Vía sin agente: usar el prompt de la biblioteca *"cambiar el avatar en base a una descripción"* y rellenar,
p. ej. `caucásica, rubia, ojos azules, una chica natural, imperfecta, real`.

---

## Instalar las skills en Claude

`+ → Skills → Manage skills → Añadir → Subir skill`, subiendo el `.md`.
Para usarla en una conversación: `+ → Skills → seleccionarla`.
