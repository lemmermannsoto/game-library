# Game Library Manager 🎮📖

Un sistema de gestión por línea de comandos (CLI) construido en Python para organizar y rastrear el estado de una biblioteca de videojuegos multiplataforma. Diseñado para centralizar títulos distribuidos entre consolas de sobremesa, bibliotecas de PC y sistemas de emulación.

## 🚀 Características Principales

- **Gestión de Estados (Backlog Tracking):** Mantén un control preciso de en qué etapa se encuentra cada juego (`Pendiente/Backlog`, `Jugando`, `Completado`, `Abandonado`).
- **Filtrado Multicriterio:** Busca rápidamente en tu catálogo por plataforma (ej. `PS4`, `PC`, `PPSSPP`, `RetroArch`) o por género (ej. `Soulslike`, `Roguelite`, `Tactical RPG`).
- **Persistencia de Datos:** Utiliza estructuras en formato JSON/CSV para guardar tu progreso localmente de forma segura.

## 🗂️ Estructura del Modelo de Datos (Ejemplo)

El sistema maneja objetos `Juego` instanciados a partir de un archivo de base de datos. Un registro típico luce así:

```json
{
  "titulo": "Hades",
  "genero": "Roguelite",
  "plataforma": "PC",
  "estado": "Jugando"
},
{
  "titulo": "Persona 5 Royal",
  "genero": "RPG",
  "plataforma": "PS4",
  "estado": "Completado"
}