# Web Roast

Independent React + Vite website based on the supplied Web Roast references.

## Run

npm install
npm run dev -- --port 5194

## Build

npm run build

Output: dist/client (static frontend) plus the included optional Sites worker.

## Included

Home, story, drink menu, category filters, quantity controls, calculated cart totals, pickup/dine-in selection, demo checkout, spaces, journal, and visit views. Responsive layouts and keyboard-accessible native dialogs.

Checkout runs in memory only. It does not process payments, send orders, or persist customer data. Tax is sample UI data. Marketing statistics and address come from the concept reference and are not verified business claims.

Assets: public/assets/hero.png generated with built-in ImageGen using the supplied cup/comic/city art direction. menu-reference.jpg is the supplied reference, displayed within measured product photo bounds. Fonts load from Google Fonts. All project images live in this folder.

## Expanded experience — September 2026

Includes three additional deep-linked pages, new locally stored generated photography, and a real Three.js WebGL product viewer. Drag to orbit, use arrow keys to rotate, change finishes, reveal product layers, pause motion, zoom, and reset the view. Animation respects reduced-motion preferences; a photo fallback is shown when WebGL is unavailable. The models are original procedural design studies, not manufacturing CAD models.

New pages: Brew Lab, Roastery, Brew Guide. New images: cafe, roastery, iced coffee. The brew guide includes an adjustable recipe calculator.

Relative asset paths and hash navigation support GitHub Pages project subpaths. Build with `npm run build`; publish the contents of `dist/client` when ready. These changes have not been deployed by this task.

## Single-page scrolling update

All nine sections stay mounted in one continuous page. Header navigation scrolls to section anchors, highlights the section currently in view, and closes the mobile menu after selection. Existing hash links still open the corresponding section. Reduced-motion preferences disable smooth scrolling.
