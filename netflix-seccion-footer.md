Por último el footer. Tenemos:

- Un mensaje con ‘¿Preguntas?….’
- Muuuuuuchos enlaces divididos en 4 columnas.

Estructuramos primero el HTML

```html
<footer>
        <p>¿Preguntas? Llama al 900 822 376</p>
        <div>
            <div>
                <a href="#">Preguntas frecuentes</a>
                <a href="#">Inversores</a>
                <a href="#">Formas de ver</a>
                <a href="#">Información corporativa</a>
                <a href="#">Avisos legales</a>
            </div>
	           <!-- Resto de columnas con enlaces -->
        </div>

    </footer>
```

Aplicamos estilos. Lo importante es ver que necesitamos posicionar en líneas diferentes los enlaces y que el bloque que contiene esos enlaces podemos darle estilo con un display flex.
