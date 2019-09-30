# Sección 02. Ejemplo 01. Introducción a Sass
## Ejemplo de declaración de variable
Se declara una variable y se establece el color
```
$text: blue;
```
A continuación utiliza la variable en la propiedad color del body
```
$text: blue;
body {
    color: $text;
}
```

## Opciones de compilación
- Compilación del .scss generando la salida .css en la carpeta css
```
$ sass scss/style.scss:css/style.css
```

- Realizar la compilación cada vez que se realiza un cambio
```
$ sass --watch scss/style.scss:css/style.css
```


## Aplicaciones gráficas
1. Compass
2. Scout
3. Koala
4. Prepros

También se pueden utilizar Sass es utilizar Task Runners
1. Gulp (Será visto más adelante)
2. Grunt

Nota: Sass tiene diferentes lenguajes, nosotros utilizaremos la Scss que es más amigable y fácil de aprender
