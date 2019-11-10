# Ejemplo de cambio en el tamaño de los items
En el ejemplo tenemos incialmente un contenedor de ancho fijo 800px, y cuatro items dentro del contenedor de 200px cada uno.

```scss
.flex-container {
    background-color: salmon;
    width: 800px;
    height: 400px;
    display: flex;
    align-items: flex-start;
}

.flex-item {
    font-size: 5em;
    color: white;
    background-color: deepskyblue;
    border: 1px solid;
    width: 200px;
}
```

Si redimensionamos el ancho de la ventana del navegador, el tamaño de la caja no varía, llagando a ocultarse parte del contenedor

![01-state](./doc/img/01-state.gif)

## STEP 01
En el primer paso si modificamos el ancho del contenedor de **width: 800px** fijo a una medida más flexible **max-width: 800px**, podemos observar que el ancho del contenedor se reduce, como era de esperar.

```scss
.flex-container {
    ...
    max-width: 800px;
    ...
}
```

Sin embargo lo que no era de esperar es que el ancho de los items tembién se reduzca, aunque tengan un ancho fijo **width: 200px**
Por lo tanto, con flexbox podemos observar que el tamaño de los items del contenedor puede reducirse si es necesario

![02-state](./doc/img/02-state.gif)
