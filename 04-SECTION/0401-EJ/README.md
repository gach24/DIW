# Ejemplo de menu justificado mediante display: table
El el ejemplo se muestra un menu de manera justificada mediante las propiedades **display: table** y **display: table-cell**

La propiedad **table-layout: fixed;** del ejemplo permite igualar el tamaño de todas las celdas, lo cual es mucho más rápido ya que por defecto **table-layout: auto** el tamaño de las celdas es calculado en función del contenido de cada una ellas, es decir, dejando la propiedad con el valor por defecto el tamaño de las celdas se distribuirá dependiendo del contenido
```
    nav {
        background-color: deepskyblue;
        ...
        
        ul {
            display: table; // Creación de las tablas
            width: 100%;
            table-layout: fixed; // Para evitar que el tamaño de la celda sea en función del contenido 
            li {
                display: table-cell; // Creación de las celdas
                ...
                
                /** Resulta que los enlaces son muy poco accesibles **/
                a {
                    padding: 1em;
                    display: block;
                }            
            }
        }
    }
```

En el ejemplo también se puede ver que para mejorar las accesibilidad de los enlaces se les añade un padding y se les quita su naturaleza **inline** para que el padding superior e inferior sea efectivo.