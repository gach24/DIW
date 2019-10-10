# Posicionamiento con float
La propiedad **float** me desplaza todo lo posible un elemento hacia la izquierda o derecha de la línea en la que se encuenran, sin embargo si hay otras cajas flotando no se superponen sino se colocan lo más a la izquierda o derecha que puede sin solaparse
Sin embargo existen diversas consideraciones:
- Los elementos no flotantes que se encuentren despues de un elemento flotante, pueden pasar varias cosas:
    1. Si el elemento se dibuja en línea, hace sitio adaptando su ancho al espacio libre dejado por el elemento/s que flotan
    2. Si el elemento se dibuja en bloque, no les hace sitio (ocupan su lugar) pero adaptan su contenido para no solapar con el elemento flotado

# Limpiar floats

Ejemplos:
