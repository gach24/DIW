# Problema de los espacios en blanco en elementos inline-block
En el ejemplo se puede ver cuatro div con el 25% de ancho cada uno, al establecer la propiedad **display: inline-block** se ven en horizontal sin embargo no caben en el ancho de la página debido a que aparece un pequeño espacio en blanco  
Este espacio es propio de la naturaleza inline de los elementos **inline-block**, es decir, en los elementos **inline** los saltos de línea tabuladores, etc. el navegador los interpreta como espacios en blanco y esto es aplicado también a los elementos **inline-block**  
En el elemplo también se puede ver (al final del html) un elemento span (de naturaleza inline) con un salto de línea que el navegador interpreta como un espacio en blanco, ese espacio en blanco es el que se ve entre los diferentes **elementos inline-block**

Posibles soluciones: 
- Eliminar el salto de línea entre los elementos inline-block (poco elegante)
- Establecer el font-size a 0 del padre y volver a restablecerlo en los hijos (más elegante)
- Comentarios (poco elegante)
- Margen negativo

Más información pincha [aquí](https://davidwalsh.name/remove-whitespace-inline-block)


