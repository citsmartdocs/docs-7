Title: Usando Markdown

# Usando Markdown

La documentación de nuestros productos se produce utilizando el patrón de lenguaje Markdown. Markdown es un lenguaje de marcado ligero que puede utilizar para agregar elementos de formato a documentos de texto en texto simple. Creada por John Gruber en 2004, Markdown es ahora uno de los lenguajes de marcado más populares del mundo.

A continuación se incluyen algunas opciones de sintaxis que se pueden utilizar para crear documentos.

## Sintaxis Básica

Estos son los elementos descritos en el documento de diseño original de John Gruber. Todas las aplicaciones de Markdown soportan estos elementos.

| Elemento | Sintaxis Markdown |
|---------|-----------------|
| Título | `# H1` <br/> `## H2` <br/> `### H3` |
| Negrita | `**texto en negrita**`|
|Cursiva	| `*texto en cursiva*` |
|Bloque de citas	| `> bloque de citas` |
|Lista no ordenada |	`1. Primero elemento` <br/> `2. Segundo elemento` <br/> `3. Tercero elemento` |
|Lista no ordenada	| `- Primero elemento` <br/> `- Segundo elemento` <br/> `- Tercero elemento` |
| Código | `código` |
| Regla horizontal | ``---`` |
| Link | `[título](https://www.exemplo.com)`|
| Imagen | `![alt text](image.jpg)` |


### Encabezamiento

Estructurar sus comentarios usando encabezamiento. Los encabezados segmentan comentarios más largos, facilitando la lectura.

Comience una línea con un carácter hash # para definir un encabezado. Organizar sus comentarios con subtítulos, iniciando una línea con caracteres hash adicionales, por ejemplo, ####. Se admiten hasta seis niveles de títulos.

Ejemplo:

```html
# Este es un título H1
## Este es un título H2
### Este es un título H3
```

### Negrita/Cursiva

Ejemplo:

```html
*cursiva*
**negrita**
***negrita-cursiva***^
```

Resultado:

*cursiva*
**negrita**
***negrita-cursiva***^

### Cita

### Lista ordenada

1. Preparar la cocina
2. Preparar ingredientes
3. Cocinar cosas deliciosas

### Lista no ordenada

Ejemplo:

```html
* Leche
* Pan
    * Granos integrales
* Mantequilla
```

Resultado:

* Leche
* Pano
    * Granos integrales
* Mantequilla

### Código

### Línea Horizontal

### Link

### Imagen


## Sintaxis extendida

Estos elementos extienden la sintaxis básica agregando recursos adicionales. Ni todas las aplicaciones de Markdown admiten estos elementos.

