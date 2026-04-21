# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Proyecto

Sitio web estático de **Tostaduría Orocafé, El Paraíso** — un sitio informativo/marketing de una empresa tostadora de café en El Paraíso, Honduras.

## Desarrollo local

No hay herramientas de build ni dependencias. Para ver el sitio localmente, basta con abrir `index.html` en un navegador o usar cualquier servidor HTTP simple:

```bash
python -m http.server 8000
# o
npx serve .
```

## Arquitectura

Todo el sitio vive en un único archivo `index.html`. El CSS está embebido en `<style>` dentro del `<head>` y no hay JavaScript propio. Las imágenes se almacenan en `img/`.

**Secciones del sitio (anclas de navegación):**
- `#servicios` — Servicios ofrecidos
- `#proceso` — Proceso del café
- `#tipos` — Variedades de café
- `#vida` — Ciclo de vida del cafeto
- `#preparacion` — Métodos de preparación
- `#ubicacion` — Mapa y dirección

**Integraciones externas:**
- Botón "Ingresar al Sistema" apunta a un Google Apps Script (sistema de pedidos/administración).
- Sección de ubicación usa un `<iframe>` embebido de Google Maps.

## Paleta de colores

| Token | Valor | Uso |
|-------|-------|-----|
| Marrón oscuro | `#3e2c20` | Encabezados, footer |
| Marrón medio | `#59412d` | Fondo del nav |
| Naranja café | `#d2691e` | Botones, acentos |
| Crema | `#fffaf5` | Fondo general |
