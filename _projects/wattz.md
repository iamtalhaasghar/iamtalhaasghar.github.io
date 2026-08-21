---
layout: page
title: Wattz
description: an offline-first Android app for tracking household electricity consumption, meter readings, and estimated billing
img: assets/img/wattz/app_icon.png
importance: 1
category: personal
---

<div class="text-center">    
    <p class="lead">Understand your electricity usage. Track every reading. Stay in control.</p>
    <p>A thoughtfully designed Android utility for households that want clear, actionable insight into their electricity consumption — no account, no cloud, no internet required.</p>
</div>

<nav class="mt-4 mb-2">
<ul style="list-style: none; padding-left: 0; display: flex; flex-wrap: wrap; gap: 0.25rem 1rem;">
    <li><a href="#the-problem">The Problem</a></li>
    <li><a href="#the-solution">The Solution</a></li>
    <li><a href="#product-showcase">Product Showcase</a></li>
    <li><a href="#key-features">Key Features</a></li>
    <li><a href="#ocr-meter-scanning">OCR Meter Scanning</a></li>
    <li><a href="#analytics">Analytics</a></li>
    <li><a href="#offline-first-architecture">Offline-First</a></li>
    <li><a href="#design-system">Design System</a></li>
    <li><a href="#tech-stack">Tech Stack</a></li>
    <li><a href="#challenges--learnings">Challenges</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#beta-download">Beta</a></li>
    <li><a href="#suggestions">Suggestions</a></li>
</ul>
</nav>

---

## The Problem {#the-problem}

Most households have an electricity meter but no easy way to track usage over time. Paper logs get lost, mental estimates are unreliable, and utility bills arrive too late to change behavior. People want to understand their consumption, but the tools available are either too complex (enterprise energy dashboards) or too simple (basic calculator apps that don't persist data).

The result: electricity usage stays a black box until the bill arrives.

---

## The Solution {#the-solution}

Wattz turns your phone into a personal electricity tracker. Record readings by typing them in or scanning your meter with the camera — the app handles the rest. It calculates consumption between readings, estimates your monthly bill, and visualizes your usage trends so patterns are impossible to miss.

Everything runs locally on your device. No signup. No data leaving your phone.

---

## Product Showcase {#product-showcase}

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/home.png" title="Home Dashboard" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/analytics.png" title="Usage Analytics" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/history.png" title="Reading History" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Home dashboard showing current usage, estimated bill, and monthly goal progress. Analytics with daily, weekly, and monthly consumption trends. Reading history with a searchable log of every meter reading.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/add-reading.png" title="Add Reading" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/billing-cycle.png" title="Billing Cycle" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/monthly-goal-drum-roll.png" title="Monthly Goal" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Meter reading with camera scanning and manual entry. Estimated billing breakdown by cycle. Monthly usage goal tracking with visual progress.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/settings.png" title="Settings" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/themes.png" title="Themes" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/onboarding.png" title="Onboarding" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Rate tier configuration and data management. Light and dark theme support. Guided onboarding flow.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/backup-options.png" title="Backup Options" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/multiple-reminders.png" title="Reminders" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
    </div>
</div>
<div class="caption">
    Database export and import for device migration. Multiple configurable reminders for scheduled readings.
</div>

---

## Key Features {#key-features}

- **Camera Meter Scanning** — Point your phone at the meter. On-device OCR reads the digits automatically.
- **Manual Readings** — Type readings by hand with validation and automatic unit calculation.
- **Consumption Tracking** — Units consumed between any two readings, broken down by day and month.
- **Analytics Dashboard** — Interactive charts showing usage trends, peak periods, and month-over-month comparisons.
- **Estimated Billing** — Configure your rate tier and get projected costs from actual consumption data.
- **Usage Goals** — Set a monthly target and track progress with a visual indicator on the home screen.
- **Reading History** — Searchable, chronological log of every reading with CSV export.
- **Reminders** — Configurable notifications so you never miss a scheduled reading.
- **Dark Mode** — Full light and dark theme support.
- **Themes** — 8 color themes (Default, Electric Blue, Emerald, Amethyst, Sunset, Rose, Teal, Ocean) with light and dark mode support. Switch instantly from Settings.
- **Offline-First** — All data stored locally. No account, no cloud, no internet required.
- **Data Backup & Restore** — Export and import your full database for device migration or safekeeping.

---

## OCR Meter Scanning {#ocr-meter-scanning}

The standout feature. Wattz uses Google's ML Kit to recognize digits directly from your meter's display — no manual transcription, no room for error.

Recognition runs entirely on-device in under 200ms. There's no image upload, no API call, no server involved. The scan happens the moment you point the camera, and the result appears pre-filled in the reading dialog — ready to confirm or correct.

The challenge wasn't OCR accuracy (ML Kit handles printed digits well). It was designing a capture flow that guides users to hold the camera steady, frame the meter correctly, and handle varying lighting conditions. The solution: a real-time preview with framing hints and automatic edge detection that locks onto the meter display.

---

## Analytics {#analytics}

Wattz doesn't just store numbers — it makes them meaningful.

The analytics screen provides:

- **Daily, weekly, and monthly** consumption breakdowns with interactive chart views
- **Month-over-month comparisons** to spot trends and seasonal patterns
- **Peak usage identification** — see which periods consume the most energy
- **Average daily usage** calculated automatically from your reading history

All analytics are computed locally from your stored readings. The charts use React Native SVG for smooth rendering, and the data updates instantly as new readings are added.

---

## Offline-First Architecture {#offline-first-architecture}

Wattz has no backend. No API. No cloud sync. Every byte of data lives in a local SQLite database on your device.

This was a deliberate architectural decision, not a limitation:

- **Privacy** — Your electricity usage never leaves your phone. There's no account to create, no data to breach.
- **Reliability** — No network dependency means the app works everywhere — underground parking, rural areas, airplane mode.
- **Speed** — Local queries return in milliseconds. There's no loading state, no spinner, no "connecting to server."
- **Simplicity** — No authentication flows, no token management, no sync conflicts.

The tradeoff is that data doesn't sync across devices. For a personal utility like electricity tracking, that's an acceptable compromise — and one that keeps the app radically simple to use and maintain.

---

## Design System {#design-system}

Wattz follows Material Design 3 with one guiding principle: **make electricity data scannable in under two seconds.**

**Color.** The palette is intentionally restrained. **Wattz Yellow (#FFC107)** is the only high-chroma color, reserved for active states and primary actions. Everything else uses neutral surfaces and grays, which means the yellow always draws the eye exactly where it matters.

**Typography.** Inter handles all text. Large consumption numbers use tight letter-spacing to feel precise. Body text uses standard line-height for readability in data-heavy list views.

**Depth.** Layering uses tonal surfaces and soft ambient shadows instead of borders. The result is an interface that feels structured and hierarchical without visual clutter.

**Components.** Rounded cards, pill-shaped buttons, thick progress bars with fully rounded caps. Every touch target meets accessibility minimums. The UI is designed to feel more like a well-built utility than a traditional data dashboard.

---

## Tech Stack {#tech-stack}

| Component | Choice | Rationale |
|-----------|--------|-----------|
| Framework | React Native 0.85 + Expo SDK 56 | Native Android performance with cross-platform codebase |
| Language | TypeScript | Type safety across navigation, database schemas, and components |
| Styling | NativeWind | Tailwind-style utilities compiled at build time — zero runtime cost |
| Database | expo-sqlite | Local-first SQL storage with no cloud dependency |
| OCR | expo-mlkit-ocr | On-device text recognition; no API calls, no latency |
| Navigation | Expo Router | File-based routing with compile-time typed routes |
| Animations | React Native Reanimated 4 | Thread-safe animations that never block the JS thread |
| Notifications | expo-notifications | Local scheduling for reading reminders without a backend |
| Icons | @expo/vector-icons + FontAwesome | Consistent iconography across the app |

---

## Challenges & Learnings {#challenges--learnings}

**Information hierarchy is the real design challenge.** The hardest part of Wattz wasn't computing consumption — it was deciding which numbers belong on the home screen and which should live one tap away. The solution: one large number (current usage), one progress indicator (monthly goal), and a clear visual path to everything else.

**Offline-first simplifies and complicates.** No server means no sync conflicts, no loading spinners, and no auth flows. But it also means the database schema has to be right from the start — SQLite migrations are the only option when there's no backend to patch.

**On-device OCR is practical sooner than expected.** ML Kit processes meter images in under 200ms on modern Android devices. The real challenge was UX, not ML — designing a capture flow that guides users to hold the camera steady and frame the meter correctly under varying lighting.

**Material Design 3's tonal palette does more than it appears.** The surface color system creates a layered, depth-aware interface without borders or heavy shadows. It's a subtle difference that elevates the app beyond typical utility toolkits.

**Every feature needed a "why."** Usage goals, estimated billing, reminders — each had to justify its presence by solving a real user problem, not just filling screen space. The result is a focused app that does fewer things well rather than many things adequately.

---

## Roadmap {#roadmap}

Features planned for upcoming releases:

- **Multi-tariff support** — Different rate tiers for peak/off-peak hours with automatic cost calculation
- **Widget support** — Home screen widget showing current month usage and estimated bill at a glance
- **Bill photo attachment** — Attach a photo of your utility bill to each reading for reference
- **Household profiles** — Track multiple meters or compare usage across household members
- **Smart insights** — Automated detection of unusual consumption spikes with plain-language explanations

---

## Beta Download {#beta-download}

Wattz is currently in beta and not yet published on the Play Store.

<div class="text-center mt-4 mb-4">
    <a id="wattz-latest-download" class="btn btn-primary btn-lg" href="#" target="_blank">
        Download Latest Beta
    </a>
    <p id="wattz-version-info" class="mt-2" style="opacity: 0.7;"></p>
</div>

Install the APK on your Android device. You'll need to enable "Install from unknown sources" in your device settings.

**Package name:** `dev.talhaasghar.wattz`

<div id="wattz-version-history" class="mt-4"></div>

<script>
  fetch('/assets/json/wattz-versions.json')
    .then(function(r) { return r.json(); })
    .then(function(versions) {
      var latest = versions[0];
      document.getElementById('wattz-latest-download').href = latest.url;
      document.getElementById('wattz-version-info').textContent =
        'v' + latest.version + ' — ' + latest.date + (latest.size ? ' — ' + latest.size : '');

      if (versions.length > 1) {
        var html = '<details><summary class="mb-2" style="cursor:pointer; opacity:0.8;">Version History</summary>';
        html += '<table class="table" style="font-size: 0.9rem;"><thead><tr><th>Version</th><th>Date</th><th>Notes</th><th></th></tr></thead><tbody>';
        versions.forEach(function(v) {
          html += '<tr><td>v' + v.version + '</td><td>' + v.date + '</td><td>' + v.notes + '</td>';
          html += '<td><a href="' + v.url + '" target="_blank">Download</a></td></tr>';
        });
        html += '</tbody></table></details>';
        document.getElementById('wattz-version-history').innerHTML = html;
      }
    });
</script>

---

## Suggestions {#suggestions}

Have a feature idea, found a bug, or want to contribute? Send an email to [hi@talhaasghar.dev](mailto:hi@talhaasghar.dev) — feedback from real users directly shapes what ships in the public release.
