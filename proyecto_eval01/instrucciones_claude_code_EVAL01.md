# Tarea para Claude Code: EVAL01 Desarrollo Web 1 (Markdown)

## Contexto

Necesito entregar una evaluación (10 %) de Desarrollo Web 1 sobre el lenguaje de marcado **Markdown**. Tu trabajo es **crear los archivos `.md` y los recursos que necesita el proyecto**. Yo me encargo después de copiar el código y la vista previa al `.docx` de entrega.

Fecha de entrega: **10 de octubre de 2026**.

## Reglas del profesor (obligatorias)

1. El documento Markdown debe usar **al menos un ejemplo de cada uno de los elementos de Markdown** (lista completa en el Paso 3).
2. El **tema** del documento debe ser uno de los que aparecen en estos dos PDF:
   - https://www.eonicasys.com.co/2026-02/Bibliografia/Atlas/ATLAS_info.pdf
   - https://www.eonicasys.com.co/2026-02/Bibliografia/Atlas/ATLAS_math.pdf
3. Se puede complementar el texto y cambiar las imágenes.
4. La vista previa se toma con **Visual Studio Code**, así que todo debe verse bien en la vista previa de VS Code.

---

## Paso 1: Crear la carpeta del proyecto

Crea esta estructura:

```text
proyecto_eval01/
├── eval01.md        (documento principal)
├── help.md          (archivo enlazado como enlace interno)
└── imagen.png       (imagen usada en el documento principal)
```

## Paso 2: Elegir el tema

- Si en la carpeta hay `ATLAS_info.pdf` o `ATLAS_math.pdf`, léelos y elige **un tema** de uno de ellos.
- Si no puedes leerlos, pregúntame qué tema usar antes de seguir.
- El tema elegido será: `TEMA: ________________` (rellenar o dejar que Claude Code lo proponga y me pida confirmación).
- Con ese tema escribe contenido real en español (definición, ejemplos, historia, etc.), no texto de relleno.

## Paso 3: Crear `eval01.md` con los 16 elementos

El documento debe tener **un ejemplo de cada elemento**, todo relacionado con el tema elegido. Sigue esta sintaxis exacta (viene del PDF del profesor):

| # | Elemento | Sintaxis que se debe usar |
|---|----------|---------------------------|
| 1 | Encabezados | `# H1` hasta `###### H6` (siempre con espacio después de `#`) |
| 2 | Negrita | `**texto**` |
| 3 | Itálica | `*texto*` |
| 4 | Tachado | `~~texto~~` |
| 5 | Código en línea | `` `texto` `` |
| 6 | Enlace externo | `[texto](https://www.eonicasys.com.co/2026-02/DesarrolloWeb1)` y también una URL suelta |
| 7 | Cita anidada | `> cita` y `>> cita anidada` |
| 8 | Lista con viñetas | `- item` o `* item`, con un subitem anidado (línea en blanco previa e indentación) |
| 9 | Lista numerada | `1. Item1`, `2. Item2`, `3. Item3`, con subitems anidados |
| 10 | Lista de tareas | `- [ ] por hacer` y `- [x] hecho` |
| 11 | Línea horizontal | `---`, `***` y `___` (cada una sola en su línea, con línea en blanco antes) |
| 12 | Tabla | `\| col1 \| col2 \|` con la fila `\|---\|---\|`, **máximo 5 columnas** |
| 13 | Bloque de código | ` ```python ` ... ` ``` ` (con un lenguaje, por ejemplo Python o C++) |
| 14 | Fórmula matemática | ` ```math ` ... ` ``` ` con una expresión válida, por ejemplo `(x^2+1)^3` |
| 15 | Imagen | `![texto alternativo](imagen.png)` |
| 16 | Enlace interno | `[Abrir archivo ayuda](help.md)` |

Además, incluye (el profesor los explica en el PDF y suman calidad):

- Un **comentario** HTML: `<!-- comentario que no se ve en la vista previa -->`
- Un **párrafo** normal y otro **párrafo enmarcado** (indentado con 4 espacios)
- Un ejemplo de **caracteres de escape**, por ejemplo `\*` y `\#`

### Cuidados para que se vea bien en VS Code

- Deja **una línea en blanco** antes y después de listas, tablas, bloques de código y líneas horizontales.
- Un solo `-` debajo de un texto lo convierte en título, así que usa siempre `---` para líneas.
- Cierra todos los bloques de código con ` ``` ` en su propia línea.
- Los caracteres `|` dentro de una tabla se escapan como `\|`.
- Guarda en **UTF-8** (hay tildes y eñes).

## Paso 4: Crear `help.md`

Un archivo corto que sirva de destino del enlace interno:

```markdown
# Ayuda del documento

> Este archivo se abre desde el enlace interno de eval01.md.
```

Puedes agregar 2 o 3 líneas explicando cómo se usa el documento principal.

## Paso 5: Crear la imagen `imagen.png`

- Debe estar en la misma carpeta que `eval01.md`.
- Debe ser **relevante al tema elegido** (diagrama, gráfico, esquema).
- Créala con Python (Pillow o matplotlib) o descárgala si el tema lo permite.
- Formato `.png` o `.jpeg`, tamaño moderado (menor de 500 KB).

## Paso 6: Verificar antes de terminar

Revisa y confirma explícitamente:

- [ ] Están los **16 elementos** de la tabla del Paso 3 en `eval01.md`.
- [ ] `help.md` e `imagen.png` existen y las rutas del documento coinciden con los nombres de archivo.
- [ ] Todos los bloques de código están cerrados.
- [ ] La tabla no pasa de 5 columnas.
- [ ] El contenido corresponde al tema elegido de los ATLAS.
- [ ] Puedes mostrarme los archivos finales (`eval01.md` completo y `help.md`).

Cuando termines, dame un resumen de los archivos creados y el tema elegido. **No** modifiques nada fuera de la carpeta `proyecto_eval01/`.

---

## Pasos que hago yo (fuera de Claude Code)

1. Abrir `proyecto_eval01/` en **Visual Studio Code**.
2. Abrir la vista previa lateral con `Ctrl+K V` sobre `eval01.md`.
3. Descargar el `DES_WEB1_EVAL01.docx` y llenar el encabezado (nombres, cédula, # de lista, firma, grupo, semestre).
4. En la tabla **"Markdown Source Code1"**, poner el nombre del archivo y pegar el código de `eval01.md` **copiado desde VS Code** (con colores, no como captura).
5. En **"Markdown Source Code2"**, hacer lo mismo con `help.md`.
6. En **"Vista previa"**, pegar la vista previa renderizada de VS Code.
7. Guardar como **`.docx`** (no PDF) y enviarlo desde el **correo institucional** a `jameza@unal.edu.co` con el asunto **`EVAL01_DES-WEB1`**.
