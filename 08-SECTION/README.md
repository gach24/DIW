# ¿Que es FLEXBOX?

- Flexbox es un módulo completo de layout, es decir, define como se muestran los elementos y como se relacionan con el resto
- El contenedor va a poder modificar las dimensiones y el orden de los items para acomodarlos según nuestras indicaciones

## ¿Que cosas podemos hacer con flexbox?

- Alineación vertical
- Columnas de igual altura independientemente del contenido
- Cambiar el orden en el que se muestran los elementos sin que cambie el HTML
- ...

## Introducción

![ejes-flexbox](./doc/img/ejes-flexbox.jpg)

Más información pincha [aqui](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## ¿Como se respetan el tamaño de los items?

- CROSS SIZE (Eje secundario)
  - Si se ha definido (por width o height), este tamaño se respetará
  - Si no se ha definido, se utilizará todo el espacio disponible (stretch)
  - Si no se ha definido y se utiliza un valor diferente de stretch para align-content o align-items en el contenedor, se tomará el tamaño de su contenido
- MAIN SIZE (Eje principal)
  - Si no se ha definido tamaño se calculará según su contenido
  - Si se ha definido (por width o por height) esté podría respetarse, podría encogerse o podría crecer

## Ejemplos

1. [Ejemplo con propiedades **display: flex** y **display: inline-flex**](./0801-EJ)

2. [Ejemplos con propiedades **flex-direction**, **flex-wrap**, **justify-content**, **align-items**, **align-content**](./0802-EJ)

3. 