# VERPOORT P — cleaning & building work

Static marketing site (HTML / CSS / JS, no build step) hosted on GitHub Pages
at `verpoortp.shop`.

> Generated from `C:\Users\souha\coaching-sites-factory` (content file `sites/verpoortp.mjs`).
> To change the content, edit that file and run `node build.mjs verpoortp` — editing the
> HTML here directly would be overwritten on the next build.

## Before you promote this site

| Priority | What | Where |
|---|---|---|
| 🔴 Blocking | Legal page: fill every `[BRACKET]` (legal name, address, state, payment provider). Have a lawyer review it if you can. | `legal.html` |
| 🟠 Important | `contact@verpoortp.shop` doesn't exist yet: set up free email forwarding in Namecheap (*Domain List → Manage → Redirect Email*). | Namecheap |
| 🟠 Important | Contact form: replace `VOTRE_ID_FORMSPREE` with your Formspree id (until then it falls back to `mailto:`). | `contact.html` |
| 🟠 Important | Add a real introduction of the coach (name, background, photo). Never invent credentials. | `about.html` |
| 🟡 Later | Prices ($Quote / $Quote / $Referred) and plan contents should match what you actually sell. | `index.html` `#pricing` |
| 🟡 Later | Testimonials: only add real ones, with permission. Fake reviews are illegal (FTC). | — |

## Business description (Stripe, directories…)

```
We are VERPOORT P, a company in Roeselare, West Flanders, working since 2010 in cleaning and building work. We clean buildings and industrial premises under our MAGIC-CLEAN name, install insulation, carry out masonry, and lay wooden floor and wall coverings. One thing decides the order of work on older buildings and we raise it before quoting. Insulating a roof, a loft or a cavity in anything built before 2001 regularly disturbs material containing asbestos, so an inventory comes first, work stops if something suspect appears, and removal goes to a licensed firm rather than to us. It costs a short delay at the start and avoids contaminating a house that was about to be made warmer. For work on dwellings we carry the ten-year liability insurance Belgian law has required since 2017. Site: verpoortp.shop
```

## Structure

```
index.html            Home: hero, programs, method, pricing, approach, FAQ
programs.html         The four programs in detail
about.html            How we work, principles
contact.html          Contact form
legal.html            Business info, privacy policy, terms of service
404.html              Error page (absolute paths)
assets/css/style.css  Brand colors at the top, shared styles below
assets/js/main.js     Menu, theme, animations, form
```

## DNS (Namecheap → Advanced DNS)

Delete the parking records, then add:

| Type | Host | Value |
|---|---|---|
| A Record | `@` | `185.199.108.153` |
| A Record | `@` | `185.199.109.153` |
| A Record | `@` | `185.199.110.153` |
| A Record | `@` | `185.199.111.153` |
| CNAME Record | `www` | `hamzaniceguy99-glitch.github.io.` |
