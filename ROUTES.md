# android reac — Screens & Navigation

## How to run
cd project
npm install --legacy-peer-deps && npx expo start
# Press 'a' for Android, 'i' for iOS, 'w' for web, or scan the QR code with Expo Go.

## Screens
| Screen | File | Description |
|--------|------|-------------|
| / | src/screens/PageScreen.tsx | Full-screen WebView of the Xccelera AI Platform Studio sign-in page |
| NotFound | src/screens/NotFoundScreen.tsx | Catch-all "Screen not found" with Go Back |

## Navigation map
- / is the initial screen; the page's links stay plain links inside the HTML.

## Shared components
None in src/components. src/design/page holds DesignPage.tsx (WebView), DesignPage.web.tsx (web preview) and pageHtml.ts.

## Design tokens
primary, background, textPrimary, textInverse (src/theme/colors.ts, used by NotFoundScreen only).
