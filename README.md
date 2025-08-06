# 🪟 Fake Window – Justerbar bakgrunn med ansiktssporing

Et lite eksperiment som simulerer en "fake window"-effekt med justerbar bakgrunn, styrt av hvor hodet ditt er foran kameraet.

Prosjektet bruker [face-api.js](https://github.com/justadudewhohacks/face-api.js) for ansiktsdeteksjon og parallax-effekt for å flytte bakgrunnen.

## 🔧 Funksjoner

- Bruker webkamera til å spore hodets posisjon i sanntid
- Dynamisk bakgrunnsbevegelse basert på brukerens bevegelse
- Enkelt å justere parametere som:
  - Deteksjonsfrekvens (FPS)
  - Bevegelsesskala
  - Smooth interpolering (lerping)

## ⚙️ Justerbare innstillinger

Disse kan endres direkte i koden:

```js
const VIDEO_WIDTH = 640;
const VIDEO_HEIGHT = 480;
const MOVEMENT_SCALE = 50;
const DETECTION_FPS = 30;
const USE_LERP = true;
const LERP_SPEED = 0.2;
