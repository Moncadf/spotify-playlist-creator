# Spotify Playlist Creator

## Descripción
Este proyecto permite a los usuarios iniciar sesión con su cuenta de Spotify y generar automáticamente una playlist con sus 50 canciones más escuchadas. Es una aplicación web sencilla que utiliza la API de Spotify para autenticación y manejo de playlists.

---

## Características
- Autenticación de usuario mediante OAuth 2.0.
- Obtención de las 50 canciones más escuchadas del usuario.
- Creación de una nueva playlist personalizada con estas canciones.

---

## Requisitos
- Cuenta de Spotify.
- Una aplicación registrada en [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/) para obtener un **Client ID**.

---

## Instalación y Configuración
### 1. Clonar el repositorio
```bash
git clone https://github.com/tu_usuario/spotify-playlist-creator.git
cd spotify-playlist-creator
```

### 2. Configurar el proyecto
1. Abre el archivo `index.html`.
2. Reemplaza los siguientes valores:
   - `TU_CLIENT_ID` con el Client ID de tu aplicación de Spotify.
   - `redirectUri` con la URL de redirección que has configurado (por ejemplo, `http://localhost:5500`).

### 3. Ejecutar en un servidor local
Si estás probando en localhost, utiliza un servidor local simple como [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) o el comando Python:
```bash
# Para Python 3
python -m http.server 5500
```
Visita `http://localhost:5500` en tu navegador.

---

## Uso
1. Abre la aplicación en tu navegador.
2. Haz clic en "Inicia sesión con Spotify".
3. Autoriza el acceso a tu cuenta de Spotify.
4. Una vez autenticado, haz clic en "Crear Playlist".
5. La aplicación creará una playlist con tus 50 canciones más escuchadas y la guardará en tu cuenta.

---

## Notas
- La playlist se crea como privada por defecto.
- Si encuentras errores relacionados con permisos, asegúrate de haber incluido los scopes necesarios: `user-top-read`, `playlist-modify-public`, `playlist-modify-private`.

---

## Tecnologías utilizadas
- **HTML5**: Estructura de la página.
- **JavaScript**: Lógica para la interacción con la API de Spotify.
- **Spotify Web API**: Para autenticación y manejo de datos de usuario.

---

## Recursos útiles
- [Documentación de la API de Spotify](https://developer.spotify.com/documentation/web-api/)
- [Ejemplos de Spotify](https://developer.spotify.com/documentation/web-api/getting-started/)

---

## Licencia
Este proyecto está licenciado bajo la MIT License. Puedes ver más detalles en el archivo `LICENSE`.
