# Project 07: Clone Blinkit's Homepage Layout Using Bootstrap

**Program:** WSJP-131 | Full Stack Mentorship Program with DSA & GenAI
**Module:** 07 - Advanced DOM & Browser Features

A responsive grocery-delivery homepage built with **HTML5 + Bootstrap 5** only.
No custom CSS file and no `<style>` tag is used. All styling comes from Bootstrap classes and utilities.

> This is a student practice project. It is not the real Blinkit website, and all images are simple emoji-based graphics created for this project.

---

## How to run

1. Unzip the folder.
2. Open `index.html` in any browser (Chrome, Edge, Firefox).
3. Internet is needed once, because Bootstrap 5 is linked via CDN.

## Folder structure

```
blinkit-clone/
├── index.html
├── README.md
├── screenshots/
│   ├── desktop.png
│   ├── tablet.png
│   └── mobile.png
└── assets/
    ├── banners/      (3 hero slides + 3 promo banners)
    ├── categories/   (20 category images)
    └── products/     (12 product images)
```

---

## 1. Breakdown of key sections built

| # | Section | What it contains |
|---|---------|------------------|
| 1 | **Navbar** (top) | Brand name, delivery info, search box, Login link, Cart button. Collapses into a hamburger menu on small screens. Sticks to the top while scrolling. |
| 2 | **Hero / banner** | Auto-playing Bootstrap carousel with 3 slides, arrows and indicators. |
| 3 | **Promo banners** | Three offer banners side by side on tablet/desktop, stacked on mobile. |
| 4 | **Product category grid** | 20 category tiles (image + name). 3 per row on mobile, 4 on small, 5 on medium, 6 on large screens. |
| 5 | **Product cards** | Two rows of product cards (image, 10 MINS badge, name, weight, price, ADD button). 2 per row on mobile, 3 on tablet, 6 on desktop. |
| 6 | **Informational sections** | "Why choose us?" with 3 cards, and a "Get the app" strip that opens a modal. |
| 7 | **Footer layout** | 4-column dark footer: about text, useful links, categories, social buttons, plus copyright line. |

**Mobile-first approach:** every grid starts with the mobile layout (`col-12`, `row-cols-2`, `row-cols-3`) and adds `sm`, `md`, `lg` classes for bigger screens.

---

## 2. Bootstrap classes / components used

**Layout & grid**
`container`, `row`, `col`, `col-12`, `col-md-4`, `col-md-8`, `col-6`, `col-md-2`, `col-md-3`, `row-cols-2`, `row-cols-3`, `row-cols-sm-4`, `row-cols-md-3`, `row-cols-md-5`, `row-cols-lg-6`, `g-3`, `g-4`

**Components**
- **Navbar:** `navbar`, `navbar-expand-lg`, `navbar-brand`, `navbar-toggler`, `navbar-collapse`, `navbar-nav`, `nav-item`, `nav-link`, `sticky-top`
- **Carousel:** `carousel`, `slide`, `carousel-inner`, `carousel-item`, `carousel-indicators`, `carousel-control-prev`, `carousel-control-next`
- **Cards:** `card`, `card-img-top`, `card-body`, `card-title`, `card-text`, `card-footer`
- **Modal:** `modal`, `modal-dialog`, `modal-content`, `modal-header`, `modal-body`, `modal-footer`, `btn-close`
- **Buttons / forms / badges:** `btn`, `btn-success`, `btn-outline-success`, `btn-outline-light`, `btn-sm`, `btn-lg`, `form-control`, `form-label`, `input-group`, `input-group-text`, `badge`, `text-bg-light`

**Utilities**
- Spacing: `m-*`, `my-*`, `mx-*`, `mb-*`, `mt-*`, `p-*`, `py-*`, `pt-*`, `pb-*`, `ps-*`, `gap-*`
- Typography: `fw-bold`, `fw-semibold`, `fs-3`, `h4`, `h5`, `h6`, `display-4`, `small`, `text-center`, `text-muted`, `text-secondary`, `text-success`, `text-dark`, `text-light`, `text-decoration-none`
- Color & borders: `bg-white`, `bg-light`, `bg-dark`, `bg-success`, `bg-opacity-10`, `border`, `border-0`, `border-bottom`, `border-start`, `rounded-4`, `rounded-5`, `shadow-sm`
- Flexbox & display: `d-flex`, `d-block`, `flex-wrap`, `flex-grow-1`, `justify-content-between`, `align-items-center`, `align-items-lg-center`, `h-100`, `w-100`, `list-unstyled`
- Images: `img-fluid`

**JavaScript:** Bootstrap 5 bundle (CDN) powers the navbar toggle, carousel and modal. No custom JavaScript was written.

---

## 3. Screenshots

| Desktop (1366px) | Tablet (820px) | Mobile (390px) |
|---|---|---|
| ![Desktop](screenshots/desktop.png) | ![Tablet](screenshots/tablet.png) | ![Mobile](screenshots/mobile.png) |

---

## Checklist against the evaluation criteria

- [x] Fidelity to the homepage structure: navbar, hero, banners, category grid, product rows, info sections, footer
- [x] Correct Bootstrap components and grid layout
- [x] Responsive on desktop, tablet and mobile
- [x] Clean, readable, indented code with comments for each section
- [x] Bonus: Bootstrap cards, carousel and modal included
