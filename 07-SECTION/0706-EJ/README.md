# Centrado vertical y horizontal cuando el alto y ancho es conocido

En el ejemplo se muestra una caja principal ".wrapper" centrada horizontalmente, esta caja contiene a su vez otra **caja ".box" de altura y anchura 10rem**, el objetivo del ejemplo es centrarla horizontal y verticalmente.

![01-state](./doc/img/01-state.png)

```scss
.wrapper {
    width: 80%;
    background-color: rgba(0,0,0,.2);
    height: 30rem;
    margin: 3rem auto;
}

.box {
    height: 10rem;
    width: 10rem;
    background-color: salmon;
}
```

Para ello, se establece la propiedad position: absolute y se centra mediante **top: 50%** y **left: 50%**, teniendo en cuenta que la posición **top y left al 50%** es respecto al primer ancestro con **position establecido**, es decir, si no indicamos lo contrario el **top y left** lo realizará respecto del **html**, por lo que es necesario establecer **position: relative** al elemento ".wrapper" para que lo centre respecto de esta caja

```scss
.wrapper {
    ...
    position: relative;
}

.box {
    ...
    position: absolute;
    left: 50%;
    top: 50%;
}
```

![02-state](./doc/img/02-state.png)

Sin embargo, como se muestra en la imagen, la caja ".box" no aparece centrada respecto a la caja ".wrapper" es necesario desplazarla a la izquierda y hacia arriba la mitad de sus dimensiones, para ello podemos utilizar márgenes negativos por la mitad de sus dimensiones
Como estas dimensiones son conocidas serán -5rem hacia la izquierda y hacia arriba

```scss
.wrapper {
    ...
    position: relative;
}

.box {
    position: absolute;
    left: 50%;
    top: 50%;
    margin-top: -5rem;
    margin-left: -5rem;
}
```

![03-state](./doc/img/03-state.png)
