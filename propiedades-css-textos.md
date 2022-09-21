Ahora que ya sabemos como trabajar con CSS y hemos visto las formas en que podemos seleccionar etiquetas para asignarles estilos, vamos dar un repaso a las básicas para poder empezar a trabajar.

Tenemos que tener en cuenta que existen infinidad de propiedades que van a permitir modificar el estilo de nuestra página web. Os dejamos una web que tiene un listado completo de propiedades para que curioseéis:


[https://css-tricks.com/almanac/properties/](https://css-tricks.com/almanac/properties/)


En este video vamos a trabajar con estilos que podemos aplicar a los textos de nuestra web, en el siguiente, veremos posicionamiento y estructura.

Así que empezamos, las propiedades que vamos a ver son las siguientes:

**COLOR**

Cambia el color del texto. Es una propiedad que ya hemos ido usando. Por ejemplo, podemos cambiar directamente el color de un párrafo.

```html
<p> Párrafo verde </p>
```

```css
p {
  color:green;
} 
```

A demás de poder introducir una serie de colores predefinidos podemos utilizar otras formas de nombrar esos colores:

**Códigos hexadecimales**

Mediante el código hexadecimal podemos elegir un color específico, por ejemplo cuando tengamos que trabajar con la identidad corporativa de una marca.

```html
<p> Párrafo verde </p>
```

```css
p {
  color: #71BD56; /* otro color de verde */
} 
```

**Códigos RGB**

De igual manera, podemos aplicar un código de color rgb para darle estilo a nuestro HTML

 

```html
<p> Párrafo verde </p>
```

```css
p {
  color: rgb(113, 189, 86); /* otro color de verde */
} 
```

 

Si a parte de color queremos establecer una opacidad trabajando con **rgb**, existe la posibilidad de definir un color con **rgba**, siendo este último argumento la opacidad que queramos darle.

 

```html
<p> Párrafo verde </p>
```

```css
p {
  color: rgba(113, 189, 86, 0.5); /* otro color de verde con opacidad 50% */
} 
```

 

Esta página es muy interesante para trabajar con colores: 


[https://htmlcolorcodes.com/es/](https://htmlcolorcodes.com/es/)


**FONT-SIZE**

Nos permite cambiar el tamaño de los textos dentro de nuestra web. Por defecto, cada etiqueta tiene asociados unos tamaños de texto que podemos cambiar. De momento la unidad de medida con la que vamos a trabajar son los PX que son una unidad relativa a la resolución de pantalla.

Para cambiar el tamaño de letra sería de la siguiente forma:

```css
p {
  font-size: 20px; /* otro color de verde con opacidad 50% */
} 
```

 

**FONT-FAMILY**

La propiedad font-family nos permite cambiar la fuente de nuestra página a una que nuestro navegador la soporte por defecto.

```html
<h2 class="titulo-seccion-a"> Título1 </h2>
<h2 class="titulo-seccion-b"> Título1 </h2>
```

```css
.titulo-seccion-a {
  font-family: monospace;
} 

.titulo-seccion-b {
  font-family: sans-serif;
}
```

 

**FONT-WEIGHT**

Nos permite cambiar el grosor de nuestra fuente. Permite seleccionar valores del 100 al 900 y atributos como (normal, lighter, bold, bolder)

```html
<h2 class="titulo-seccion-a"> Título1 </h2>
<h2 class="titulo-seccion-b"> Título1 </h2>
```

```css
.titulo-seccion-a {
  font-weight: lighter;
} 

.titulo-seccion-b {
  font-weigth: bold;
}
```

 

**TEXT-DECORATION**

La propiedad text decoration nos sirve para poder darle una decoración a un texto pudiéndolo subrayar, tachar…

```html
<h2 class="titulo-seccion-a"> Título1 </h2>
<h2 class="titulo-seccion-b"> Título1 </h2>
```

```css
.titulo-seccion-a {
	text-decoration: underline;
} 

.titulo-seccion-b {
	text-decoration: line-through;
}
```

 

La propiedad text-decoration nos es de gran ayuda también cuando trabajamos con enlaces. Las etiquetas tienen propiedades asignadas por defecto y el enlace tiene un underline que podemos quitar usando el text-decoration

```css
a {
  text-decoration: none;
} 
```

 

**TEXT-TRANSFORM**

Propiedad que nos permite transformar un texto, poniéndolo todo en mayúsculas, minúsculas, capitalizarlo…

```html
<h2 class="titulo-seccion-a"> Título1 </h2>
<h2 class="titulo-seccion-b"> Título1 </h2>
```

```css
.titulo-seccion-a {
  text-transform: uppercase;
} 

.titulo-seccion-b {
  text-decoration: lowercase;
}
```

 

En el siguiente vídeo seguimos trabajando con propiedades CSS.
