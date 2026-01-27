# Tokens de Diseño y Reglas CSS/Tailwind

Este documento centraliza los tokens técnicos para la implementación de interfaces Anclora.

## CSS Custom Properties (Variables)

Para uso en proyectos de Vanilla CSS.

```css
:root {
  /* Colors */
  --anclora-gold: #C5A059;
  --anclora-navy: #05070A;
  --anclora-slate: #0A0F14;
  --anclora-white: #FFFFFF;
  
  /* Spacing */
  --spacing-xs: 4px;
  --spacing-sm: 8px;
  --spacing-md: 16px;
  --spacing-lg: 24px;
  --spacing-xl: 32px;
  --spacing-xxl: 48px;
  
  /* Radii */
  --radius-sm: 2px;
  --radius-md: 4px;
  --radius-lg: 8px;
  
  /* Shadows */
  --shadow-luxe: 0 10px 30px rgba(0, 0, 0, 0.5);
  --shadow-gold: 0 4px 20px rgba(197, 160, 89, 0.15);
}
```

## Configuración Tailwind CSS (Extensión)

```javascript
module.exports = {
  theme: {
    extend: {
      colors: {
        anclora: {
          gold: '#C5A059',
          navy: '#05070A',
          slate: '#0A0F14',
        }
      },
      fontFamily: {
        montserrat: ['Montserrat', 'sans-serif'],
        outfit: ['Outfit', 'sans-serif'],
      },
      letterSpacing: {
        'luxury': '0.2em',
      }
    }
  }
}
```

## Reglas de Implementación

1. **Botones**: Deben seguir estrictamente las clases `btn-primary`, `btn-secondary` definidas en el kit de marca.
2. **Tipografía**: Títulos siempre en `Montserrat` con `letter-spacing` amplio (especialmente en el Hero).
3. **Cards**: Fondo `--anclora-slate` con borde sutil `rgba(197, 160, 89, 0.05)`.
4. **Animaciones**: Usar transiciones suaves (`cubic-bezier(0.4, 0, 0.2, 1)`) de 0.3s para estados hover.
