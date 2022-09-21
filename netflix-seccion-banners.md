Toca ahora crear la estructura de nuestro banner:

- Identificamos un bloque con un título y un texto
- Una imagen

```html
<section>
      <div>
          <h3>Disfruta de Netflix en tu TV.</h3>
          <p>Smart TV, Playstation, Xbox, Chromecast, Apple TV, reproductores Blu-ray y muchos más.</p>
      </div>
      <img src="./assets/banner-1.png" alt="">
 </section>
```

Le asignamos estilos:

```html
<section class="banner">
        <!-- metemos un div para limitar el ancho y que flex no nos ponga todos los textos en una linea -->
        <div class="banner-info">
            <h3 class="banner-title">Disfruta de Netflix en tu TV.</h3>
            <p class="banner-text">Smart TV, Playstation, Xbox, Chromecast, Apple TV, reproductores Blu-ray y muchos más.</p>
        </div>
        <img class="banner-image" src="./assets/banner-1.png" alt="">
    </section>
```

```css
.banner {
  display: flex;
  justify-content: center;
  padding: 70px 0;
  border-bottom: 8px solid #222;
}

.banner-info {
  max-width: 500px;
  margin: 0px 70px;
}

.banner-title {
  font-size: 50px;
  margin-top: 0px;
}

.banner-text {
  font-size: 26px;
}

.banner-image {
  width: 500px;
  height: auto;
}
```

A partir de aquí creamos los otros 3 bloques que tienen la misma estructura con la única diferencia del posicionamiento de las imagenes.
