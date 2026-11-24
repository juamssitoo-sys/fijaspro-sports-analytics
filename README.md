# ⚽ FijasPro — Kinetic Telemetry Sports Analytics Platform

Plataforma moderna de analítica deportiva inteligente, telemetría cuantitativa y modelos predictivos verificados para **Fútbol (UEFA Champions League y Copa Libertadores 2026)**, **NBA** y **Esports**.

---

## 🎨 Especificaciones de Diseño (Kinetic Dark)

Basado en el sistema de diseño oficial `fijaspro_design_system.md`:
* **Fondo Principal:** Grafito oscuro (`#111318`, `#1A1B21`, `#1E2025`, `#282A2F`) para evitar la fatiga visual.
* **Colores de Acento:**
  * **Blaze Coral (`#FFB4A1` / `#FF5628`):** Pasión de estadio, llamadas a la acción e identidad de marca.
  * **Tactical Emerald (`#43FFBB`):** Eventos en vivo, métricas verificadas y alta confianza del modelo.
  * **Cyber Cyan (`#7BD0FF`):** Telemetría táctica, Esports y comparativas.
* **Tipografías:**
  * `Mulish` (Headlines y marcadores)
  * `Instrument Sans` (Lectura y navegación)
  * `Spline Sans Mono` (Números tabulares, xG, porcentajes y telemetría)

---

## 🚀 Despliegue en Vercel

Este proyecto cuenta con `vercel.json` y `package.json` preconfigurados para despliegue instantáneo con **cero configuración adicional**.

### Opción 1: Despliegue con Vercel CLI (desde la terminal)
```bash
# Estando en la carpeta del proyecto:
cd c:\Users\rexxd\Downloads\fijaspro-sports-analytics

# Ejecutar el despliegue a producción:
npx vercel --prod
```

### Opción 2: Despliegue desde GitHub / Vercel Dashboard
1. Sube este directorio a tu repositorio de GitHub (o vincula tu cuenta).
2. Entra a [vercel.com/new](https://vercel.com/new).
3. Selecciona el repositorio e impórtalo. Vercel detectará automáticamente `vercel.json` y desplegará la web en segundos con SSL y CDN global.

### Probar localmente
```bash
npx serve .
# O abrir directamente index.html en cualquier navegador.
```

---

## 📊 Módulos y Funcionalidades Incluidas

1. **Dashboard General (Inicio):**
   * Portada editorial con métricas en vivo.
   * Resumen de la UEFA Champions League (144 partidos, 36 clubes).
   * Destacado de la **Gran Final de Copa Libertadores 2026: SE Palmeiras vs Estudiantes de La Plata**.
2. **Laboratorio de Fútbol:**
   * Comparativa H2H de la Final de Libertadores 2026 (Palmeiras vs Estudiantes LP) con desglose de figuras (**Vitor Roque** vs **Guido Carrillo**), xG, posesión y duelos.
   * Tabla completa de posiciones de la UEFA Champions League.
   * Filtros interactivos por competición.
3. **NBA Telemetry:**
   * Análisis avanzado de posesiones, Pace, True Shooting % y Offensive Rating.
4. **Esports (VALORANT & CS2):**
   * Telemetría de rondas de pistolas, ADR y First Kills.
5. **Modelo Cuantitativo v4.2 & Pronósticos:**
   * Simulador predictivo estocástico (xG Engine) sin cuotas ni sesgo de apuestas.
