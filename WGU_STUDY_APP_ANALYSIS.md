# WGU Study App Analysis

## Current status

The repository is now a static web app that can be shared on GitHub and imported into Vercel. The app does not require React, Vite, npm, a backend, or environment variables.

## Architecture

- `index.html` contains the full app shell, styling, data, and JavaScript.
- Browser `localStorage` is used for saved progress.
- `vercel.json` provides clean URLs and basic security headers.
- No server-side code exists.
- No account system exists.
- No database exists.

## Functional coverage

The app includes:

- Certification navigation
- Search/filter across certification content
- Domain progress display
- Study focus notes
- Practice questions
- Flashcards
- Quick labs
- PBQ-style simulations
- Local progress persistence
- Confidence display
- JSON progress export

## Certification coverage included

- CompTIA Cloud+ gap module
- CompTIA Network+
- CompTIA Security+
- AWS Cloud Practitioner
- AWS Solutions Architect Associate
- Linux Essentials
- ITIL Foundation

## Known gaps

This is still a prototype and should not be treated as complete exam prep by itself.

Priority gaps:

1. Official objective mapping is missing.
2. Question volume is not high enough for serious readiness.
3. Explanations need source references.
4. Spaced repetition is not implemented.
5. Mobile polish still needs live-device testing.
6. The app does not sync across devices.
7. The app has no admin/editor interface.

## Recommended next build phase

### Phase 1: Accuracy

- Add objective IDs to every question.
- Add a source field to every question, lab, PBQ, and flashcard.
- Add a verified flag only after objective/source review.

### Phase 2: Confidence

- Add domain-level scoring.
- Add weak-area recommendations.
- Add repeat-until-mastered question sets.
- Add daily streaks and study time.

### Phase 3: Scale

- Move content into JSON files.
- Add import/export of study packs.
- Consider a lightweight backend only if cross-device sync becomes necessary.

## Deployment recommendation

Deploy to Vercel as a static/Other project.

Use:

- Framework preset: Other / Static
- Build command: none
- Install command: none
- Output directory: blank/root
- Root directory: repo root

## Content warning

This project is not affiliated with WGU, CompTIA, AWS, LPI, or PeopleCert. It does not include real exam questions, exam dumps, or protected testing content. All study content should be verified against current official objectives before serious use.
