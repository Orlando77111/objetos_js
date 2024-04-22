# objetos_js

En JavaScript, `window` es un objeto global que representa la ventana del navegador. Es el objeto principal a través del cual puedes interactuar con el navegador y controlar diversos aspectos de la ventana y el documento que se está mostrando en ella.

El objeto `window` proporciona acceso a varias propiedades y métodos que te permiten, entre otras cosas:

1. Manipular el tamaño y la posición de la ventana del navegador.
2. Abrir nuevas ventanas o pestañas.
3. Cerrar ventanas.
4. Acceder a la barra de direcciones del navegador.
5. Manipular cookies.
6. Interactuar con los marcos (iframes) en la página.

Por ejemplo, puedes acceder a la propiedad `window.location` para obtener o cambiar la URL actual de la ventana, o puedes utilizar el método `window.open()` para abrir una nueva ventana o pestaña del navegador. La mayoría de las acciones relacionadas con la ventana del navegador se realizan a través del objeto `window`.

## Como se usa window en javascript

El objeto `window` en JavaScript se utiliza de diversas formas para interactuar con la ventana del navegador. Aquí tienes algunos ejemplos comunes de cómo se puede utilizar:

1. **Obtener la URL actual:**
```javascript
var currentURL = window.location.href;
```

2. **Abrir una nueva ventana o pestaña:**
```javascript
window.open("https://www.ejemplo.com", "_blank");
```

3. **Cerrar la ventana actual:**
```javascript
window.close();
```

4. **Obtener el tamaño de la ventana del navegador:**
```javascript
var windowWidth = window.innerWidth;
var windowHeight = window.innerHeight;
```

5. **Redirigir a una nueva URL:**
```javascript
window.location.href = "https://www.ejemplo.com";
```

6. **Mostrar un cuadro de diálogo de confirmación:**
```javascript
window.confirm("¿Estás seguro que deseas continuar?");
```

7. **Mostrar un cuadro de diálogo de alerta:**
```javascript
window.alert("¡Hola! Este es un mensaje de alerta.");
```

8. **Definir/manipular cookies:**
```javascript
document.cookie = "nombre=valor; expires=Fecha";
```

## Ejemplo

Claro, aquí tienes un ejemplo básico de cómo utilizar el objeto `window` en JavaScript para abrir una nueva ventana con un mensaje:

```Javascript
function abrirVentana() {
    // Abre una nueva ventana con un mensaje
    window.open('', '', 'width=400,height=200');
    // Escribe un mensaje en la nueva ventana
    window.document.write("<p>¡Hola! Esta es una ventana emergente.</p>");
}
```

En este ejemplo:

- Hay un botón que, cuando se hace clic en él, llama a la función `abrirVentana()`.
- La función `abrirVentana()` utiliza `window.open()` para abrir una nueva ventana sin una URL específica. Los parámetros `'width=400,height=200'` especifican el ancho y el alto de la ventana.
- Después de abrir la ventana, la función utiliza `window.document.write()` para escribir un mensaje dentro de la nueva ventana.
