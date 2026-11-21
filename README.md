# CineKit — Movie Night, Sorted

Stop scrolling. Answer four quick questions and CineKit rolls the reel on a film from your own list — Malayalam classics included. Your watchlist lives on ticket stubs, tonight's film gets a countdown to lights-down, and every finished film lands in your movie diary with its stars.

**Live:** https://abhiramunni.github.io/cinekit/

## What it does

- **Pick for tonight** — mood, time, language and who's watching filter your own list plus the Malayalam classics shelf; the reel spins slot-machine style and lands on a film, with a plain-words "why this one" line. A Double feature toggle picks two back to back.
- **Tonight's screening** — the picked film on the marquee with a live countdown to your start time, a snack checklist (popcorn, filter coffee/chai, blankets, phones on silent) and a "We watched it" button that opens the rating sheet.
- **Watchlist on ticket stubs** — search, language and status filters; move films from Want to watch to Watching to Watched; star ratings on watched stubs; add-your-own form.
- **Malayalam classics shelf** — 10 films every Malayali should see (Kireedam, Manichitrathazhu, Drishyam, Premam, Maheshinte Prathikaaram, Kumbalangi Nights, Joji, Bangalore Days, Ustad Hotel, Nna Thaan Case Kodu), one tap to add.
- **This week's buzz** — O.M Chapter 1 in cinemas from 20 Nov 2026, Ramayana past ₹1,000 crore in India, The Vvaan on Prime Video, King coming 24 Dec.
- **Movie diary** — films watched this month, hours, average rating, top genre, a 14-day minutes chart and a newest-first watched log.
- **Where to watch** — indicative November 2026 prices for Netflix, Prime Video, JioHotstar, ZEE5, SonyLIV and BookMyShow Stream, plus 6 plain-language guides (the 20-minute rule, subtitles vs dubbing, family movie night, theatre vs home, and more).
- **Your data stays yours** — everything is saved in localStorage on your device. No account, no tracking. Copy a movie summary, remove the samples, or erase everything in two taps.

## Details

- Single self-contained `index.html` (photos embedded as base64; the two WebP originals are in `assets/`).
- Warm editorial design: espresso auditorium, ivory paper, amber/gold/terracotta marquee. Fraunces + Inter.
- 4-second cinematic marquee intro with tap-to-skip (quick version on return visits) and a 3-step onboarding coach.
- No backend, no signup. Works offline once loaded (fonts need a connection on first load).

## QA

Headless jsdom suite (`qa-test.js`): run with `node qa-test.js` from this folder. Covers seed data, picker pool maths, runtime/hour formatting, tonight's countdown, watchlist CRUD, ratings, sample removal and erase-all — zero uncaught JS errors, no pictographic emoji.

## Notes

- Prices and "now showing" items are indicative for November 2026 — check the cinema or streaming app before you pay or travel.
- Runtimes for the classics shelf are the commonly listed theatrical runtimes.
