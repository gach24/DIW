# Elementos en línea y en bloque
## Elementos en línea
- Ocupan el espacio necesario para mostrar su contenido
- No tienen dimensiones modificables (alto, ancho)
- Permiten otros elementos a su lado
- Padding y margin solo empujan a elementos adyacentes en horizontal, nunca en vertical

## Elementos en bloque
- Ocupan todo el ancho disponible 
- Tienen dimensiones modificables (alto y ancho)
- No permiten otros elementos a su lado (aunque especique un ancho, sigue ocupando todo el espacio disponible)

## Elementos inline-block
- Mezcla de inline y block
- Tienen dimensiones modificables (alto, ancho)
- Permiten otros elementos a su lado. Si no especifico dimensiones, ocupa lo que ocupe su contendido
### Consideraciones sobre los elementos inline-block
- **vertical-align** alinea elementos entre ellos (no su contenido dentro)
- Espacios no deseables entre elementos y en imagenes dentro de contenedores. [Ver enlace](https://davidwalsh.name/remove-whitespace-inline-block)

Ejemplos:
1. [0301-EJ](./0301-EJ). Ejemplo de elementos con propiedad **display: inline**
2. [0302-EJ](./0302-EJ). Ejemplo de elementos con propiedad **display: block**
3. [0303-EJ](./0303-EJ). Ejemplo de elementos con propiedad **display: inline-block**
4. [0304-EJ](./0304-EJ). Soluciones al espacio en blanco entre elementos inline-block
5. [0305-EJ](./0305-EJ). Soluciones al espacio en blanco debajo de las imágenes
6. [0306-EJ](./0306-EJ). Ejemplo de elementos con propiedad **display: table**. Menus justificados
