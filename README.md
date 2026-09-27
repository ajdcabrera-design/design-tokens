# design-tokens

Shared color, type, radius, and spacing for the portfolio and UX Atlas. Edit `tokens.css` and `DESIGN.md` here. Those two files carry the same values.

## Use it in a site

```bash
npm install github:ajdcabrera-design/design-tokens
```

In the site stylesheet, after Tailwind:

```css
@import "tailwindcss";
@import "design-tokens/tokens.css";
```

Leave component specs and page rules in the product repo.
