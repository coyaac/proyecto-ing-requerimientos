# 🎵 SoundMate – Red Social Musical Basada en tu Spotify

## 🎧 Descripción del proyecto  
**SoundMate** es una red social para amantes de la música que permite compartir lo que escuchas, descubrir nuevas canciones y conectarte con personas que tienen gustos similares, todo basado en tu perfil de Spotify. A través de una interfaz personalizada y recomendaciones inteligentes, SoundMate transforma tu historial de escucha en una experiencia social única.

---

## 📲 Funcionalidades principales

- 🔗 Sincronización automática con tu cuenta de Spotify  
- 🧬 Perfil musical personalizado: artistas favoritos, géneros, playlists  
- 🧑‍🤝‍🧑 Recomendaciones de usuarios con gustos similares  
- 📡 Feed en tiempo real con lo que tus amigos están escuchando  
- 🎯 Sugerencias de música personalizadas  
- 🔁 Compartir canciones, playlists y estados musicales  

---

## ⚙️ Aspectos técnicos

### 🏗️ Arquitectura general

- **Frontend:** Next.js + TailwindCSS  
- **Backend:** Node.js + Express  
- **Base de datos:** PostgreSQL (via Prisma ORM)  
- **Autenticación:** OAuth 2.0 con Spotify  
- **Integración externa:** Spotify Web API  
- **Recomendaciones:** Sistema basado en embeddings musicales (vectores de similitud)

---

### 🧩 Módulos principales

#### 1. Login / Registro
- Autenticación vía Spotify (OAuth)
- Almacenamiento seguro de tokens y datos del usuario
- Opción para configurar privacidad del perfil

#### 2. Perfil musical
- Estadísticas: artistas más escuchados, géneros, canciones top
- Visualización de cambios semanales/mensuales
- Comparación de perfiles con amigos

#### 3. Feed social
- Muestra lo que tus contactos están escuchando en tiempo real
- Opción de dar "me gusta", comentar y guardar canciones
- Publicaciones personalizadas (ej. “Mi canción del día”)

#### 4. Recomendador de amistades
- Algoritmo que analiza tu historial y genera matches musicales
- Muestra perfiles con compatibilidad alta
- Posibilidad de seguir o chatear con matches

#### 5. Recomendador musical
- Playlists personalizadas según tu historial + el de tus amigos
- Explorador por moods, géneros y artistas en tendencia

#### 6. Configuración y privacidad
- Control total sobre qué se comparte
- Filtros para mostrar u ocultar actividad
- Notificaciones y gestión de conexión con Spotify

---

## 🧪 Tecnologías utilizadas

| Componente        | Tecnología                     |
|-------------------|-------------------------------|
| Frontend          | Next.js + TailwindCSS         |
| Backend           | Node.js + Express             |
| Base de datos     | PostgreSQL + Prisma ORM       |
| Autenticación     | OAuth 2.0 (Spotify)           |
| Recomendaciones   | TensorFlow.js + Cosine Similarity |
| APIs externas     | Spotify Web API               |
| Visualización     | Chart.js / D3.js              |

---

## 🗺️ Roadmap

### MVP (Versión inicial)
- ✅ Login con Spotify  
- ✅ Perfil musical básico  
- ✅ Feed con lo que estás escuchando  
- ✅ Recomendaciones simples de usuarios  

### Fase 2
- 💬 Sistema de mensajes y conexión entre usuarios  
- 🎧 Recomendaciones de música personalizadas  
- 📊 Estadísticas avanzadas y visualizaciones  

### Fase 3
- 🧠 Algoritmo de matching musical más preciso (AI)  
- 🤝 Playlist colaborativas  
- 📱 Versión móvil (PWA o React Native)

---

## 👥 Público objetivo

- Melómanos que buscan nuevas conexiones  
- Usuarios activos de Spotify  
- Personas que valoran la música como lenguaje social  
- Artistas independientes que buscan visibilidad  

---

## 🚀 Objetivo final

Crear una plataforma donde la música sea el puente para crear conexiones humanas auténticas, permitiendo descubrir canciones, artistas y personas a través de lo que más te representa: lo que escuchas.

---

## 📌 Estado del proyecto

> 🚧 Proyecto en desarrollo activo  
>  
> Se aceptan colaboraciones y sugerencias. ¡Feel free to fork and contribute!

---

## 📝 Licencia

Este proyecto está bajo la licencia [MIT](LICENSE).

---

## 🤝 Contribuciones

¿Quieres colaborar? ¡Genial! Por favor, revisa las normas de contribución en [CONTRIBUTING.md](CONTRIBUTING.md) y comienza con un pull request.

---

<img width="3840" height="1680" alt="Untitled diagram _ Mermaid Chart-2025-08-20-205021" src="https://github.com/user-attachments/assets/c491a256-9ed8-4c53-b6af-4925121d3a22" />

| test id case | test case scenario           | test case                                  | pre-conditions                       | test steps                                                                                 | test data                          | expected results                                       | quality       |
|--------------|-----------------------------|--------------------------------------------|------------------------------------|--------------------------------------------------------------------------------------------|----------------------------------|-------------------------------------------------------|---------------|
| TC001        | Login con Spotify            | Autenticación exitosa con cuenta Spotify  | Usuario tiene cuenta válida en Spotify | 1. Abrir app SoundMate; 2. Seleccionar login con Spotify; 3. Ingresar credenciales Spotify | Usuario y contraseña Spotify válidos | Usuario autenticado, redirigido al feed principal     | Funcionalidad |
| TC002        | Login con Spotify            | Autenticación fallida con credenciales inválidas | Usuario tiene cuenta Spotify       | 1. Abrir app; 2. Seleccionar login con Spotify; 3. Ingresar credenciales incorrectas        | Usuario/contraseña incorrectos   | Mensaje de error "Credenciales inválidas" y no acceso | Seguridad     |
| TC003        | Sincronización automática   | Datos sincronizados correctamente          | Usuario autenticado y tiene historial en Spotify | 1. Login exitoso; 2. Navegar a perfil musical                                            | Cuenta Spotify con historial musical | Perfil musical muestra artistas, géneros y playlists correctos | Funcionalidad |
| TC004        | Perfil musical personalizado | Visualización correcta de estadísticas     | Sincronización completada          | 1. Acceder al perfil musical; 2. Ver estadísticas (artistas, géneros, canciones top)       | Datos de usuario con historial variado | Estadísticas muestran datos reales y actualizados    | Usabilidad    |
| TC005        | Feed social                 | Visualizar actividad de amigos en tiempo real | Usuario autenticado y con amigos conectados | 1. Ingresar al feed; 2. Observar publicaciones de amigos con canciones actuales           | Amigos activos escuchando música  | Feed actualizado con publicaciones correctas          | Funcionalidad |
| TC006        | Feed social                 | Dar "me gusta" a una canción en el feed    | Usuario autenticado y feed cargado | 1. Ingresar feed; 2. Seleccionar "me gusta" en una publicación                            | Publicación válida               | Contador de "me gusta" incrementa y cambio visual      | Usabilidad    |
| TC007        | Recomendador de usuarios    | Mostrar usuarios con gustos similares       | Usuario autenticado con historial de escucha | 1. Ingresar a sección de recomendaciones; 2. Visualizar lista de usuarios recomendados    | Usuario con historial variado    | Lista muestra usuarios con alta compatibilidad musical | Funcionalidad |
| TC008        | Recomendador musical        | Generar playlist personalizada               | Usuario autenticado y sincronizado | 1. Entrar a recomendador musical; 2. Seleccionar generar playlist personalizada            | Historial de escucha variado     | Playlist generada con canciones relevantes al usuario | Funcionalidad |
| TC009        | Configuración y privacidad  | Cambiar opciones de privacidad               | Usuario autenticado                | 1. Ir a configuración; 2. Cambiar privacidad (ocultar actividad); 3. Guardar cambios      | Configuración inicial pública    | Cambios aplicados, actividad oculta en feed            | Seguridad     |
| TC010        | Logout                     | Cerrar sesión correctamente                   | Usuario autenticado                | 1. Seleccionar logout; 2. Confirmar cierre de sesión                                      | Usuario conectado               | Usuario deslogueado y redirigido a pantalla de login   | Funcionalidad |
| TC011        | Registro de nuevo usuario       | Registro exitoso vía Spotify                         | Usuario no registrado                        | 1. Abrir app; 2. Seleccionar registro con Spotify; 3. Autorizar acceso Spotify                    | Cuenta Spotify nueva                | Usuario creado y perfil sincronizado con datos Spotify        | Funcionalidad |
| TC012        | Registro de nuevo usuario       | Registro fallido sin permiso de Spotify              | Usuario no registrado                        | 1. Abrir app; 2. Seleccionar registro con Spotify; 3. Denegar acceso Spotify                     | Sin permiso                        | Mensaje de error y no creación de usuario                      | Seguridad     |
| TC013        | Recomendador musical            | Explorar playlists por géneros                        | Usuario autenticado y sincronizado          | 1. Acceder recomendador musical; 2. Filtrar por género; 3. Seleccionar playlist                   | Género musical específico          | Playlist relevante aparece según filtro                        | Funcionalidad |
| TC014        | Feed social                    | Comentar una publicación                             | Usuario autenticado y feed activo           | 1. Entrar al feed; 2. Seleccionar publicación; 3. Escribir comentario y enviar                     | Texto comentario válido            | Comentario aparece debajo de la publicación                    | Usabilidad    |
| TC015        | Feed social                    | Comentar con texto vacío                             | Usuario autenticado y feed activo           | 1. Entrar al feed; 2. Seleccionar publicación; 3. Intentar enviar comentario vacío                 | Texto comentario vacío             | Botón deshabilitado o mensaje de error                         | Seguridad     |
| TC016        | Perfil musical personalizado   | Comparar perfil con amigo                            | Usuario autenticado con amigos               | 1. Acceder perfil musical; 2. Seleccionar amigo para comparar perfiles                            | Perfil usuario y amigo             | Muestra comparación clara de artistas, géneros y playlists    | Funcionalidad |
| TC017        | Recomendador de amistades      | Seguir usuario recomendado                           | Usuario autenticado y recomendaciones cargadas | 1. Entrar a recomendador de amistades; 2. Seleccionar usuario; 3. Pulsar "seguir"                | Usuario recomendado válido         | Usuario seguido y aparece en lista de amigos                   | Funcionalidad |
| TC018        | Recomendador de amistades      | Iniciar chat con usuario seguido                     | Usuario autenticado y con usuarios seguidos | 1. Entrar sección mensajes; 2. Seleccionar usuario seguido; 3. Enviar mensaje                     | Texto de mensaje                  | Mensaje enviado y recibido correctamente                       | Funcionalidad |
| TC019        | Configuración y privacidad     | Activar/desactivar notificaciones                     | Usuario autenticado                         | 1. Ir a configuración; 2. Cambiar estado notificaciones; 3. Guardar cambios                       | Estado notificación ON/OFF         | Notificaciones activadas o desactivadas según selección        | Usabilidad    |
| TC020        | Feed social                    | Guardar canción desde feed                            | Usuario autenticado y feed activo           | 1. Entrar al feed; 2. Seleccionar canción en publicación; 3. Pulsar "guardar"                     | Canción válida                    | Canción agregada a lista personal de guardados                 | Funcionalidad |

