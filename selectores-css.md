A lo largo de este video vamos a ver las formas que tenemos de asignar estilos al HTML, tanto con etiquetas genéricas, como a un grupo de ellas o a una específica.

## TIPOS DE SELECTORES

### ETIQUETA

Tenemos la opción de aplicar un estilo asignándoselo a una etiqueta. Este estilo recaerá sobre todas las etiquetas del documento.

```html
<!-- Los dos títulos serán de color azul-->

<h1>Título</h1>
<h1>Título2</h1>
```

```css
h1{
	color: blue;
}
```

El color azul se asignará a todas las etiquetas ```<h1>``` del documento.

### CLASES

Las clases nos sirven para asignar una propiedad a un grupo de etiquetas que nosotros queramos (las etiquetas pueden ser diferentes). En HTML utilizamos el atributo **class**

```html
<h2 class="titulo-rojo">Subtítulo 1</h2>
<h3 class="titulo-rojo">Subtítulo 2</h3>
```

En CSS las clases se identifican con un punto .

```css
.titulo-rojo {
	color: red;
}
```

### ID

El id es un identificador único, por lo que nos valdrá para asignarle un valor a una etiqueta concreta. Al ser un identificador único, no puede duplicarse.

```html
<p id="parrafo-principal">Este es el párrafo principal</p>
```

En CSS las clases se identifican con una almohadilla #

```css
#parrafo-principal{
	color:green;
}
```

## PESO Y HERENCIA DE LOS SELECTORES

Una etiqueta puede tener estilos asignados por etiqueta, clase o id. Estos se compaginan, y en caso de coincidir, se prioriza desde el más específico al más amplio.


> ID > CLASE > ETIQUETA


Como podemos  tener varias clases asignadas a una etiqueta, puede darse el caso que ambas clases asignen un color distinto al texto. Como la hoja de estilos se lee de arriba a abajo, se asignará el valor de la última clase. En este ejemplo el título saldrá verde. Hay que tener mucho cuidado con esto para evitar pisar propiedades.

```html
<h1 class="titulo-rojo titulo-verde">Título>/h1
```

```css
.titulo-rojo {
	color: red;
}

.titulo-verde {
	color: green;
}
```

Cuando vimos la estructura de HTML explicamos que se trataba de una estructura de árbol con padres, hijos… 

Esto cobra importancia también ahora, ya que algunos valores se heredan de los padres y abuelos. Hay otras que no se heredan. Las iremos viendo conforme trabajemos.

```html
<div class="texto-verde">
  <h4>Título</h4>
  <h4>Título</h4>
</div>

```

```css
.texto-verde {
  color: green;
}
```
