# Ejemplo: Unidad de medida FR (Fraction Unit)

Inicialmente, en el archivo html se crean 12 cajas como elementos de bloque. La primera sección del archivo .scss solo modifica las características estéticas de las cajas.

```html
    <div class="grid">
        <div class="grid-item item1">1</div>
        <div class="grid-item item2">2</div>
        ...
    </div>
```

```scss
body {
    font: 3em sans-serif;
    ...
}

.grid {
    padding: 1rem;
}
...
```

En esta ocasión creamos tres columnas con la unidad de medida **fr** que lo que a decir es que se repartan el espacio disponible

```scss
.grid {
    display: grid;
    grid-column-gap: 1rem;
    grid-row-gap: .5rem;
    grid-template-columns: 1fr 1fr 1fr;
}
```

![01-state](./doc/img/01-state.png)
