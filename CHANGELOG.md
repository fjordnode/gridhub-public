# Changelog

Notable changes to GridHub, roughly grouped by when they shipped.

## February 2026

- **Calendar Subscribe URLs** — Subscribe to a live-updating .ics feed URL from any calendar app, with signed tokens and automatic refresh
- **Calendar Export Reminders** — Choose reminder alerts (10min / 30min / 1h / 24h before sessions) for both downloaded .ics files and subscribe URLs
- **MotoGP Results Layout** — Reordered columns to match official timing screens, combined-best view for test sessions aggregating fastest laps across all sessions per rider
- **WSBK 2025 Data** — Expanded to 14 circuit mappings with updated results and standings
- **F1 Live Telemetry** — Toggleable telemetry strip showing current speed, gear, throttle, brake, DRS, and RPM per driver with faster 250ms refresh rate
- **Purple Sector Deltas** — Session-best sectors now show the time margin over the next-fastest, and fastest speed trap is highlighted in purple
- **F1 Live Timing Overhaul** — Complete rewrite with snapshot-first architecture, real-time tyre strategy graphics with compound badges, sector progression and mini-sector visualization, pit status detection, and auto-width tables
- **Moto2/Moto3 Results** — Historical results page now includes support class results
- **Navigation Redesign** — New tab bar layout replacing the previous header navigation
- **Weekend Schedule Redesign** — Horizontal day-column layout with compact inline weather
- **Dynamic Social Previews** — Shared links generate Open Graph images with event-specific artwork
- **F1 2026 Pre-season** — Test sessions displayed as Day 1/2/3 with updated team logos

## January 2026

- **WSBK 2026 Schedule** — Full 2026 WorldSBK calendar with correct per-venue session times
- **Calendar Export** — New page to download or subscribe to a personalized .ics racing calendar, filtered by series, session types, and support classes
- **F1 Pre-season Tests** — Pre-season test events now appear in the main calendar view
- **MotoGP 2026 Preliminary Calendar** — Full provisional schedule from official announcements, auto-upgrades when API data becomes available

## December 2025

- **2026 Calendars** — Added 2026 season data for all series with year selector support
- **Championship Progression Charts** — Interactive line charts showing points accumulation across the season for both F1 and MotoGP
- **F1 Results Validation** — Automatic post-race revalidation for 7 days to catch DSQs, penalties, and classification changes
- **Card-based Previous Results** — Redesigned previous race results with a cleaner card layout
- **Dark Mode Only** — Removed light theme, app now runs in dark mode exclusively
- **Umami Analytics** — Replaced Vercel Analytics with self-hosted Umami

## November 2025

- **F1 Live Timing** — Real-time positions, gaps, intervals, and sector times via OpenF1 API with WebSocket streaming
- **Position Change Animations** — Animated position arrows in live timing when drivers gain or lose places
- **F1 Tyre Age** — Live timing shows actual tyre age (laps) for current stints
- **F1 Sprint Qualifying** — Full Sprint Shootout session support in results and live timing

## October 2025

- **MotoGP Live Timing** — Real-time session data with lap tracking, sector times, and flag status
- **MotoGP Sprint Wins** — Championship standings now correctly account for sprint race points

## September 2025

- **Series Visibility Controls** — Hide series you don't follow from the settings menu; persists across visits
- **Results Overhaul** — Seamless session switching with instant cached data, no more flickering or loading delays
- **F1 Tyre Strategy Column** — Color-coded compound badges showing tyre progression through races (S → M → H)
- **Smart Loading Indicators** — Loading spinners only appear during actual API fetches, not when serving cached data
- **Session Weather** — Weather forecasts shown per session in event detail pages

## August 2025

- **MotoGP Session Formats** — Correct session handling across 2023–2025 format changes (P1/P2 vs FP1/FP2, sprint evolution)
- **Live Session Countdown** — Flag-aware countdown timer with automatic session detection

## July 2025

- **F1 Weather Integration** — Per-session weather data from OpenF1 API
- **MotoGP Sector Times** — Sector times and speed data in results tables
- **WSBK & WEC Standings** — Full championship standings integration for WorldSBK and WEC

## June 2025

- **Historical Championship Standings** — F1 back to 2015, MotoGP back to 2013 with year selector
- **Shared Results Architecture** — Unified results display across all series with consistent session tabs
- **MotoGP Historical Results** — Fixed event lookup for 2023/2024 seasons with proper language-variant matching
- **Smarter Caching** — Finished race results cached for days instead of seconds; cache-first data loading
- **Hybrid API Server** — Express-based API proxy with multi-layer caching, replacing direct client-side API calls
- **URL Series Filtering** — Bookmarkable URLs like `/?series=F1,MotoGP`

## May 2025

- **Initial Release** — GridHub launches with F1, MotoGP, WEC, and WorldSBK support
- Calendar with list and calendar views
- Event detail pages with weekend schedules, track maps, and weather forecasts
- Previous race winners
- Race results with per-session tabs
- Mobile-responsive design
