# GRID DE BOOTSTRAP

El sistema de cuadrícula de Bootstrap utiliza una serie de contenedores, filas y columnas para diseñar y alinear el contenido. Está construido con flexbox y es totalmente responsivfe.

Como funciona:

- Los contenedores proporcionan un medio para centrar y rellenar horizontalmente los contenidos de su sitio. Puedes usar la clase **container** para un ancho centrado o **container-fluid** para un ancho del 100% en todos los tamaños de dispositivo
- Las filas son envoltorios para columnas. Cada columna tiene un relleno horizontal para controlar el espacio entre ellas. Este relleno se contrarresta en las filas con márgenes negativos. De esta manera, todo el contenido de sus columnas se alinea visualmente en el lado izquierdo.
- En un diseño de cuadrícula, el contenido debe colocarse dentro de las columnas y solo las columnas pueden ser elementos secundarios inmediatos de las filas.
- Gracias a flexbox, las columnas de cuadrícula sin un ancho especificado se diseñarán automáticamente como columnas de igual ancho. Por ejemplo, cuatro instancias de .col-sm tendrán automáticamente un 25% de ancho desde el punto de corte pequeño en adelante
- Las clases de columnas indican la cantidad de columnas que le gustaría usar de las 12 posibles por fila. Entonces, si desea tres columnas de igual ancho, puede usar .col-4.
- Los anchos de columna se establecen en porcentajes, por lo que siempre son fluidos y de tamaño relativo a su elemento principal.
- hay cinco puntos de interrupción de la cuadrícula, uno para cada punto de interrupción sensible: todos los puntos de interrupción (extra pequeño), pequeño, mediano, grande y extra grande.
