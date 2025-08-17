# Proyecto: Mi Primer Fetch con la API de Rick and Morty

Este es un proyecto fundamental en mi ruta de aprendizaje, ya que representa mi primera incursión en el consumo de APIs y el manejo de la asincronía en JavaScript. Utilicé la popular [API de Rick and Morty](https://rickandmortyapi.com/) para practicar y solidificar mi comprensión de `fetch` con promesas.

> **Nota del desarrollador:** Este proyecto fue construido utilizando la sintaxis `.then().catch()` para manejar las promesas. Es un reflejo de mis habilidades en ese momento y sirve como base para futuras mejoras y refactorizaciones con técnicas más modernas como `async/await`.


## ✨ Características

- **Conexión con API externa:** Realiza una petición `GET` a la API de Rick and Morty para obtener una lista de personajes.
- **Renderizado Dinámico:** Utiliza JavaScript para crear tarjetas de personaje en el DOM sin necesidad de tenerlas escritas en el HTML estático.
- **Manipulación del DOM:** Cada tarjeta de personaje se crea y se añade al contenedor principal mediante métodos como `createElement`, `appendChild` y `classList.add`.
- **Diseño con CSS:** Incluye estilos para presentar la información de manera clara y atractiva, con un diseño de tarjetas responsivo usando Flexbox.
- **Indicador de Estado:** Muestra el estado del personaje (Vivo, Muerto o Desconocido) con un ícono de color distintivo gracias a Font Awesome.

## 🚀 Tecnologías Utilizadas

- **HTML5:** Para la estructura básica de la página.
- **CSS3:** Para el diseño y la apariencia.
- **JavaScript (ES6+):** El corazón del proyecto, encargado de toda la lógica.
- **Fetch API con Promesas (`.then/.catch`):** Para realizar las peticiones HTTP asíncronas.
- **Font Awesome:** Para los íconos de estado.

## 🧠 Conceptos Aprendidos

Este proyecto fue mi primera experiencia utilizando `fetch` y marcó un hito en mi aprendizaje de JavaScript asíncrono. Los conceptos clave que puse en práctica se centraron en el manejo de promesas con la sintaxis tradicional de `.then()` y `.catch()`:

- **Peticiones Asíncronas:** Entender que las peticiones a una API no bloquean la ejecución del resto del código.
- **Promesas y Encadenamiento (`.then()`):** `fetch` devuelve un objeto `Promise`. Aprendí a encadenar métodos `.then()` para manejar el resultado de esta promesa.
  - El **primer `.then()`** se usa para tomar el objeto `Response` y convertir su cuerpo a formato JSON usando el método `response.json()`, que a su vez devuelve otra promesa.
  - El **segundo `.then()`** recibe los datos ya en formato JSON, listos para ser utilizados (en este caso, para iterar sobre ellos y crear las tarjetas).
- **Manejo de Errores (`.catch()`):** Implementé un bloque `.catch()` al final de la cadena para capturar cualquier error que pudiera ocurrir durante la petición de red o el procesamiento de los datos, evitando que la aplicación se rompa y mostrando el error en la consola.
- **Creación de Elementos HTML desde JS:** Generar la estructura de las tarjetas de personaje de forma programática, lo que permite escalar la aplicación para mostrar más o menos personajes.
- **Iteración de Datos:** Usar el método `forEach` para recorrer el array de personajes recibido de la API y crear una tarjeta para cada uno.

## 🏃‍♂️ Cómo ejecutar el proyecto

1.  Clona este repositorio en tu máquina local.
    ```bash
    git clone https://github.com/tu-usuario/proyecto-API-RickandMorty.git
    ```
    *(Reemplaza `tu-usuario` con tu nombre de usuario de GitHub)*

2.  Navega a la carpeta del proyecto.

3.  Abre el archivo `index.html` en tu navegador web preferido.

¡Y listo! Las tarjetas de los personajes deberían aparecer en la pantalla.
