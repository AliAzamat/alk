# SEO Agency Landing Page (Vue 3)

**A component-based landing page for a website-promotion (SEO) agency, built with Vue 3 and Vue CLI: a hero section, a pricing calculator with a range slider, rate breakdowns, an application form, reviews, tariff cards, a portfolio, and a multi-column footer.** The content is in Russian.

`App.vue` mounts the header and `src/views/Home.vue`, which assembles the page from self-contained section components, with a small set of reusable UI primitives shared across them.

## Sections

| Section | Component | Contents |
|---|---|---|
| Header | `Header/` | Logo, navigation, services menu, contacts |
| Hero | `Home.vue` | Headline over a hero image |
| Calculator | `Calculator/` | Filters, a "site is already being promoted" toggle, a price slider (0–28,000 ₽/month) that updates the displayed price live, and a three-month promotion plan list |
| Rates | `Rates/` | Analysis, content, keyword, and marks breakdowns |
| Application form | `ApplyForm/` | Contact inputs with consent checkbox |
| Reviews, Tariffs, Portfolio | `Reviews/`, `Tariffs/`, `Portfolio/` | Card lists rendered from component data |
| Footer | `Footer/` | Logo, link columns, bottom bar |

Reusable primitives: `TagH` (renders `h1`–`h6` from a `type` prop so heading level and styling are decoupled), `Button`, `Input`, `Checkbox`, `Slider`, `Dropdown`.

## Running

Requires Node.js. Vue CLI 4 uses webpack 4, which needs the legacy OpenSSL provider on Node 17 and newer:

```bash
git clone https://github.com/AliAzamat/alk.git
cd alk
npm ci

export NODE_OPTIONS=--openssl-legacy-provider   # Node 17+ only
npm run serve      # development server
npm run build      # production build to dist/ (verified to compile)
```

## Limitations

- It's a static front end: the application form and the calculator's "Calculate" button don't submit anywhere.
- The package is still named `sergey` from the original scaffold, and the portfolio uses placeholder entries.
