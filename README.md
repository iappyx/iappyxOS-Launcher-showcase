# iappyxOS Launcher Showcase

Widgets, wallpapers, page transitions, icon filters, and plugins for [iappyxOS Launcher](https://github.com/iappyx/iappyxOS-Launcher) — a programmable Android home screen.

Everything here is loaded directly from inside the launcher: Settings → Showcase. No copy-paste needed.

## Widgets

Sandboxed HTML widgets that drop into a home-grid cell.

| Widget | Description | Bridges |
|--------|-------------|---------|
| [Clock](widgets/clock/) | The classic clock — time and date, nothing else. | — |
| [Compass](widgets/compass/) | Magnetic compass combining magnetometer and accelerometer for a steady bearing. Offline. | sensor |
| [Live GPS Map](widgets/live-gps-map/) | A small map that follows your GPS in real time; pulsing dot, auto-pan. | location, storage, vibration |
| [Morse Flashlight](widgets/morse-flashlight/) | Type a message; the torch blinks it in Morse code. | torch |
| [QR & Barcode Scanner](widgets/qr-barcode-scanner/) | Scans QR and 1D barcodes through the camera; copies/opens results. | clipboard, intent, storage |
| [Radio Player](widgets/radio-player/) | Internet radio with live logos, podcasts, audio visualizer, and stream metadata. | alarm, audio, httpClient, notification, sensor, storage, vibration |
| [Road Trip NL](widgets/roadtrip-nl/) | Driving companion that announces nearby Dutch locations via TTS. Bundled offline database. | location, screen, sqlite, storage, tts, vibration |
| [Sticky Notes](widgets/sticky-notes/) | Pastel sticky notes on a transparent canvas — drag, archive, restore. | storage, vibration |
| [Water Tracker](widgets/water-tracker/) | Tap a glass to mark it drunk; daily reset; nudge reminders. | alarm, notification, sqlite, vibration |
| [Weather](widgets/weather/) | Current conditions for your GPS location via Open-Meteo. | httpClient, location, storage |
| [AdGuard Stats](widgets/adguard-stats/) | Today's block percentage, total queries, and blocked count for self-hosted AdGuard Home. | plugin: adguard-home |
| [AdGuard Protection Toggle](widgets/adguard-protection-toggle/) | One-tap protection toggle with duration picker; auto-restore countdown. | plugin: adguard-home |
| [AdGuard Top Blocked](widgets/adguard-top-blocked/) | Top blocked domains over a 24h window with proportional bars. | plugin: adguard-home |
| [AdGuard Top Clients](widgets/adguard-top-clients/) | Top DNS clients by query count, 24h window. | plugin: adguard-home |
| [AdGuard Live Queries](widgets/adguard-live-queries/) | Auto-scrolling list of the last 30 DNS queries; filter chip for All/Blocked. | plugin: adguard-home |

## Wallpapers

Programmable HTML wallpapers running in the launcher's `:wallpaper` process.

| Wallpaper | Description |
|-----------|-------------|
| [Bouncing Balls](wallpapers/bouncing-balls/) | Twenty colourful balls bounce around, dodging your icons and widgets in real time. |
| [Cells Flow](wallpapers/cells-flow/) | Animated mosaic of warm orange and cool blue cells, pulsing and shifting. |
| [Chromatic Halo Bloom](wallpapers/chromatic-halo-bloom/) | Each icon and widget gets a glowing halo, all cycling through the spectrum. |
| [Clouds](wallpapers/clouds/) | Drifting 3D clouds with a warm sun. Painterly, calm. |
| [Digital Rain](wallpapers/digital-rain/) | Matrix-style green katakana raining down. Capped at 30fps to stay battery-friendly. |
| [Falling Snow](wallpapers/falling-snow/) | Snowflakes drift downward and pile up; shake to clear. |
| [Fireworks](wallpapers/fireworks/) | Looped fireworks against a black sky. |
| [Hue Drift](wallpapers/hue-drift/) | Slow-drifting radial colour gradient with parallax and tilt response. |
| [Live Map](wallpapers/live-map/) | Interactive map centred on your real-time GPS location. |
| [Live Weather Scenes](wallpapers/live-weather-scenes/) | Real-time weather scenes that change with conditions: sun, clouds, rain, storm, snow, fog. |
| [Magnetic Neon Particles](wallpapers/magnetic-neon-particles/) | Glowing particles that respond to motion — tilt to fling, shake for a burst. |
| [Material Color Drift](wallpapers/material-color-drift/) | Infinite grid of Material Design colour swatches drifting in every direction. |
| [Neon Halo Drift](wallpapers/neon-halo-drift/) | 3D halo of neon particles orbiting through deep dark space. |
| [Neon Web Drift](wallpapers/neon-web-drift/) | Glowing nodes connected by lines, drifting through 3D space; touch ripple. |
| [Rotating Radial Gradient](wallpapers/rotating-radial-gradient/) | A radial rainbow gradient that slowly rotates. |
| [Shake for a Photo](wallpapers/shake-for-a-photo/) | Shake your phone to fetch a new random landscape photo, smooth crossfade. |
| [Waves](wallpapers/waves/) | A calm 3D ocean-wave mesh in deep navy. |

## Page transitions

How home-screen pages move from one to the next.

| Transition | Description |
|------------|-------------|
| [3D Cube](transitions/3d-cube/) | Six home screens form a 3D cube; pages turn around the meeting edge. |
| [Aperture](transitions/aperture/) | Pages contract to a dot in the centre, then bloom back out into the next. |
| [Card Stack](transitions/card-stack/) | Outgoing page lifts and tilts back like a dealer flicking a card. |
| [Carousel](transitions/carousel/) | Pages rotate around their own centres like records on a turntable. |
| [Column Rain](transitions/column-rain/) | Columns drop off the bottom one at a time; new columns drop in from the top. |
| [Depth Stack](transitions/depth-stack/) | Outgoing page recedes (fades and scales down) as the incoming one slides over it. |
| [Dissolve](transitions/dissolve/) | Cells fade out individually in a stochastic speckle, like an old film cut. |
| [Explode](transitions/explode/) | Cells radiate outward from the centre with a spin, then settle into the new page. |
| [Fade](transitions/fade/) | A pure crossfade — no motion at all. |
| [Frosted Blur](transitions/frosted-blur/) | Outgoing page blurs out as the incoming one sharpens into focus. Android 12+. |
| [Horizontal Sweep](transitions/horizontal-sweep/) | The default left/right slide between pages. |
| [Implode & Explode](transitions/implode-explode/) | Cells collapse to the centre, then burst back into new positions. |
| [Scatter](transitions/scatter/) | Each cell flies to its own off-screen point instead of moving as a slab. |
| [Tilt Cascade](transitions/tilt-cascade/) | Horizontal slide with a 3D tilt; reads as a flipping card. |
| [Vertical Fall](transitions/vertical-fall/) | Pages fall up or down between cards instead of sliding sideways. |
| [Zoom-through](transitions/zoom-through/) | Pages zoom out as new ones zoom in. Quick and punchy. |

## Icon filters

Apply a coordinated look to every app icon on every page.

| Icon filter | Description |
|-------------|-------------|
| [Aurora](icon_filters/aurora/) | Holographic cyan→magenta→gold→teal sheen over each icon. |
| [Greyscale](icon_filters/greyscale/) | Pure black-and-white. Minimalist, no tint. |
| [Mono accent](icon_filters/mono-accent/) | Greyscale icons tinted to your system accent (Material You). |
| [Pixelate](icon_filters/pixelate/) | 8-bit retro: icons downsampled to chunky pixels. |
| [Rainbow matrix](icon_filters/rainbow-matrix/) | Greyscale icons tinted by grid position — radial rainbow. |
| [Sepia](icon_filters/sepia/) | Warm brown vintage tones. |
| [Tinted mono](icon_filters/tinted-mono/) | Each icon recoloured with its own dominant colour. |
| [Vintage](icon_filters/vintage/) | Faded saturation with a warm shift — old polaroid feel. |
| [Wallpaper themed](icon_filters/wallpaper-themed/) | Tints sampled from your wallpaper, distributed across the grid. |
| [Sweetheart](icon_filters/sweetheart/) | Heart-shaped icons in soft pink duotone. |
| [Squircle](icon_filters/squircle/) | iOS-style squircle silhouette. |
| [Star](icon_filters/star/) | Five-pointed star silhouette via custom SVG path. |
| [Round](icon_filters/round/) | Circular icons — every app inscribed in a perfect disc. |
| [Hex](icon_filters/hex/) | Hexagonal icons with flat-top orientation. |
| [Hex tiles](icon_filters/hex-tiles/) | Hexagonal icons with subtle film grain. |
| [Round mono](icon_filters/round-mono/) | Circular greyscale icons tinted to your Material You accent. |
| [Cloud](icon_filters/cloud/) | Soft cloud silhouette via custom SVG path. |
| [Shield](icon_filters/shield/) | Heraldic shield silhouette via custom SVG path. |
| [Leaf](icon_filters/leaf/) | Leaf silhouette via custom SVG path. |

## Plugins

Capability-gated bridges to self-hosted and third-party services. Once installed, widgets and wallpapers reach them via `iappyx.plugin('<slug>').*`. Credentials live in encrypted device storage.

| Plugin | Description |
|--------|-------------|
| [Home Assistant](plugins/home-assistant/) | Read entity states, fire services, pull history from a self-hosted Home Assistant. |
| [Immich](plugins/immich/) | Recent/random/album photos from a self-hosted Immich server. |
| [Paperless-ngx](plugins/paperless-ngx/) | Recent scans, full-text search, tag/correspondent filtering for self-hosted Paperless-ngx. |
| [Spotify](plugins/spotify/) | Now playing, queue, recently played, transport controls. OAuth, auto-refreshes. |
| [Microsoft 365](plugins/office365/) | Outlook mail, Calendar, To Do, OneDrive, OneNote, Excel range reads via Microsoft Graph. |
| [Google Workspace](plugins/google-workspace/) | Gmail, Calendar, Drive, Tasks, Sheets range reads. Device-flow OAuth. |
| [GitHub](plugins/github/) | PR queue, notifications, issues, starred repos, contribution heatmap, repo stats. |
| [Philips Hue](plugins/hue/) | Lights, rooms, scenes, sensors. Pure local-network, no cloud, no OAuth. |
| [Unraid](plugins/unraid/) | System stats, Docker containers, parity, VMs, shares (Unraid 7.0+ GraphQL API). |
| [MQTT](plugins/mqtt/) | Generic MQTT 3.1.1 client — TCP, TLS, or WebSocket. Subscribe + publish. |
| [AdGuard Home](plugins/adguard-home/) | Live block stats and one-tap protection toggle for self-hosted AdGuard Home. |

## How to use

1. Open [iappyxOS Launcher](https://github.com/iappyx/iappyxOS-Launcher) on your Android device
2. Settings → Showcase
3. Pick a category (widgets, wallpapers, transitions, icon filters, plugins)
4. Tap an entry → preview → install

Everything here is also browsable directly: each folder contains the source HTML/JSON, ready to read or copy by hand.

## Submit your own

Have a widget, wallpaper, transition, icon filter, or plugin to share? Submit it:

1. Fork this repo
2. Add a folder under the matching category with the files listed below
3. Add a new entry to `showcase.json` (under the matching array)
4. Open a PR

### Folder structure per type

```
widgets/your-widget/
├── widget.html          # the widget source
└── meta.json            # title, description, author, bridges, uses

wallpapers/your-wallpaper/
├── wallpaper.html       # the wallpaper source
└── meta.json

transitions/your-transition/
├── spec.json            # the transition keyframes / cell choreography
└── meta.json

icon_filters/your-filter/
├── spec.json            # the filter recipe (CSS filter, SVG shape, tint, …)
└── meta.json

plugins/your-plugin/
├── plugin.html          # the plugin runtime (handles iappyx.plugin('slug') calls)
├── settings.html        # the settings UI shown inside the plugin sandbox
├── manifest.json        # declared capabilities, hostname allow-list, methods
└── meta.json            # title, description, author, aiPrompt
```

### meta.json format

```json
{
  "title": "Your thing",
  "description": "Short description of what it does.",
  "author": "your-github-username",
  "bridges": ["sensor", "storage"],
  "uses": ["Optional: libraries or sources, e.g. Three.js (MIT) or iappyxOS plugin: home-assistant"],
  "added": "2026-06-04"
}
```

### showcase.json

Every new entry **must** also be added to its category array in `showcase.json`. The launcher reads this file as the index — a folder alone is invisible on-device.

## License

MIT — see [LICENSE](LICENSE). Individual third-party libraries used by entries (Leaflet, Three.js, Vanta.js, OpenStreetMap tiles, Open-Meteo, …) keep their own licenses; check each entry's `uses` field.
