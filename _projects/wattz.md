---
layout: page
title: Wattz
description: a modern android app for tracking household electricity consumption
img: assets/img/wattz/app_icon.png
importance: 1
category: fun
---

**Wattz** is a modern Android application for tracking household electricity consumption, meter readings, usage analytics, and estimated billing. Built with React Native and Expo, it brings a premium fintech-grade experience to everyday energy management.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/home-screen.png" title="Home Screen" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/analytics-screen.png" title="Analytics" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/wattz/reading-history.png" title="Reading History" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The home dashboard puts your most important electricity data front and center. The analytics screen breaks down consumption patterns over time. Reading history provides a chronological view of all recorded meter data.
</div>

### Features

- **Meter Reading Entry** — Record electricity meter readings with manual input or OCR-powered camera scanning via ML Kit
- **Consumption Tracking** — Automatically calculate units consumed between readings and visualize daily, weekly, and monthly trends
- **Analytics Dashboard** — Interactive charts showing usage patterns, peak consumption periods, and month-over-month comparisons
- **Estimated Billing** — Calculate projected electricity costs based on recorded consumption and configurable rate tiers
- **Reading History** — Browse, search, and export a complete chronological log of all meter readings
- **Usage Goals** — Set monthly consumption targets and track progress with visual indicators
- **Reminders** — Never miss a reading with smart notifications and configurable reminder schedules
- **Onboarding** — Guided first-run experience to get users started quickly
- **Dark Mode** — Full light and dark theme support following Material Design 3 guidelines
- **Offline-First** — All data stored locally on device using SQLite; works without an internet connection
- **CSV Export** — Export reading history as CSV for sharing or external analysis

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/wattz/settings.png" title="Settings" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/wattz/meter-reading.png" title="Meter Reading Dialog" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The settings screen provides easy access to app configuration, rate tiers, and data management. The meter reading dialog supports both manual entry and camera-based OCR scanning.
</div>

### Design Philosophy

Wattz follows a design language called **"Electric Minimalist"** — combining the high-performance feel of a modern fintech app with the playful accessibility of a lifestyle companion. The UI is built entirely on **Material Design 3** principles with a clean, airy aesthetic inspired by Google Pixel apps and premium banking interfaces.

The primary color palette is anchored by **Wattz Yellow (#FFC107)**, used for key interactive elements and active states. Typography uses **Inter** exclusively, with a dramatic hierarchy that makes consumption numbers feel impactful. Depth is conveyed through tonal layering and ambient shadows rather than heavy borders.

### Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | React Native 0.85 via Expo SDK 56 |
| Language | TypeScript |
| Styling | NativeWind (Tailwind CSS for RN) |
| Database | expo-sqlite (offline-first) |
| OCR | expo-mlkit-ocr (camera meter scanning) |
| Navigation | Expo Router (file-based) |
| Animations | React Native Reanimated 4 |
| Notifications | expo-notifications |
| Architecture | React Compiler, typed routes |

### What I Learned

Building Wattz taught me how to design a data-heavy mobile app that still feels lightweight and approachable. The biggest challenge was balancing information density with visual clarity — making sure users can answer "how much electricity have I used?" at a glance without feeling overwhelmed by charts and numbers. The OCR meter scanning feature also pushed me into working with on-device ML inference, which opened up possibilities for future smart features.

Wattz is available on the Google Play Store under the package name `dev.talhaasghar.wattz`.
