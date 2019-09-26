# Sección 01. Ejemplo 03
Se distribuyen cuatro "div/cajas" con margen, horizontalmente sobre la página, el ancho de cada página es de 22% por lo que queda disponible para el espacio entre cajas un 12%
## Versión 1.0
Se añaden cuatro margenes derechos (margin-right) de un 3%, sin embargo los "div/cajas" no quedan correctamente distribuidos
```
.box {
    width: 22%;
    ...
    border: 10px solid blue;
    margin-right: 3%; 
}
```

## Version 2.0 
Se añade a cada "div/caja" un margen del 4% y despues se anula el del "div/caja" situado más a la derecha
```
.box {
    width: 22%;
    ...
    border: 10px solid blue;
    margin-right: 4%; 
}

.box:last-child {
    margin-right: 0; 
}
```

## Versión 3.0
Se añade a todos los "div/caja" que no sean el situado más a la derecha (el último) un márgen del 4%
```
.box {
    width: 22%;
    ...
}

.box:not(:last-child) {
    margin-right: 4%; 
}

```