---
layout: default
title: Notes - KC1YQN
---

# notes

---

## field notes

---

### February Update

January was my first full month with the Anytone 878. I feel like I’ve got the basics down now — codeplugs make sense, BrandMeister isn’t intimidating anymore, and the hotspot behaves mostly the way I expect it to. Still a beginner, but not lost.

February moved fast, but it also feels like I’ve learned so much that it’s been longer than it actually has. Less structured, more exploring.

At the beginning of the month, I had my first ISS reception. I used an ISS tracker app and caught an afternoon pass at ~80° elevation. I heard stations from Iowa, Ohio, and Connecticut via the International Space Station.

Accommodating Doppler shift during the 10-minute pass was the highlight. Physics felt immediate.

#### Programming + Radio

I finally had a reason to use a Raspberry Pi via Pi-Star. Learned basic Linux CLI skills (git, ssh, nano, sudo, config editing).

Wrote a Python script to parse Pi-Star logs → JSON → push to my site using the GitHub API. Site is hosted on GitHub Pages.

Simplified infrastructure after abandoning Cloudflare Workers. Static site + focused Python scripts is the right level of complexity.

I focus on understanding concepts over memorizing syntax.

Now I have a live dataset updating automatically. Potential extensions:
- Geographic tagging
- Time-of-day analysis
- Pattern visualization

Small system. Real infrastructure.

#### Operating

Mostly TG3100 (USA) and TG91 (Worldwide).

When tired, I don’t feel like talking. Most available time is when tired.

Goal: 100–300 QSOs this year. Enough for experience, not vanity metrics.

I need to key up more. This is a communication hobby.

#### What’s Driving This

It’s the science.

I want to understand *why* it works.

Influenced heavily by *Remembrance of Earth’s Past* by Cixin Liu. It made electromagnetic theory feel consequential.

Currently halfway through *The Radio Theory Handbook* by Ron Bertrand (VK2DQ).

Long-term goal: understand Maxwell’s equations at a real level.

After Bertrand + calculus review → *Introduction to Electrodynamics* (Griffiths).

Not aiming to be a professional physicist. Aiming for depth.

#### Broad Direction

Avoid ten scattered hobbies under “radio.”

Operate more. Study fundamentals. Build infrastructure. Grow deliberately.

HF in the future:
- 40 m likely
- ~60 ft height if possible
- Possibly inverted-V
- Europe as a target

No random wires. No blind installs. I want to understand what I build.

Continue small station-adjacent systems.

Underlying driver: physics.

This will take years. That’s fine.

---

### February 24, 2026 — Winter Storm Reception Test

~24 inches of snow. Signals unusually clean.

Received:
- Whitman – WA1NPO
- West Bridgewater
- Bridgewater – W1MV
- Walpole – K1HRV
- Cumberland – NB1RI
- Providence – R1MIX
- Portsmouth – W1SYE

Confirmed reliable RX across southeastern MA into RI during heavy snow.

---

### February 2 – First ISS Reception

Afternoon pass at ~80° elevation. Heard Iowa, Ohio, Connecticut. Extremely cool.

---

### January 31 – February 1 — Things Clicking Into Place

Major breakthrough: Digital Monitor on AT878.

Understanding:
- Monitor both time slots
- Listen before changing hotspot talkgroups
- Distinction between NEDECN (DMR-MARC) and BrandMeister

Developed real monitoring strategy (DMR + analog pairing).

Completed QSO on TG93 (USA).

Operational confidence increasing.

---

### January 28–30 — Minuteman Repeater Association

Received Heavy Hitters via K1KWP.

Attempted signal check. Repeater repeated transmission (confirmation of TX reach).

Access to MMRA system via Mendon repeater confirmed.

---

### January 23–25, 2026 — Southern New England

Major codeplug revision:
1. Distance-based RepeaterBook search (added RI)
2. Added BrandMeister TGs (USA, TAC310, Casual, Europe, Australia)
3. Troubleshot local DMR repeaters (talkgroup programming + squelch)

Indoor 2 m RX 15–30 miles consistent.

Skywarn activity helpful for testing coverage.

#### Reception Log Highlights (Jan 23)

- AE1C – ~20 mi – DMR Skywarn – S5  
- N1ZHG – ~28 mi – FM – S4  
- KB1RI – ~14 mi – FM – S3–S4  
- NB1RI – ~18 mi – FM – S6  
- K1KWP – ~12 mi – FM – S3  
- K1BIM – ~40 mi – FM – S5–S9  
- W1MV – ~22 mi – FM – S4  

---

### January 22, 2026 — Boston

Fixed incorrect talkgroup on Prudential repeater.

Attempted APRS TX; no APRS.fi listing yet.

---

## January 17, 2026 — New Jersey Net

Listened to a nightly [NJ statewide linked net on W2NJR](https://w2njr.net/) on the Alpine, NJ repeater (~13 miles). Reception was dramatically better with the Slim Jim clipped to a window hanger than with the Signal Stick.

Alpine was full quieting, and I even received a 33 from a wide-area repeater ~50 miles south on 147.375 MHz, despite operating from a north-facing window.

The Slim Jim is clearly the best non-permanent antenna solution—portable, effective, and easy to deploy anywhere.

---

## January 15, 2026 — First FM Transmission

[Slim Jim antenna](https://n9taxlabs.com/shop/ols/products/dual-band-slim-jim-antenna-with-10-or-16-foot-cable) arrived and was hung in a second-floor window aimed toward W1BIM. Successfully participated in the W1BIM nightly net and answered the trivia question: Which steam-powered device was patented in 1861? (Otis elevator.)

A major milestone—~40 miles of FM TX reach using an HT. Received a 59 on signal too. Expectations exceeded once again! It’s addictive.

---

## January 13, 2026 — First QSO

Spent time organizing zones, channels, and scan lists; ChatGPT helped clarify best practices.

After some Pi-Star troubleshooting (DMR ID needed an “01” suffix), the hotspot worked immediately.

Completed my first real QSO via the North America talkgroup on BrandMeister—with a station in China. Dad was able to listen in, which made it even better.

---

## January 5–8, 2026 — Antenna Upgrade

Bluetooth lets the HT stay upstairs while I move around doing chores—more like listening to a podcast. It makes radio easier to integrate into daily life.

Ordered a 2m/70cm [Slim Jim antenna from N9TAX labs](https://n9taxlabs.com/shop/ols/products/dual-band-slim-jim-antenna-with-10-or-16-foot-cable) for window mounting—the best compromise short of a permanent outdoor antenna.

Purchased a Raspberry Pi 3B for hotspot use.

Tried calling W1BOS for signal reports without response. Suspect terrain (Blue Hills) may be blocking the path. Plan to test from work in Cambridge to rule out configuration issues.

---

## January 1–4, 2026 — Massachusetts: Long-Distance RX & First DMR TX

Received W1BIM signal from ~40 miles away, listened to [Georges Old Timers nightly net](http://www.georgesoldtimersnet.com/). This far exceeds expectations for indoor second-floor reception using a Signal Stick.

Exported Massachusetts repeaters from RepeaterBook → codeplug → radio, quickly loading 2–3 dozen repeaters for scanning. Decent Rx from the Prudential Building repeater (W1BOS, ~25 miles).

First successful DMR transmission happened accidentally while unplugging the programming cable—I inadvertently kerchunked the Marshfield digital repeater (W1ATD) about 30 miles away. Confirmed it registered via BrandMeister. Encouraging TX reach from the first floor with a handheld.

---

## December 28–30, 2025 — Jupiter, Florida: Early Nets & DMR

Manually programmed several repeaters with offsets and color codes using RepeaterBook. Listened to the weekly [Jupiter–Tequesta Ham Club net](https://jtrg.org/), which was welcoming and active.

Tried checking into an AllStar net but discovered afterwards that I had programmed the wrong TX frequency. Registered for a DMR ID and attempted DMR texting with Dad—unsuccessful, likely due to configuration errors.

---

## December 25–27, 2025 — Northern New Jersey: First Reception & Net

Indoor reception with the stock rubber duck was quiet… I realized I needed to switch from analog to digital channel type and lower the squelch from 5 to 1. Installing a ¼-wave Signal Stick noticeably improved reception. NOAA Weather Radio came in clearly and is a reliable test signal.

First repeater heard: 442.9 MHz Alpine, NJ (~10–15 miles).

Listening to my first net on Christmas night was tremendously exciting.

---

## December 3–15, 2025 — Licensing & CW

Passed the Technician exam online through [PARC](https://parcradio.org/) and received my call sign a few days later. Having a “Y” means saying “Yankee” a lot, but it’ll do.

Started learning Morse with the **Morse Mania app**— CW is more accessible than expected.

Prepared for operating radio by reading the manual, watching programming videos, and researching New Jersey repeaters.

---

## November 20–30, 2025 — Radio Purchase

Decided on the [Anytone AT-D878](https://www.gigaparts.com/anytone-at-d878uvii-plus-digital-dmr-dual-band-handheld-commercial-radio-with-gps-aprs-rx-tx-and-bluetooth.html), which supports both analog and DMR and has local repeaters in range. Since HF isn’t available with a Technician license, DMR felt like a practical way to explore DX without the cost and complexity of HF infrastructure.

An HT can also work satellites, and that alone will eventually make the hobby worthwhile.

I kept expectations low for FM range since I’m not near major repeaters, but again, DMR serves as a backup path. Purchased the radio and will wait to open it until licensed / Christmas.
