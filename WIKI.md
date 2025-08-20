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

