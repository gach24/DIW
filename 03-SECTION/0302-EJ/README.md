# Elementos de bloque
En el ejemplo se muestran dos cajas que son elementos de bloque por defecto, ambas cajas ocupan un 30% del ancho, sin embargo al ser elementos de bloque no permiten otros elementos a sus lados como si ocuparan todo el ancho disponible
De forma que ambas cajas se muestran una debajo de la otra
Por otra parte al ser un elemento de bloque también se les puede establecer un alto 
```
div {
    border: 1px solid; // Para ver sus dimensiones 
    width: 30%; // Ocupa un 30% sin embargo no permite elementos a sus lados como si ocupara todo el ancho disponible
    height: 20rem; // También permite establecer un alto
}
```