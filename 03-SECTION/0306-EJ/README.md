# Ejemplo de menu justificado mediante display: table
El el ejemplo se muestra un menu de manera justificada mediante las propiedades **display: table** y **display: table-cell**
Ventajas: 
- Me permite distribuir elementos de forma tabular sin la rigidez de las tablas (Puede ser responsive)
- Puedo mostra los elementos de manera más semántica (headers, sections, articles, ...)
- Los vamos a usar principalmente para:
    - Menus justificados
    - Columnas de igual altura
    - Alineaciones verticales

La propiedad **table-layout: fixed;** del ejemplo permite igual el tamaplo de todas las celdas (lo cual es mucho más rápida), dejando la propiedad con el valor por defecto el tamaño de las celdas se distribuirá dependiendo del contenido

En el ejemplo también se puede ver que para mejorar las accesibilidad de los enlaces se les añade un padding y se les quita su naturaliza inline para que el padding superior e inferior sea efectivo.