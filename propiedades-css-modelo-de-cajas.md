
Seguimos trabajando con propiedades CSS, en este video vamos a ver aquellas que nos van a ayudar a estructurar y posicionar los elementos dentro de nuestra web.

## WIDTH Y HEIGHT

Estas propiedades nos van a permitir asignar un ancho y alto específico a un elemento, por ejemplo un div. 

Si creamos un div y le asignamos un color de fondo este no se va a ver, y es que lo que está pasando es que el tamaño del div depende del contenido que contenga.

 

```html
<div class="contenedor"> </div>
```

```css
.contenedor {
	background-color: blue; /* con esta propiedad podemos asignarle un color al fondo*/
}
```

 

Con las propiedades width y height podemos indicar el tamaño del contenedor. ¡Ahora si se ve el azul!

```css
.contenedor {
	background-color: blue; /* con esta propiedad podemos asignarle un color al fondo*/
	width: 500px;
	height: 300px;
}
```

 

## DISPLAY

Si entendemos cada elemento de nuestra página web como una caja. Con la propiedad display estamos indicando como se comporta esta caja dentro de la web. Atributos importantes:

- INLINE: Se muestran los elementos uno detrás de otro, podría ser un span. No acepta las propiedades width y height
- INLINE-BLOCK:  Mostramos los elementos uno detrás de otro pero respetando las propiedades width y height.
- BLOCK: Actúan como bloque, no dejando que los elementos se posicionen a los lados.

Para ver como actúan estos tres atributos sobre nuestros elementos creamos 3 cajas:

```html
<div class="contenedor caja-a"> </div>
<div class="contenedor caja-b"> </div>
<div class="contenedor caja-c"> </div>
```

```css
.contenedor {
	width: 500px;
	height: 300px;
}

.caja-a{
	color:red;
}

.caja-b{
	color:blue;
}

.caja-c{
	color:green;
}
```

Y vamos viendo conforme le apliquemos los atributos como se comportan:

- Cuando les introducimos **inline** no se muestra nada, ya que no soporta altos y anchos definidos.
- Con **inline-block** vemos todos comportándose como un bloque y aprovechando el espacio disponible.
- Con **block** cada elemento se comporta como un bloque independiente.

¡PLUS! Os dejamos un enlace para que empecéis a curiosear con flex. A lo largo del máster lo utilizaremos mucho para maquetar:


https://css-tricks.com/snippets/css/a-guide-to-flexbox/


 

## MODELO DE CAJAS

Vamos ahora a ver el modelo de cajas. Si entendemos un elemento como una caja tenemos:

![Modelo de cajas](S4-recursos/img/modelo-de-cajas.jpg)

- **Contenido de una caja**: Podemos modificar el tamaño con WIDTH y HEIGHT
- **Relleno de la caja:** El espacio en blanco alrededor del contenido. Lo controlamos con el PADDING
- **Borde de la caja:** Borde de la caja que controlamos con la propiedad BORDER
- **El margen de la caja:** El espacio en blanco hacia otros elementos. Controlamos con la propiedad MARGIN

Vamos a probar el modelo de cajas con un párrafo:

```html
<p class="parrafo-principal"> Voy a probar el modelo de cajas con un párrafo</p>
```

Tras analizarlos con el inspector, vamos a ponerle un borde para que veamos el padding y el margin.

```css
.contenedor {
	border: 2px solid black;
}
```

 

Vemos primero como actúa el padding:

```css
.contenedor {
	border: 2px solid black;
	padding: 50px;
}
```

 

Y posteriormente como actúa el margin:

```css
.contenedor {
	border: 2px solid black;
	padding: 50px;
	margin: 150px;
}
```

 

Para asignar border, padding y margin especifico arriba, abajo, izquierda o derecha haríamos:

```css
border-top: 1px solid black; /* borde superior */
border-right: 1px solid black; /* borde derecho */
border-bottom: 1px solid black; /* borde inferior */
border-left: 1px solid black; /* borde izquierdo */

padding-top: 1px; /* padding superior */
padding-right: 1px; /* padding derecho */
padding-bottom: 1px; /* padding inferior */
padding-left: 1px; /* padding izquierdo */
padding: 10px 20px; /* se le asigna 10px al padding superior/inferior y 20 al derecho/izquierdo */
padding: 1px 1px 1px 1px; /* en orden: superior-derecha-inferior-izquierda */

margin-top: 1px; /* margin superior */
margin-right: 1px; /* margin derecho */
margin-bottom: 1px; /* margin inferior */
margin-left: 1px; /* margin izquierdo */
margin: 10px 20px; /* se le asigna 10px al padding superior/inferior y 20 al derecho/izquierdo */
margin: 1px 1px 1px 1px; /* en orden: superior-derecha-inferior-izquierda */
```

 
