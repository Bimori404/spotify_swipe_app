# Music Swipe App - Change Log

## Version 1.0.0

**Features Added:**

1. **Estructura HTML**:
   - Se añadió una estructura HTML básica para la aplicación de deslizamiento de música.
   - Se incluyó un contenedor para insertar dinámicamente las tarjetas de canciones.

2. **Integración de Tailwind CSS**:
   - Se integró Tailwind CSS para el estilo de la aplicación.
   - Se estilizó la tarjeta de deslizamiento con color de fondo, esquinas redondeadas, sombra y manejo de desbordamiento.
   - Se añadieron estilos para el contenido de la tarjeta y los botones de acción.

3. **JavaScript para Obtener y Manejar Datos**:
   - Se agregó una función `fetchSongs` para obtener datos de canciones de la API de Spotify usando RapidAPI.
   - Se implementó manejo de errores para solicitudes a la API.
   - Se añadió una función `createCard` para crear dinámicamente tarjetas de canciones con portada de álbum, título de canción y nombres de artistas.
   - Se incluyeron escuchadores de eventos para los botones de aceptar y rechazar para manejar acciones de deslizamiento.
   - Se agregó una función `initialize` para obtener canciones al cargar el documento y agregar tarjetas de canciones al contenedor.

## Version 1.1.0

**Added:**

- Propiedad `overflow-x: hidden` al elemento `body` para evitar el desplazamiento horizontal no deseado en dispositivos móviles.
- `min-height: 100vh` a la clase `.bg-svg` para asegurar que el fondo cubra toda la altura de la pantalla.
- `background-position: center` a la clase `.bg-svg` para centrar el fondo por defecto.
- Media query para dispositivos con ancho máximo de 767px, ajustando `background-position: top` para mejorar la visualización del fondo en pantallas pequeñas.
- Ajustes en las dimensiones de `.swipe-card` para pantallas pequeñas.

**Fixed:**

- Problema con la carga de imágenes de usuario en dispositivos móviles.
- Error que causaba que las tarjetas finales no se mostraran correctamente cuando se agotaban las pistas disponibles.

## Version 1.2.0

**Added:**

- Funcionalidad de deslizamiento para aceptar o rechazar pistas.
- Vista previa de pistas antes de aceptarlas.

**Changed:**

- Rediseño de la interfaz de usuario.
- Actualizaciones en las solicitudes a la API de Spotify.

**Fixed:**

- Problema con la visualización de algunas pistas.
- Errores de estilo y diseño.

## Version 1.3.0

**Added:**

- Formulario de inicio de sesión con Tailwind CSS.
- Validación de credenciales de usuario.
- Botón "Login with Spotify" para iniciar autenticación.
- Funcionalidad de redirección a la página de autorización de Spotify.
- Script JavaScript para manejar el inicio de sesión y la autenticación con Spotify.

**Changed:**

- Modificación del flujo de autenticación.

## Version 1.4.0

**Added:**

- Creacion de README.md.
- Separación del código en archivos HTML, JavaScript y CSS.
- Funcionalidad para autenticarse con Spotify usando OAuth 2.0.
- Creación de playlists en Spotify.
- Añadir canciones a playlists en Spotify.

## Version 2.0.0

**Features:**

- Implementación de un flujo de inicio de sesión para acceder a cuentas de Spotify.
- Mejoras en la interfaz de usuario y experiencia del usuario.
- Integración de un reproductor de música en la parte inferior de la página.

**Improvements:**

- Consolidación de código JavaScript y HTML en un solo archivo.
- Actualización de estilos y posicionamiento para soporte del reproductor de música.
- Mejora en la legibilidad y mantenibilidad del código.

## Version 2.1.0

**Added:**

- Funcionalidad de "Logout".
- Mostrar la imagen de perfil del usuario en el botón de usuario.

**Changed:**

- Actualización del README.
- Mejora de la adaptabilidad para dispositivos móviles.
- Ajustes en el diseño de las tarjetas en móviles.

**Fixed:**

- Problema con el cierre de sesión.
- Reproducción continua de canciones al rechazar una tarjeta.

## Version 2.3.0

**New Features:**

- Función de Acceso como Invitado:
  - Se agregó un nuevo botón para permitir a los usuarios acceder a la aplicación como invitados utilizando las credenciales proporcionadas.

  - Se implementó una funcionalidad básica de autenticación de invitados en JavaScript para simular el inicio de sesión de invitados utilizando las credenciales proporcionadas.

**Changes:**

- Ajustes Menores de UI:
  - Se realizaron ajustes menores en el diseño de la interfaz de usuario para una mejor presentación visual.

**Bug Fixes:**

- Manejo de Credenciales de Invitados:
  - Se incluyó un aviso sobre la naturaleza insegura de almacenar y utilizar directamente las credenciales de invitados en el frontend, y se enfatizó la importancia de manejar de manera segura la autenticación de usuarios en el backend.

**Security and User Experience Improvements:**

- Manejo de Solicitudes CORS:
  - Se abordó el problema de CORS (Cross-Origin Resource Sharing) al realizar solicitudes desde el cliente hacia un servidor externo.
  - Se sugirió la configuración del servidor para incluir el encabezado `Access-Control-Allow-Origin` o el uso de un proxy durante el desarrollo para evitar problemas de CORS.

- Consideraciones de Seguridad:
  - Se destacó la importancia de manejar correctamente las credenciales y tokens, especialmente en entornos de producción, para garantizar la seguridad de los usuarios.

**Known Issues:**

- Almacenamiento Inseguro de Credenciales:
  - El uso directo de las credenciales de invitados en el frontend es inseguro y debe abordarse mediante la implementación de mecanismos seguros de autenticación en el backend.

**Notas Adicionales:**

- Requiere Integración con el Backend:
  - Aunque se ha implementado una autenticación básica de invitados con fines de demostración, se recomienda encarecidamente integrar esta función con un backend seguro para el manejo adecuado de credenciales y autenticación.

- Consideraciones de Experiencia de Usuario:
  - Se debe informar a los usuarios sobre las limitaciones y riesgos asociados con el acceso de invitados, y se les debe animar a utilizar métodos de autenticación más seguros siempre que sea posible.
