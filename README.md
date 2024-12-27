# Frontend CRUD con Vue.js

Este proyecto es un frontend desarrollado en **Vue.js** que interactúa con un backend en **Spring Boot** para realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) en una lista de personas.

## Características

- Listado de usuarios con paginación.
- Creación de nuevos usuarios.
- Edición de usuarios existentes.
- Eliminación de usuarios.
- Integración con un backend REST API alojado en Render.
- Diseño responsive utilizando **Bootstrap**.

## Requisitos previos

Asegúrate de tener lo siguiente instalado:

- Navegador moderno (Google Chrome, Firefox, Edge, etc.).
- **Node.js** y **npm** instalados en tu sistema (si planeas hacer modificaciones al proyecto).

## Tecnologías utilizadas

- **Vue.js**: Framework frontend para crear interfaces de usuario reactivas.
- **Bootstrap 5**: Framework CSS para diseños responsivos.
- **Fetch API**: Para la comunicación con el backend.

## Configuración

### Paso 1: Clonar el repositorio

Clona el repositorio de este proyecto en tu computadora:

```bash
git clone https://github.com/harnelp/front_crund_java
```

### Paso 2: Configurar el backend

Asegúrate de que el backend de Spring Boot esté funcionando y accesible en la URL configurada. Este proyecto utiliza la URL:

```
https://springboot-crud-x14q.onrender.com
```

Si necesitas cambiar esta URL, modifica la variable `baseUrl` en el código del frontend.

### Paso 3: Desplegar el frontend

Si no planeas modificar el código del frontend, simplemente despliega los archivos HTML en un servicio como **Netlify**, **Vercel**, o cualquier servidor web estático.

1. Ve a la página de configuración de tu servicio de despliegue.
2. Selecciona los archivos del proyecto.
3. Publica el proyecto.

La URL del frontend quedará accesible una vez desplegado.

## Uso

1. Abre la URL del frontend en tu navegador.
2. Utiliza los botones "Crear Usuario", "Editar" o "Eliminar" para realizar operaciones CRUD.
3. Usa los botones de paginación para navegar entre las páginas de usuarios.

## Cómo cambiar el número de usuarios por página

El número de usuarios mostrados por página se define mediante la variable `pageSize` en el código del frontend. Para cambiar este valor:

1. Abre el archivo HTML del proyecto.
2. Encuentra la sección de `data()` donde se define `pageSize`.
3. Cambia el valor a la cantidad deseada:

```javascript
pageSize: 10, // Cambiar "10" al número deseado
```

4. Guarda los cambios y vuelve a desplegar el frontend si es necesario.

## Endpoints del backend

El frontend interactúa con los siguientes endpoints del backend:

- `GET /api/persons/paged?page={page}&size={size}`: Obtener usuarios con paginación.
- `POST /api/persons`: Crear un nuevo usuario.
- `PUT /api/persons/{id}`: Actualizar un usuario existente.
- `DELETE /api/persons/{id}`: Eliminar un usuario.

## Contribuir

Si deseas contribuir a este proyecto:

1. Haz un fork del repositorio.
2. Crea una rama con el nombre de tu función o mejora.
3. Realiza los cambios necesarios y haz un commit.
4. Envía un pull request describiendo tus cambios.

## Enlace al Proyecto en Producción

Puedes probar el proyecto en el siguiente enlace:

👉 [CRUD Frontend - Desplegado en Netlify](https://front-crud-spring.netlify.app/)


