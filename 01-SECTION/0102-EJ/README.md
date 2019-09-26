# Sección 01. Ejemplo 02
Ejemplo sin border-box y con border-box de cuatro cajas en línea horizontal
## PASO 1
En el ejemplo se distribuyen cuatro cajas alineadas horizontalmente, cada una de ellas ocupa el 25% del ancho de la página, sin embargo como cada una de las cajas tiene un borde (pasaría lo mismo si tuvieran algún padding) y la propiedad *box-sizing* no está establecida a *border-box* las cuatro cajas no caben dentro de ancho de la página, desplazando a la situada más a la derecha a la siguiente línea
```
.box {
    box-sizing: border-box;
    width: 25%;
    height: 20rem;
    float: left;
    padding: 2rem;
    border: 1px solid black;
    ...
}
```
## PASO 2
Se establece *box-sizing: border-box* a la clase box del div. De esta manera el borde y el padding pasan a formar parte del ancho total de la caja, y los cuatro div caben en una sola línea
```
.box {
    box-sizing: border-box; /* Añadida */
    width: 25%;
    height: 20rem;
    float: left;
    padding: 2rem;
    border: 1px solid black;
    ...
}
```
## PASO 3
Como complemento al paso anterior se establece la propiedad *box-sizing: border-box* a todos los elementos del html incluidos también pseudoelementos.
La notación **:before, *:after* es para navegadores antiguos
```
*, *::before, *::after, *:before, *:after {
    box-sizing: border-box;
}
```