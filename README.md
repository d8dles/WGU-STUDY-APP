# WGU AWS Study Command Center

A single-file browser study app for WGU Cloud + Network Engineering AWS study prep. It includes certification dashboards, flashcards, practice questions, quick labs, PBQ-style simulations, timed readiness checks, weak-area tracking, local progress tracking, confidence metrics, and JSON progress export.

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

## Ownership, Use, and Disclaimers

This is an original study tool created for personal learning and portfolio demonstration. It is not affiliated with, endorsed by, sponsored by, or approved by Western Governors University, CompTIA, Amazon Web Services, Linux Professional Institute, or PeopleCert.

This project does not contain exam dumps, real exam questions, protected exam content, or confidential testing material. Any practice questions, labs, flashcards, PBQ-style simulations, explanations, or study paths are original educational content and should be verified against current official objectives before relying on them for exam preparation.

Progress is stored locally in the browser using `localStorage`. There is no backend, no account system, no cloud sync, no database, and no server-side user profile. Clearing browser data may erase saved progress.

## Known Gaps Before Serious Use

- Official objective mapping still needs deeper verification against current vendor objective PDFs/exam guides.
- Questions need source references, such as CompTIA domain numbers, AWS exam guide sections, or vendor documentation links.
- Question volume is still prototype-level and not enough by itself for serious exam readiness.
- Spaced repetition is not implemented yet.
- Mobile polish should be tested across real devices.
- The timed exam mode is a readiness drill, not a real exam simulator yet.

## Run Locally

Open `index.html` directly in a browser, or serve the folder with any static server. There is no build step and no backend.

## Deploy

### Vercel

Import this repository into Vercel as a static/Other project. Use the repository root as the project root. No framework preset, build command, install command, or output directory is required for the current single-file version.

### GitHub Pages

Put `index.html` at the repository root, then enable Pages from the default branch and root folder.

## How to Use

1. Open the app.
2. Select a certification from the sidebar.
3. Use Overview, Practice, Timed Exam, Weak Areas, Flashcards, Labs, PBQ/Sims, and Sources.
4. Progress saves automatically in the browser.
5. Export progress as JSON from the Sources tab when needed.

## Recommended Next Steps

1. Verify every question against current official objectives.
2. Add more questions per certification and per domain.
3. Add source links/objective IDs to every question, flashcard, lab, and PBQ.
4. Add spaced repetition for flashcards.
5. Add domain-level readiness scoring.
6. Add real mobile testing.

---

**Last Updated**: July 8, 2026  
**App Status**: Working static prototype with A+ restored  
**License**: All Rights Reserved
