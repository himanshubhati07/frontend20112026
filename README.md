# android reac

Shows the Xccelera AI Platform Studio sign-in page (the original HTML, unchanged) full-screen inside a WebView on iOS/Android, and in an iframe-style web component for the Expo web preview.

## Tech stack
React Native (Expo) + TypeScript, React Navigation, react-native-webview.

## Getting started
```
npm install --legacy-peer-deps
cp .env.example .env
npx expo start
```
Scan the QR code with Expo Go, or press w for the web preview.

## Environment variables
See .env.example. No variable is read by the app; the page has no API, mock data or stores.

## Project structure
- src/design/page: the page's HTML (pageHtml.ts) and WebView components, copied unchanged
- src/screens: PageScreen (renders the page), NotFoundScreen
- src/navigation: root stack navigator
- src/theme: colors used by NotFoundScreen

## Known differences
- The page's own scripts are kept and run inside the web view.
- The page is rendered by a WebView, so it is responsive to the device width rather than the 1440px design frame.

## Measured against the uploaded HTML

<!-- design-check:begin -->
- **Content:** all 28 text items, stylesheets, images and scripts of the page are in the project exactly as the page had them (checked by code). <!-- check:fidelity -->
- **Look:** the page at / matches the uploaded HTML 100.0 % (390 px: 100.0 %) (screenshots compared in a browser). <!-- check:visual -->
Behaviour is not compared automatically: clicks, hover and focus states, form submission, and anything that needs a real backend. A difference there is not ruled out by the lines above.
<!-- design-check:end -->
