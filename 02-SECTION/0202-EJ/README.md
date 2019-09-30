# Sección 02. Ejemplo 02: Ejemplo de Sass tratamiento de ficheros
## Comentarios
Los comentarios pueden ser de una sola línea // o como en css /* */
Naturalmente los comentarios de una sola línea en el fichero .scss desaparacerán en el fichero traducido a css
´´´
/**
 Comentario varias líneas
 */
// Comentario una sola línea
blockquote {
    margin: 0 0 20px 0;
    
    p {
        margin: 0;
    }
}
´´´

## Ficheros sourcemap
Estos ficheros enlazan en el depurador el css con el fichero .scss origen
El compilador genera ficheros sourcemap (.map) por defecto, es posible evitarlo mediante otras opciones
```
$ sass --sourcemap=auto scss/style.scss:css/style.css (opción por defecto)
$ sass --sourcemap=inline scss/style.scss:css/style.css (en el propio css)
$ sass --sourcemap=none scss/style.scss:css/style.css (no genera sourcemap)

## @import
La directiva @import permite realizar una referencia a un archivo externo, es como añadir una nueva etiqueta <link> a un archivo html
Admite diferentes formatos:
- @import '/archivo.css';
- @import url() screen and (min-width: 860px);
- @import '_variables.scss' (realiza un copy y paste del archivo en el lugar donde hicimos el import). Adicionalmente las variables, mixins, funciones, etc. Importados quedarán disponibles a continuación y el @imports posteriores

Utilizando el _ le indicamos a Sass que no compile esos archivos, ya que serán importados en el archivo principal/es que si serán procesados.

Podemos realizar los imports de esta manera:
```
@import variables
@import layout
```

La división en varios ficheros, permite tener el código divido en partes más fáciles de mantener