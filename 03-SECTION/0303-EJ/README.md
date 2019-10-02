# Elementos inline-block
En el ejemplo inicialmente se muestran dos cajas con las mismas dimensiones pero con distinto contenido, al establecer la propiedad **display: inline-block** se alinean horizontalmente y aparentemente se desalinean verticalmente, sin embargo se están alineando por la linea de texto base, valor por defecto de la propiedad **vertical-align**
```
div {
    background-color: salmon;
    color: white;
    border: 1px solid;
    width: 20rem;
    height: 20rem;
    ...

    display: inline-block;  
    // vertical-align: baseline; // Valor por defecto
}
```