### ✅ 1.1 Introducción a la Web


-[^1]¿Qué es la web y cómo funciona?
-[^2] Protocolos: HTTP, HTTPS.
-[^3] ¿Qué es un servidor y un cliente?
-[^4]Cómo funciona un navegador web.

### ✅ 1.2 HTML (HyperText Markup Language)
[^5]- Estructura básica de un documento HTML.
[^6]- Etiquetas fundamentales: `<html>`, `<head>`, `<body>`, `<h1>`-`<h6>`, `<p>`, `<a>`, `<img>`, `<div>`, `<span>`.
[^7]- Listas y tablas.
[^8]- Formularios y validación básica.

### ✅ 1.3 CSS (Cascading Style Sheets)
[^9]- Sintaxis y selectores CSS.
[^10]- Modelo de caja (Box Model).
[^11]- Propiedades de diseño: colores, fuentes, márgenes, paddings.
[^12]- CSS Grid y Flexbox para maquetación.
[^13]- Animaciones y transiciones básicas.

### ✅ 1.4 JavaScript Básico
- Variables (`let`, `const`, `var`).
- Tipos de datos y operadores.
- Condicionales y bucles (`if`, `for`, `while`).
- Funciones y eventos.
- Manipulación del DOM.

### 🔹 Ejercicios
1. Crear una página HTML con estilos CSS atractivos.
2. Agregar un botón con un evento en JavaScript que cambie el color de fondo.

[^1]: La web es un subconjunto del internet. Consiste de las páginas web a las cuáles podemos acceder vía un navegador. Es una de las formas en las que se transmite información en internet. La web funciona gracias a la comunicación entre los navegadores web y los servidores que alojan los sitios web, y utiliza una variedad de tecnologías para crear y presentar contenido a los usuarios.




[^2]: El protocolo HTTP es la tecnología subyacente que impulsa la comunicación de red. Como su nombre indica, el protocolo seguro de transferencia de hipertexto HTTPS es una versión más segura o una extensión de HTTP.

[^3]: **El cliente realiza solicitudes de servicios o datos, mientras que el servidor proporciona esos recursos**. Este sistema se basa en una comunicación constante mediante protocolos de red, lo que permite un flujo de información bidireccional entre ambos.




[^4]: Es un programa que permite ver la información que contiene una página web. **El navegador interpreta el código, HTML generalmente, en el que está escrita la página web y lo presenta en pantalla permitiendo al usuario interactuar con su contenido y navegar**




[^5]: La estructura basica sería la siguiente:
	- `<!DOCTYPE html>` → Le dice al navegador que es un documento HTML5.
	- `<html>` - Todo el contenido HTML va dentro de esta etiqueta.
	- `<head>` - Contiene información sobre la página (no visible), como el título o los metadatos.
	- `<body>` - Aquí va el contenido que se ve en la página web.




[^6]:     **html:** Contenedor principal de toda la pagina
		**head:** Informacion no visible, como el titulo
		**body:** Todo el contenido visible va aquí
		**h1 - h6:** Son los titulos, h1 se verá mas grande y h6 mas pequeño.
		**p:** Parrafos de texto
		**a:** Enlaces
		**img:** Inserta imagenes
		**div:** Es un contenedor en bloque
		**span:** Contenedor en linea





[^7]: Podemos hacer 2 tipos de lista:
		No ordenada:
			<ul>
				  <li>Manzana</li>
				  <li>Banana</li>
				  <li>Naranja</li>
			</ul>
		Ordenada:
			<ol>
				  <li>Primer paso</li>
				  <li>Segundo paso</li>
				  <li>Tercer paso</li>
			</ol>




[^8]: Para hacer formularios usamos el comando <form> y con diferentes acciones, por ejemplo podemos hacer un formulario tipo texto que se haría de la siguiente manera:
		
			<form action="/procesar" method="post">
				  <label for="nombre">Nombre:</label>
				  <input type="text" id="nombre" name="nombre" required>
			</form>
	
	

[^9]: La sintaxis básica es así:
	
	Selector {
		propiedad: valor;
	}
	
	Y hay diferentes tipos de selectores:
	- de etiqueta  (p)
	- de clase (.contenedor)
	- de ID (#menu0)
	- Universal (*)
	- Etc

[^10]: Pues en CSS, cada elemento es una caja que está compuesta por varias capas. Desde el interior hacia afuera:
	1- Contenido: Lo que esté dentro de este
	2- Relleno: Espacio entre el contenido y el borde
	3- Borde: El marco que rodea el relleno
	4- Margen: Espacio afuera del borde, separa elementos entre sí

[^11]: -Para los colores, puedes usar nombres (red, blue, green, etc), hexadecimales (#ffff), rgb(), hsl().
	-Para las fuentes, hay difentes etiquetas, font-family, font-size, font-weight, font-style, text-align.
	-Para los margenes, margin: 20px;,  margin-top:, margin-left:, etc.
	-Y para el padding, padding-left, padding:, etc.
	
	Un ejemplo podría ser:
		.contenedor {
			color: #ffff;
			 background-color: red;
			 font-family: sans-serif;
			 margin: 20px;
			 padding-right: 15px;
		}

[^12]: Flexbox es eje flexible, es ideal para distribuir elementos en una sola dirección (fila o columna).
	
	.contenedor {
	  display: flex;
	  justify-content: space-between; /* distribución horizontal */
	  align-items: center;            /* alineación vertical */
	}
	
	<div class="contenedor">
	  <div>Item 1</div>
	  <div>Item 2</div>
	  <div>Item 3</div>
	</div>
	
	
	Y CSS Grid es ideal para crear distribuciones en dos dimensiones (filas y columnas).
	
	.grid {
	  display: grid;
	  grid-template-columns: 1fr 1fr 1fr; /* 3 columnas iguales */
	  gap: 10px;
	}
	
	<div class="grid">
	  <div>Bloque 1</div>
	  <div>Bloque 2</div>
	  <div>Bloque 3</div>
	</div>
	
	

[^13]: Las transiciones nos permiten que hagamos un cambio como color o tamaño, y que ocurra de forma gradual. El comando que usariamos en CSS, sería transition, y lo usariamos de la siguiente forma:
	
	transition: background-colot 0.3s ease;
	
	En este caso lo que haria es que al pasar el raton, el color de fondo cambia suavemente en 0,3 segundos.
	
	Un ejemplo de las animaciones sería el siguiente:
	
	@keyframes mover {
	  from { transform: translateX(0); }
	  to { transform: translateX(100px); }
	}
	
	.caja {
	  width: 100px;
	  height: 100px;
	  background: green;
	  animation: mover 2s ease-in-out infinite;
	}
	
	Esto hará que la caja se mueva de izquierda a derecha repitiendose infinitamente.
	
