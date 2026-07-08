# WGU AWS Study Command Center

A single-file browser study app for WGU Cloud + Network Engineering AWS study prep. It includes certification dashboards, objective-tagged practice questions, quick labs, PBQ-style simulations, timed readiness checks, weak-area tracking, local progress tracking, confidence metrics, JSON progress export, and active spaced repetition for flashcards.

## Current Coverage

The app currently includes starter study sections for:

- CompTIA A+ Core 1
- CompTIA A+ Core 2
- CompTIA Network+
- CompTIA Security+
- CompTIA Cloud+
- AWS Cloud Practitioner
- AWS Solutions Architect Associate
- AWS Cloud Operations / SysOps-style prep
- Linux Essentials
- ITIL Foundation

## What Works Now

- Browser-only progress saving with `localStorage`
- Spaced repetition for flashcards using Again / Hard / Good / Easy scheduling
- Due-card count per certification
- Timed readiness checks
- Weak-area tracking by objective tag
- Practice question scoring
- Lab completion tracking
- PBQ-style simulation checks
- Official source bank with vendor/WGU links
- JSON progress export

## Ownership, Use, and Disclaimers

This is an original study tool created for personal learning and portfolio demonstration. It is not affiliated with, endorsed by, sponsored by, or approved by Western Governors University, CompTIA, Amazon Web Services, Linux Professional Institute, or PeopleCert.

This project does not contain exam dumps, real exam questions, protected exam content, or confidential testing material. Any practice questions, labs, flashcards, PBQ-style simulations, explanations, or study paths are original educational content and should be verified against current official objectives before relying on them for exam preparation.

Progress is stored locally in the browser using `localStorage`. There is no backend, no account system, no cloud sync, no database, and no server-side user profile. Clearing browser data may erase saved progress.

## Remaining Gaps

- More question volume is still needed for each certification.
- Objective tags are starter labels and should be expanded into precise vendor objective references.
- Source references should eventually exist per individual question, not just per certification.
- Timed readiness mode is not a full-length simulated exam yet.
- Mobile polish should be tested on real devices.

## Run Locally

Open `index.html` directly in a browser, or serve the folder with any static server. There is no build step and no backend.

## Deploy

### Vercel

Import this repository into Vercel as a static/Other project. Use the repository root as the project root. No framework preset, build command, install command, or output directory is required for the current single-file version.

### GitHub Pages

Put `index.html` at the repository root, then enable Pages from the default branch and root folder.

---

**Last Updated**: July 8, 2026  
**App Status**: Working static prototype with SRS and A+ restored  
**License**: All Rights Reserved
