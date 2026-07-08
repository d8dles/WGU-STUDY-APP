# WGU AWS Study Command Center

A single-file browser study app for WGU Cloud + Network Engineering AWS study prep. It includes certification dashboards, flashcards, practice questions, quick labs, PBQ-style simulations, local progress tracking, confidence metrics, and JSON progress export.

## Ownership, Use, and Disclaimers

This is an original study tool created for personal learning and portfolio demonstration. It is not affiliated with, endorsed by, sponsored by, or approved by Western Governors University, CompTIA, Amazon Web Services, Linux Professional Institute, or PeopleCert.

This project does not contain exam dumps, real exam questions, protected exam content, or confidential testing material. Any practice questions, labs, flashcards, PBQ-style simulations, explanations, or study paths are original educational content and should be verified against current official objectives before relying on them for exam preparation.

Progress is stored locally in the browser using `localStorage`. There is no backend, no account system, no cloud sync, no database, and no server-side user profile. Clearing browser data may erase saved progress.

## Known Gaps Before Serious Use

- CompTIA Cloud+ coverage needs to be added or intentionally excluded with a clear explanation.
- Official objective mapping is missing for many questions, flashcards, labs, and PBQ-style tasks.
- Questions need source and objective references, such as CompTIA domain numbers or AWS exam guide sections.
- Question volume is still prototype-level and not enough by itself for serious exam readiness.
- Spaced repetition is not implemented yet.
- Mobile polish should be tested across real devices.

## Run Locally

Open `index.html` directly in a browser, or serve the folder with any static server. There is no build step and no backend.

## Deploy

### Vercel
Import this repository into Vercel as a static/Other project. Use the repository root as the project root. No framework preset, build command, install command, or output directory is required for the current single-file version.

### GitHub Pages
Put `index.html` at the repository root, then enable Pages from the default branch and root folder.

## Important Content Note

This is an original learning tool, not an exam dump. Before using it as a serious exam-prep source, verify every question, flashcard, lab, and domain against the current official WGU, CompTIA, AWS, LPI, and PeopleCert objectives.

---

# WGU AWS Study App - Complete Guide

## Quick Answer to Your Questions

### Does this app save progress?
**YES.** Uses browser localStorage to persist:
- Selected certification
- Practice answers and scores
- Completed labs
- PBQ/simulation results
- Current tab position

Progress survives page refreshes and browser restarts until cache/browser data is cleared.

### Does it build confidence?
**Yes, with prototype-level confidence tracking.** It tracks all practice attempts, displays a confidence metric based on recent performance, shows attempt counts, and reflects improvement in average score.

### Has it been tested?
**Functionally checked at the prototype level.** Core interactions reviewed:
- [x] localStorage persistence across sessions
- [x] Practice questions save answers correctly
- [x] Scoring calculates percentages properly
- [x] Labs track completion state
- [x] PBQ simulations validate multi-select
- [x] Flashcard navigation works
- [x] UI elements respond correctly
- [x] No obvious app-breaking console errors during local review

### Did this pull information from tests?
**No.** Content is hand-curated and not from official exams. No real exam questions, dumps, or protected exam content are included. Questions should be mapped to official objectives before relying on the app as serious exam prep.

---

## Current App Status

| Feature | Status |
|---------|--------|
| Practice Mode | Working |
| Flashcards | Working |
| Lab Tracking | Working |
| PBQ Simulations | Working |
| Progress Saving | Working |
| Score Tracking | Improved |
| Confidence Metrics | Prototype |
| Progress Export | Working |

## Data Accuracy Assessment

### What's functionally checked
- HTML/JavaScript syntax was reviewed locally.
- `vercel.json` is valid JSON.
- The app uses a single `index.html` file and requires no build step.
- localStorage, flashcards, labs, PBQs, progress tracking, and export logic are present in the code.

### What's not verified yet
- Questions match official exam blueprints.
- Information accuracy against current certification objectives.
- Domain percentages align with official specs.
- Lab deliverables meet WGU expectations.
- PBQ scenarios reflect real exam style.

## How to Use

1. Open `index.html` in a browser.
2. Click a certification on the left.
3. Choose practice, flashcards, labs, PBQs, or sources.
4. Progress saves automatically in the browser.
5. Export progress as JSON from the Sources tab when needed.

## How to Expand

Add more questions, flashcards, labs, and PBQs by editing the `certs` data inside `index.html`.

Recommended structure for future question improvements:

```javascript
{
  q: 'A user has an APIPA address...',
  a: 'The client did not receive a DHCP lease',
  opts: ['Option A', 'Option B', 'Option C', 'Correct answer'],
  exp: 'Explanation of why this is correct.',
  objective: 'CompTIA Network+ N10-009 Domain 1.2',
  source: 'Official exam objective or vendor doc reference',
  verified: true
}
```

## File Structure

```text
index.html
README.md
LICENSE
vercel.json
.nojekyll
.gitignore
IMPROVEMENTS_MADE.md
WGU_STUDY_APP_ANALYSIS.md
```

## Recommended Next Steps

1. Add CompTIA Cloud+ or document why it is intentionally excluded.
2. Add official objective mapping for every question, lab, PBQ, and flashcard.
3. Increase question volume by certification and domain.
4. Add spaced repetition for flashcards.
5. Add a domain weakness dashboard.
6. Test mobile polish on real devices.

---

**Last Updated**: July 8, 2026  
**App Status**: Working static prototype  
**License**: All Rights Reserved
