# Ejemplo de disposición en columnas mediante diferentes métodos
## Ejemplo mediante **display: inline-block**
En este ejemplo se disponen cuatro columnas en horizontal una al lado de la otra, utilizando **display: block**. Las columnas miden un 22% del ancho de su contenedor y además existe un margen entre columnas de un 4%, en total un 100% (4*22%+3*4%), sin embargo, las columnas no caben en el ancho de su contenedor debido al espacio en blanco de los elementos inline-block.
Para solucionar el problema se pone el tamaño de fuente en el contenedor a 0 (**font-size: 0**-) y luego se restablece en sus hijos
```
#columns-inline-block {
    font-size: 0; // font-size a 0 para que me quepan los 4 articles
    article {
        display: inline-block;
        width: 22%; 
        vertical-align: top; // Alineación entre elementos inline-block
        height: 30rem; // Todos los articles con la misma altura
        font-size: 1rem; // Restablezco el font-size para que se vean los articles
        &:not(:last-child) {
            margin-right: 4%; // Margin solo a los primeros tres articles
        }
    }
}
```

## Ejemplo mediante float
En este ejemplo se disponen también cuatro columnas con las mismas características, en ese caso flotando todas ellas a la izquierda (**float: left**), no es necesario en este caso establecer el **font-size: 0** ya que las columnas son elementos de bloque, que no generan ningún espacio en blanco, y mediante la propiedad **float** es pesible que los elementos se dispongan unos al lado de otros
Sin embargo, el contenedor pierde su altura haciendose invisible o viendo una pequeña parte en este caso ya que tiene un **padding**, para evitar esto se establece la propiedad **overflow: hidden**
```
#columns-float {
    overflow: hidden; // Soluciona el problema cuando el padre pierde su altura cuando 
    article {
        float: left;
        width: 22%;
        height: 30rem;
        &:not(:last-child) {
            margin-right: 4%;
        }       
    } 
}
```

## Ejemplo mediante **display: table** y **display: table-cell**
En el último ejemplo se disponen también cuatro columnas con las mismas características, en este caso aplicado las propiedades **display: table** y **display: table-cell** a cada una de sus columnas hijas.
Notar que en este caso las columnas son de igual altura sin establecersela explicitamente y además son completamente responsive, si reducimos el ancho de la ventana del navegador las columnas se hacen mas delgadas y su altura crece, no desbordando su contenido
```
#columns-table {
    display: table;
    table-layout: fixed;
    border-spacing: 2rem 0;
    article {
        display: table-cell;
        width: 25%;
    }      
}
```

