# Espacio en blanco en las imagenes
En el ejemplo se puede ver una imagen (por defecto elemento con naturaleza inline) rodeado de un div con un borde, y se aprecia un pequeño espacio en la parte inferior de la imagen (entre la imagen y el borde del div)
Este espacio se debe a que el navegador interpreta la imagen como un caracter
Al estar en línea con otros caractéres reserva el espacio para representar caracteres que requieren un espacio por debajo como la p,q, ...

Posibles soluciones:
- En la mayoría de los casos podemos solucionar este problema estableciendo la propiedad **display a block**
```
    <div>
        <img src="http://dummyimage.com/200x200" alt="Dummy image">
    </div>

    ...
    img  {
        display: block;        
    }
```

- Estableciendo la propiedad **font-size del padre a 0**

