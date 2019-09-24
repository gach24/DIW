# Sección 01: Ejemplo 01
Ejemplo en el que se ven los cambios producidos por el cambio de tamaño en una caja al añadirle paddings y borders sin establecer la propiedad *box-sizing: border-box*
Incialmente la caja tendrá un tamaño de 16rem (tamaño absoluto)
```
div {
    width: 20rem;
    height: 20rem;
    background-color: salmon;
    color: white;
}
```
Si añadimos padding y border la caja tendrá de tamaño los 20 inciales + los 2*2 de padding + 5px+5px de border
```
div {
    width: 20rem;
    height: 20rem;
    background-color: salmon;
    color: white;
    padding: 2rem;
    border: 5px solid blue;
}
```