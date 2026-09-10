# Venix (venix-theme)

Demo PWA orientada al disfrute del jugador: contiene una experiencia rápida para "jugar" en el navegador, ganar XP y subir de nivel.

Archivos incluidos:
- index.html (UI responsive + mini-juego Tap Frenzy + XP/levels + confetti + leaderboard local)
- manifest.json
- sw.js
- config.js

Cómo probar local:
1. Clona el repo y cambia a la rama `venix-theme`.
2. Sirve el sitio en localhost (ej: `npx serve .` o Live Server en VSCode).
3. Abre en el navegador en `http://localhost:5000` (o el puerto que use `serve`).

Notas:
- El mini-juego "Tap Frenzy" dura `GAME_SECONDS` (configurable en `config.js`) y otorga XP base + bonus por taps.
- El progreso se guarda en `localStorage` bajo la clave `venix_play_data`.
- El service worker requiere HTTPS o localhost para registrarse.

Siguientes mejoras posibles:
- Integrar API de juegos reales (RAWG) para relleno dinámico.
- Añadir sistema de logros y perfil centralizado.
- Mejorar assets (icons reales, imágenes optimizadas) y añadir analytics.
