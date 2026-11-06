# Next Route — Patient Journey Navigator

Hackathon prototype for **PS3 "The Missing Link – Patient Journey & Healthcare Access Navigator"**.

Next Route helps patients, especially elderly patients and patients with disabilities, through the administrative side of care: finding the right facility and department, knowing which documents and referrals to bring, booking a slot, following the queue on the day, and tracking follow-ups. It does not diagnose.

**Live demo:** https://<your-username>.github.io/next-route/

## Features
- Step-by-step patient journey: service → facility → documents → booking → visit pass → follow-ups
- English, Tamil, Hindi and Kannada, with read-aloud
- State-wide facility coverage, including rural areas
- Accessible design (Atkinson Hyperlegible font, large targets, plain language)
- Talk-to-a-person help with call-back times

## Constraint handling (Stress-test lab)
| Card | Constraint | How Next Route adapts |
| --- | --- | --- |
| C04 | Malformed or malicious data | Validation gate: safe parsing, per-record checks, injection/Unicode defence, quarantine with a data-quality report. Existing data is never overwritten. |
| C05 | Demand ×3, resources −50% | Never overbooks; honours existing bookings first, moves displaced ones before new patients, then priority groups (60+, pregnant, disability), follow-ups, first come first served. Navigator queue triaged with instant self-service answers. |

Open the app → **Stress-test lab** to trigger each constraint live.

## Run locally
No build step. Open `index.html` in any modern browser.

## Tech
Single-file HTML/CSS/JavaScript app. Data is stored only in the browser (localStorage); nothing is sent to a server.

## Team
<add team member names>
