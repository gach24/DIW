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