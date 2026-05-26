# Voltrox Athletics — Proyecto Web

## Qué es
Landing page de una sola página para **Voltrox Athletics**, el negocio de coaching deportivo online de **Nehemias Bou Sleiman** (@nemybousleiman). Vende planes de entrenamiento y asesoría personalizada, 100% online.

## Stack
- Un único archivo `index.html` con CSS y JS inline (sin frameworks, sin build tools)
- Fuentes: Barlow Condensed, JetBrains Mono, Manrope (Google Fonts)
- Deploy: Vercel (auto-deploy en cada `git push`)

## Cuentas y accesos
- **GitHub:** Luche77 / repo: `voltrox-web`
- **Vercel:** cuenta `lucasdetorro` / proyecto `voltrox-web`
- **URL producción:** https://voltrox-athletics.vercel.app

## Deploy workflow
```
Editar index.html → git add . → git commit -m "mensaje" → git push → Vercel despliega solo
```

## Design tokens
| Token | Valor |
|---|---|
| Fondo | `#0A0A0A` |
| Naranja | `#FF5500` |
| Texto | `#F0EDE8` |
| Fuente display | Barlow Condensed 800 |
| Fuente mono | JetBrains Mono |
| Fuente body | Manrope |

## Secciones del sitio
1. **Nav** — Logo + links + CTA "Empezá hoy" (sticky, blur backdrop)
2. **Hero** (`#inicio`) — Título animado, slogan, intro, botón "Ver Programas"
3. **Sobre mí** (`#sobre-mi`) — Foto `perfil.jpeg`, bio, stats
4. **Programas** (`#programas`) — Cards de planes + sección "Cómo funciona"
5. **Nutrición** (`#nutricion`) — 3 cards: Volumen, Definición, Mantenimiento
6. **Contacto** (`#contacto`) — Botones sociales + formulario prefillable
7. **Footer** — Copyright

## Planes actuales y precios
| Plan | Precio |
|---|---|
| Asesoría 1 a 1 (12 semanas) | $360.000 |
| Hipertrofia x2 por semana | $27.500 |
| Hipertrofia x3 por semana | $30.000 |
| Hipertrofia x4 por semana | $35.000 |
| Hipertrofia x5 por semana | $39.000 |
| Hipertrofia x6 por semana | $45.000 (antes $55.000) |

Todos los planes de Hipertrofia incluyen: rutina PDF completa, videos de técnica, progresión estructurada. Son unisex (hombre y mujer). La Asesoría 1 a 1 incluye además llamadas semanales, plan nutricional y chat directo.

## Contacto del coach
- **WhatsApp:** +5492477618128 → `https://wa.me/5492477618128`
- **Instagram:** @nemybousleiman → `https://www.instagram.com/nemybousleiman/`

## Imágenes
- `perfil.jpeg` — Foto de Nehemias en el gym, usada en la sección "Sobre mí"
- Placeholders en cards de planes (espacio para foto del coach, a agregar)

## Stats en "Sobre mí"
- 3 Años de Experiencia
- 100% Online

## Notas de desarrollo
- El formulario de contacto prefillea el campo "mensaje" y "objetivo" según el plan clickeado (JS inline al final del HTML)
- Las animaciones de reveal usan `IntersectionObserver`
- El nav se marca como "scrolled" a partir de 30px de scroll
- Responsive breakpoints: 980px y 560px
