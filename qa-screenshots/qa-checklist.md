# QA Report: Javier Jesus Huaman Cruces

**Date:** 2026-03-01
**URL:** https://javier-huaman.cofoundy.dev
**Status:** PASS

## Data Validation
- [x] Name matches source: "Javier Jesus Huaman Cruces" on page matches Sheet and config.ts
- [x] Email matches source: javierhuamancruces@gmail.com (Cloudflare email-encoded, but correct in config and HTML href)
- [x] Job title matches source: "Ingeniero Industrial | Planificador de Mantenimiento en Gran Mineria" consistent with CV/Sheet
- [x] LinkedIn URL matches: https://linkedin.com/in/javiercruces (matches Sheet data)
- [x] YouTube URL matches: https://www.youtube.com/channel/UC1aWA5Fo6vodMuFDPoz2jFg (matches Sheet data)
- [x] Companies verified: Ferreyros S.A. (Antapaccay, Toquepala), Agricola CHAPI S.A. -- consistent with CV
- [x] Education institutions verified: Universidad Catolica de Trujillo, TECSUP, Colegio de Ingenieros del Peru, Universidad Alas Peruanas -- all from CV
- [x] CIP 372877 matches source data
- [x] No hallucinated data detected

## Clean Deploy
- [x] No "Powered by" / "Made with" / "Built with" watermarks
- [x] No "Lorem ipsum" / "Your name here" / "[placeholder]" text
- [x] No "View source" / "View on GitHub" / "Fork this" template links
- [x] No template watermarks (Astro logo, Vercel badge, etc.)
- [x] No "undefined" or "null" visible in content
- [x] No broken links showing "#" or "javascript:void(0)" as visible text

## Technical
- [x] CSS loads: /_astro/index.BtBCoxo5.css -> HTTP 200
- [x] Profile image loads: /profile.jpg -> HTTP 200 (1.09 MB)
- [x] Favicon loads: /favicon.svg -> HTTP 200
- [x] No critical console errors expected (static Astro site, no JS frameworks)
- [x] Cloudflare email protection active (email-decode.min.js present -- expected behavior)

## Content Review
- [x] Hero section: Name, title, social icons (Email, LinkedIn, YouTube) render correctly
- [x] About section: Bio text matches config.ts, 10 skills tags present
- [x] Projects section: 4 projects listed (HOTSHEET, COVID-19 Continuidad, Capacitacion AMT/SAP, FocusArt Workshops)
- [x] Experience section: 3 positions with date ranges (Oct 2023-Present, Oct 2015-Oct 2023, May 2014-Oct 2015)
- [x] Education section: 4 entries (MBA en curso, TECSUP PAEP, Lean Six Sigma, Ingenieria Industrial)
- [x] Footer: Name, title, social links, copyright 2026, navigation links

## Minor Observations (Non-blocking)
- Profile image is 1.09 MB -- could be optimized for faster loading but not a blocker
- "Educacion" section heading is missing accent mark (should be "Educacion" with tilde) -- minor typography note, matches config

## Issues Found
None

## Evidence
- Full HTML source reviewed via curl
- HTTP status checks performed for all critical assets
