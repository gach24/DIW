# Valores de justify-content

- justify-content: flex-start
Reparte los items elementos del contenedor al inicio del mismo, es el valor por defecto

```scss
.flex-container {
    ...
    display: flex;
    justify-content: flex-start; // Por defecto
}
```

![01-state](./img/justify-content/01-state.png)

- justify-content: flex-end
Reparte los items elementos del contenedor al final del mismo

```scss
.flex-container {
    ...
    display: flex;
    justify-content: flex-end;
}
```

![02-state](./img/justify-content/02-state.png)

- justify-content: center
Reparte los items elementos del contenedor en su centro

```scss
.flex-container {
    ...
    display: flex;
    justify-content: center;
}
```

![03-state](./img/justify-content/03-state.png)

- justify-content: space-between
Reparte el espacio entre los diferentes elementos del contenedor hasta los límites

```scss
.flex-container {
    ...
    display: flex;
    justify-content: space-between;
}
```

![04-state](./img/justify-content/04-state.png)

- justify-content: space-around
Reparte el espacio entre los diferentes elementos del contenedor

```scss
.flex-container {
    ...
    display: flex;
    justify-content: space-around;
}
```

![05-state](./img/justify-content/05-state.png)
