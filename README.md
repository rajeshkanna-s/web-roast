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
