# PASOS

1. Establezco sobre el body una altura de 130% sobre la ventana, una imagen de fondo que cubra todo el contenido y no se repita
2. Dentro del body creo una capa con las siguientes características
    - Font-family -> Lato y tamaño 1.6em
    - Color de fondo negro semitransparente
    - Deberá cubrir la ventana, haciendo una especie de velo negro (background-color: rgba(0, 0, 0, .8)), por lo que debere poner el **position: fixed**, si pongo el position: absolute, me dejará al descubierto un 30% del scroll ya que height: 100% será sobre el ancestro que tenga position establecido y quiero que el velo oscuro aparezca siempre.

3. A la caja interior ".box-content" (futuro popup) ancho del 70% y color #828282
4. El titulo y la X de cierre son blancos
5. Centrado horizontal y vertical del ".box-content"
6. Establezco dimensiones al icono 1.8rem de alto y ancho
7. Deberé poner el icono al lado del título, pero manteniendo la caja centrada
8. Al título margen inferor de .5em y un font-size un 10% mayor
9. La X del close necesito que sea un cuadrado perfecto y centrado horizontal y verticalmente

