# Design QA — Web Roast

Source visual truth: supplied 3959981496316230538_31582183788_jpg.jpg (home), 3959981496106513453_31582183788_jpg.jpg (menu), plus story and design-system references in the user brief.
Implementation evidence: qa/desktop.png and qa/mobile-menu.png. Browser: Codex in-app browser.
Reference size: 1440 × 1799. Desktop CSS target: 1440 × 1100; mobile: 390 × 844. Browser captures use its reported viewport density; portrait reference composition was adapted into a scrolling responsive site, not stretched into the screen. Comparison is regional, not a pixel-difference assertion.
State: home, menu, pastry filter, populated cart, checkout, success, mobile navigation.

## Findings and comparison history
- Initial headline was too small. Increased its responsive scale while retaining the black/red four-line hierarchy; inspected the revised desktop and mobile captures.
- Initial pastry photographs included baked-in captions. Restricted photograph bounds with row-specific aspect ratios and positions; verified four clean pastry cards on mobile.
- Mobile menu headline wrapped the ampersand onto a third line. Reduced menu headline size at the narrow breakpoint and recaptured.
- Full hero/reference images were presented together in the browser review. Focused menu and mobile captures checked readable text and controls.

## Fidelity surfaces
- Typography: Montserrat body with heavy italic Barlow Condensed display; the latter approximates the reference's condensed display face rather than reproducing its distressed texture.
- Spacing: left copy/right cup desktop layout, stacked mobile, product grid and separate order panel. Mobile cart stacks below products.
- Colors: cream #fff3e3, red #e50914, blue #0a3d8f.
- Imagery: generated branded cup/splash/city hero plus supplied product photographs. Hero image is regenerated, not identical. Organic image-to-background boundaries, web logo mark, avatars, and illustrated craft cards remain simplified relative to the concept board.
- Copy: primary headlines, brand story, products, prices and principal calls to action retained. Secondary views use coherent concept copy.

## Interaction checks
- Navigation and mobile menu operate.
- Pastries filter shows four products.
- Hero Roast plus Web Cookie: subtotal $7.20, sample tax $0.64, total $7.84.
- Checkout accepts a name, completes demo confirmation, and clears the cart.
- Empty cart disables checkout. Native dialog focus and close buttons work.
- No horizontal overflow at the tested 390px viewport. No captured console errors.

## Scope and remaining differences
This passes as a functional responsive interpretation, not a pixel-exact recreation. Decorative differences above are retained as follow-up fidelity work. No real orders, payments, backend or persistence.

final result: passed

## Expansion verification

Production build passed. All four existing packaging/worker tests passed. Production CSS image paths resolve to existing files without root-relative URLs. Browser inspection confirmed a rendered WebGL model and no console errors. Material and exploded-view controls were exercised. Coffee studio and Solara collection were checked at 390px with no horizontal overflow; Solara new-expression filtering correctly shows three distinct watches. This verifies the local implementation; hosted GitHub Pages was not redeployed or rechecked.

## Single-page / live-time verification — 2026-09-08

Both production builds and all eight existing worker/packaging checks passed. Both pages expose nine mounted scroll sections. Mobile coffee navigation to Drinks closes the menu, highlights Drinks, and positions the section 95px below the viewport top. No horizontal overflow at 390px. Browser console checks returned no errors on the updated previews.
