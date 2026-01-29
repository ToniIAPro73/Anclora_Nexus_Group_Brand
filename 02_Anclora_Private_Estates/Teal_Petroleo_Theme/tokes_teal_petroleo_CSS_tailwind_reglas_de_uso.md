Tokens CSS (variables)

```css
:root{
  /* Anclora Teal Petróleo — Official */
  --anclora-primary:   #0A3843; /* master brand background */
  --anclora-dark:      #062A33; /* footer / overlays / night */
  --anclora-hover:     #124A50; /* hover / active / accents */
  --anclora-bg:        #0F3F45; /* secondary sections / cards */

  /* Suggested UI helpers */
  --anclora-text:      rgba(255,255,255,.92);
  --anclora-text-muted:rgba(255,255,255,.72);
  --anclora-border:    rgba(255,255,255,.12);
  --anclora-surface:   rgba(255,255,255,.04);
}
```

Tokens Tailwind (theme.extend)

```js
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        anclora: {
          primary: "#0A3843",
          dark: "#062A33",
          hover: "#124A50",
          bg: "#0F3F45",
          // Optional helpers
          text: "rgba(255,255,255,.92)",
          muted: "rgba(255,255,255,.72)",
          border: "rgba(255,255,255,.12)",
          surface: "rgba(255,255,255,.04)",
        },
      },
    },
  },
};
```

Reglas de uso (qué fondo para qué contexto)

1. PRIMARY `#0A3843`: fondo “master”. Logo, hero, portada, páginas clave. Si dudas, usa este.
2. DARK `#062A33`: footer, overlays, modales, secciones de lectura larga en modo “night”.
3. HOVER `#124A50`: hover/active de botones y links, tabs activos, micro-acentos. No usar como fondo principal.
4. BACKGROUND `#0F3F45`: alternancia de secciones, cards grandes, fondos secundarios para dar aire sin salir de marca.

Reglas de oro:

* Mantén el dorado “metalizado” (con volumen). Evita dorado plano chillón.
* No introduzcas verdes saturados; mantente en teal/petróleo para “quiet luxury”.
* Contraste recomendado: texto `rgba(255,255,255,.92)` y secundario `rgba(255,255,255,.72)` sobre estos fondos.
