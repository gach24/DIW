# Técnicas para evitar que un contenedor pierda su altura
En el ejemplo se analizan las dos técnicas principales para evitar que un contenedor su altura cuando todos sus hijos son elementos flotantess
## Mediante la propiedad **overflow: hidden**
Estableciendo esta propiedad al contenedor se evita que pierda la altura

```css
    ul {
        ...
        overflow: hidden;

        li {
            float: left; 
            ...
            a {
                ...
            }
        }
    }
```

## Mediante pseudoelementos
La otra técnica es mediante un psudoelemento que añada un elementos de bloque con la propiedad **clear: both** establecida para que rompa el flujo de floats. En el contenedor ya no todos sus elementos son flotantes por lo que recupera su altura
```css
    ul {
        ...
        &::after {
            content: '';
            display: block;
            clear: both;           
        }

        li {
            float: left; 
            ...
            a {
                ...
            }
        }
    }
```