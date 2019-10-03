# Elementos inline-block
En el ejemplo inicialmente se muestran tres cajas con distintas dimensiones y contenido, al establecer la propiedad **display: inline-block** se alinean horizontalmente y aparentemente se desalinean verticalmente, sin embargo se están alineando por la linea de texto base, valor por defecto de la propiedad **vertical-align**
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

En las sucesivas versiones se cambia la propiedad **vertical-align** con diferetes opciones de alineamiento entre los elementos inline-block
- vertical-align: middle. Alinea los elementos por su centro geométrico
- vertical-align: top. Alinea los elementos por su línea superior
- vertical-align: bottom. Alinea los elementos por su línea inferior