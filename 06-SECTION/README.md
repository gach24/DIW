# Ejemplos de posicionamiento
La propiedad position, junto con la propiedad float (vista anteriormente), permite modificar la posición de cualquier elemento de la página
El navegador, por defecto, coloca los elementos teniendo en cuenta el orden en el que aparecen en el html y si es un elemento en linea o en bloque. 
Con **position** puedo modificar este comportamiento
## Valores de position
### Static
Valor por defecto. Se ignoran las propiedades top, bottom, left, right y z-index
Un elemento con la **position: static** esta tal cual establece el flujo normal del html
### Relative
Posicionamiento de la caja respecto a su posición original, es decir, donde se encuentra el elemento en su posición original si no le establezco ningun position. 
En el momento que yo le de coordenadas voy a mover ese elemento a partir de ese punto.
Además:
1. El resto de elementos de la página respetan su posición original pero ignoran la nueva posición, como consecuencia podemos tener solapamientos.
2. Top, bottom, left y right desplazan el elemento de su posición inicial
3. Sirve de "referencia" para hijos posicionados de forma absoluta

### Absolute
Posiciona el elemento en la coordenada (0, 0) del primer ancestro que tenga establecida la propiedad **position** diferente de **static.**
Además:
1. El elemento se posiciona fuera del flujo normal, el resto de elementos no respetan su posición original, es decir, se mueven y el espacio que dejan es ocupado por el resto de elementos, con lo que también podemos tener posibles solapamientos
2. Top, right, bottom y left colocan la caja en la coordenada (0, 0) respecto del primer ancestro con la propiedad **position** establecida pero distinta de **static** 
3. Cuidado con el ancho, ocupa lo que ocupe su contenido, si tengo un elemento vacío me quedo sin ancho
4. Si no tengo ningún ancestro con **position** distinto de **static**, el elemento se coloca en la coordenada (0,0) del html

### Fixed
Posicionamiento de la caja respecto de la coordenada (0, 0) de la ventana
Además:
1. Fuera del flujo normal, es decir, el resto de elementos no respetan la posición original del elemento. Posibles solapamientos
2. Ni el body ni el html son la ventana, por eso el elemento posicionado con fixed no se menea aunque haga scroll
