# Propiedad flex-shrink

En el ejemplo incialmente partimos de un contenedor flex de 900px

```scss
.flex-container {
    background-color: salmon;
    display: flex;
    max-width: 900px;
    padding: 1rem;
    margin-bottom: 3rem;
}
```

El contenedor flex contiene 20 items, a los que no se les establece ningún tipo de ancho (ni flex-basis ni width)

```html
    <div class="flex-container stepone">
        ...
        <div class="flex-item">20</div>
    </div>
```

```scss
.flex-item {
    font-size: 5em;
    color: white;
    background-color: deepskyblue;
    border: 1px solid;
}
```

Como se puede apreciar en la imagen los items se reducen al mínimo pero respetando su contenido, aunque el número de items sea demasiado grande y termine desbordando al contenedor

![01-state](./doc/img/01-state.png)

## STEP 01

En el paso 01 establecemos un ancho a los items de 100px

```scss
.flex-item {
    ...
    flex-basis: 100px;
    ...
}
```

Sin embargo, no sucede nada ya que los items encogen todo lo que pueden porque no caben en el contenedor, es decir, los items ya son lo más pequeño posible y no hace caso al flex-basis: 100px

## STEP 02

En el paso 02 se crea otro contenedor flex esta vez con solamente 9 items, de 80px de ancho

```html
    <div class="flex-container stepone">
        ...
        <div class="flex-item">9</div>
    </div>
```

```scss
.flex-item {
    flex-basis: 80px;
}
```

Como se ve en la imagen, los elementos caben en el contenedor y no es necesario que se encojan.
![02-state](./doc/img/02-state.png)

Si cambio el flex-basis a 100px los elementos no caben en el contenedor pero se encogen hasta caber

```scss
.flex-item {
    flex-basis: 80px;
}
```

![03-state](./doc/img/03-state.png)

La unica manera de que me respete el ancho aunque suponga un desbordameinto es mediante min-width

```scss
.flex-item {
    min-width: 100px;
}
```

![04-state](./doc/img/04-state.png)
