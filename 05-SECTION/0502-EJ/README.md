# Elementos en bloque junto a elementos float
Como vemos en el ejemplo tenemos una imagen y dos párrafos (elementos en bloque) al establecer en la imagen que flote a la derecha **float: right** la imagen se desplaza a la parte derecha y aparentemente los elementos en bloque ocupan el espacio restante (como en el caso de los elementos en línea), sin embargo, esto no es del todo cierto, en el ejemplo se puede apreciar como los elementos en bloque se solapan con la imagen flotada a la derecha, aunque el contenido de estos no se solapa

```scss
p {
    background-color: deepskyblue;
    margin-bottom: 5em;
    padding: 1em;
}

img {
    float: right;
}
```

Si necesito que un determinado párrafo se comporte normalmente sin tener en cuenta la imagen flotada puedo utilizar la propiedad **clear: right**
