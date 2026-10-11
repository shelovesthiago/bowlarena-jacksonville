# Bowl Arena of Jacksonville

A responsive, multipage website concept for Bowl Arena of Jacksonville, 433 Western Blvd., Jacksonville, NC 28546.

Static HTML and CSS only. No framework, no build step and no backend.

## Pages

| File | Contents |
|---|---|
| `index.html` | Homepage: hero, quick facts, feature cards, price snapshot, food preview, visit policies and hours |
| `bowling.html` | Open-bowling and hourly rates, shoes and socks, Thunder Alley, reservation policies, league summary |
| `leagues.html` | Adult winter and summer leagues, league formats, youth Saturday schedule |
| `parties.html` | Birthday party times, deposit, itinerary and party policies |
| `food-arcade.html` | Snack-bar highlights, full menu image, bar note, arcade and prize counter |
| `pro-shop.html` | Products, drilling and ball-service pricing |
| `about.html` | Business history, contact information, hours and directions |

## Shared files

```text
styles.css                        Styling and responsive layout for every page
assets/
├── bowl-arena-logo.png           Business logo (transparent PNG)
├── bowling-action-original.jpg   Hero image
├── favicon.png                   Browser tab icon
└── snack-bar-menu-original.jpg   Full snack-bar menu
```

HTML files and `styles.css` stay in the repository root. Images go in `assets/`.

## Navigation

- Every page uses the same header and footer.
- Desktop (wider than 1100px): Home, Bowling, Leagues, Parties, Food & Arcade, Pro Shop, About, plus a Call Now button.
- 1100px and narrower: the links collapse into a ☰ Menu dropdown built with a native HTML `<details>` element. No JavaScript.
- The current page's link carries `aria-current="page"` in both the desktop nav and the mobile menu. If you add a page, add it to the header and footer on every page.

## Colors

Set at the top of `styles.css`. Matched to the official logo.

```css
--ink:   #081124;
--navy:  #0b1832;
--blue:  #1f718a;  /* dark teal from the logo */
--teal:  #a5d2e6;  /* light blue from the logo */
--cream: #f3f0e8;
--paper: #fbfaf7;
--muted: #697183;
--line:  #d8d8d3;
```

## Deployment

The repository is connected to Vercel. Committing a change to GitHub triggers a new deployment automatically. After it finishes, hard-refresh the browser (Ctrl+Shift+R) to see the update.

The site can also be hosted on Cloudflare Pages, Netlify, GitHub Pages or traditional web hosting by serving the repository root.

## Before official launch

- Confirm all prices, hours, league schedules, reservation terms, menu items and policies with Bowl Arena management.
- Confirm birthday-party package inclusions and Pro Shop service prices.
- Replace or add photographs with business-owned photos of parties, the arcade and the Pro Shop.
- Obtain permission to use the business's branding and photographs.
- Transfer the Vercel project to the owner's account and connect the owner's domain after approval.
