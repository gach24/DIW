# Ejercicio sobre menu justificado mediante display: table y display: table-cell
En el ejercicio se crea un menu con las siguientes entradas:
```
    <nav>
        <ul>
            <li><a href="#">Disciplinas</a></li>
            <li><a href="#">Actualidad</a></li>
            <li><a href="#">Entrenamientos</a></li>
            <li><a href="#">Materiales</a></li>
            <li><a href="#">Salud y Nutrición </a></li>
            <li><a href="#">Contacto</a></li>
        </ul>
    </nav>
    <main>
    </main>
```
Además se añade justo debajo una caja (etiqueta main) de altura fija (10rem) y color gris
```
    main {
        height: 10rem;
        background-color: silver;
    }
```
El menu utiliza las propiedades display: table en la lista y display: table-cell en los elementos de la lista para mostrar la lista en forma de menú
```
nav {
    ...
    ul {
        display: table;
        table-layout: fixed;
        ...
    }

    li {
        display: table-cell;
        ...
    }

    a { 
        ...
    }
}

```

Para hacer un subrayado sobre los elementos del menu cuando el usuario pasa el ratón por encima, se utiliza un borde amarillo en el selector hover
```
    a { 
        padding: 1em 1em;
        &:hover {
            
            border-bottom: 4px solid #FFCC00;  
        }
    }
```
Este borde amarillo se aplica sobre el enlace no sobre los elementos de la lista (<li>) y para aumentar el tamaño del enlace se utiliza un padding, sin embargo el enlace tiene naturaleza inline, por lo que para que el padding sea tenido en cuenta se cambia su naturaliza a **display: inline-block**
Se utiliza **inline-block** y no **block** porque pretendemos que el borde inferior no ocupe todo el espacio de la celda, simplemente que sobresalga un poco

Por último, cuando pasamos el ratón sobre el enlace aparece el borde inferior, pero esto hace la caja inferior se despace hacia abajo, para evitar este efecto establecemos el borde previamente con un color transparente y añadimos una transición para que el cambio sea menos brusco
```
    a { 
        padding: 1em 1em;
        display: inline-block;
        border-bottom: 4px solid transparent; // Para el desplazamiento de la caja inferior
        transition: border-bottom 1s linear;
        &:hover {
            border-bottom: 4px solid #FFCC00;  
        }
    }
```




