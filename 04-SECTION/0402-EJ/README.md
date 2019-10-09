# Ejemplos de menus justificados con border-collapse, border-spacing y centrado
## MENU 1
Idéntico al ejercicio anterior [0401-EJ](../0401-EJ/)

## MENU 2
En el ejemplo se muestra como los border solapar los border de dos celdas colindanates mediante **border-collapse: collapse**, por defecto ambos bordes colindates se dibujan uno al lado del otro dando la sensación de un borde con doble grosor, con esta propiedad ambos bordes se collapsan mustrando un único borde del grosor adecuado
```
    nav {
        background-color: deepskyblue;
        ...
        
        ul {
            display: table; // Creación de las tablas
            table-layout: fixed; // Para evitar que el tamaño de la celda sea en función del contenido 
            border-collapse: collapse;
            ...
            li {
                display: table-cell; // Creación de las celdas
                border: 2px solid white;
                ...
          
            }
        }
    }
```

Además se utiliza la propiedad **border-spacing: .5em 1em;** para establecer la separación entre bordes izquierda/derecha y arriba/abajo respectivamente, cuidado con esto porque el borde es al contrario que otras propiedades CSS
```
    nav {
        ...
        
        ul {
            display: table; // Creación de las tablas
            table-layout: fixed; // Para evitar que el tamaño de la celda sea en función del contenido 
            border-spacing: .5em 1em; // Cuidado aquí la primera medida es izquierda y derecha y la                                  última arriba y abajo
            ...
            li {
                display: table-cell; // Creación de las celdas
                border: 2px solid white;
                border-radius: .5em; // Junto con border-spacing
                ...
          
            }
        }
    }
```

## MENU 3
En el tercer menú se establece el ancho de las celdas a un ancho determinado (15rem), con el ancho de la tabla a auto **width: auto** de forma que la tabla no ocupa el ancho de toda la página, y a continuación se centra mediante **margin: 0 auto** 
```
.nav {
    background-color: transparent; 
    ...
    ul {
        width: auto; // Calcula el ancho en función del tamaño de las celdas
        margin: 0 auto; // Centrado de la tabla
    }

    li {
        border: 1px solid deepskyblue;
        width: 15rem; // Ancho fijo
    }

}
```


