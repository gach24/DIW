# Multicolumn layout
Me permite dividir en columnas según indique el número (column-count) o ancho (column-width)
Propiedades importantes:
- **column-count**. Establece el número de columnas
- **column-gap**. Establece la separación entre columnas
- **column-rule**. Establece la línea de separacion entre columnas (grosor, tipo y color)
- **column-width**. No es posible establecer %

En el ejemplo se puede ver un div con tres columnas, separación entre columnas de 3rem, una línea de separación entre columnas y con el texto justificado
```
    div {
        ...
        column-count: 3; // Tres columnas
        column-gap: 3rem; // Separación entre columnas
        column-rule: 1px solid white;  // Línea divisoria entre columnas
        text-align: justify; // Texto justificado
    }
```

