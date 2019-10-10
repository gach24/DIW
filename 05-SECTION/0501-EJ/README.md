# Elementos inline junto a elementos float
Como vemos en el ejemplo tenemos una imagen y dos span (elementos en línea) al establecer en la imagen que flote a la derecha **float: rigth** la imagen se desplaza a la parte derecha y el resto de elementos **inline** se situan en el espacio restante, respetando el espacio del elemento/s flotados

```
span {
    background-color: deepskyblue;
}

img {
    float: right;
}
```
