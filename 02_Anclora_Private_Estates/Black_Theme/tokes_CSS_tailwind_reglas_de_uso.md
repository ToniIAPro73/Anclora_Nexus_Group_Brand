Tokens CSS (variables)

```css
:root{
  /* Anclora Dark-Neutral (from logo backgrounds) */
  --anclora-primary:    #343433; /* main dark gray */
  --anclora-dark:       #020201; /* near-black (visual black) */
  --anclora-hover:      #3D3D3C; /* hover / elevated surface */
  --anclora-background: #262625; /* secondary background */

  /* Optional UI helpers */
  --anclora-text:       rgba(255,255,255,.92);
  --anclora-text-muted: rgba(255,255,255,.70);
  --anclora-border:     rgba(255,255,255,.12);
  --anclora-surface:    rgba(255,255,255,.04);
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
          primary: "#343433",
          dark: "#020201",
          hover: "#3D3D3C",
          background: "#262625",
          // Optional helpers
          text: "rgba(255,255,255,.92)",
          muted: "rgba(255,255,255,.70)",
          border: "rgba(255,255,255,.12)",
          surface: "rgba(255,255,255,.04)",
        },
      },
    },
  },
};
```

Reglas de uso (qué fondo para qué contexto)

1. PRIMARY `#343433`: fondo principal “premium dark” para UI y páginas de lectura. Menos agresivo que negro.
2. DARK `#020201`: branding de alto impacto (logo, hero, portadas, splash). Máximo contraste con el dorado.
3. HOVER `#3D3D3C`: hover/active, cards elevadas, estados seleccionados. No usar como fondo base de página.
4. BACKGROUND `#262625`: fondo secundario para alternar secciones, panels, layout largo sin fatiga visual.

Reglas de oro:

* Mantén el dorado metalizado; estos fondos están pensados para que el oro domine.
* Evita grises con tinte azul o marrón: rompe neutralidad y ensucia el dorado.
* Texto recomendado sobre estos fondos: principal 90–95% blanco; secundario 65–75% blanco.
