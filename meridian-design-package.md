# Meridian Private Aviation, design package (Tier 1)

Written before generation. Every line of copy below ships verbatim. Band ranges are starting points, validated by the flick test.

## 1. The brand premise

One word from aviation's world: **ready**. Before you ask, the aircraft is ready. The car pulls to the foot of the stairs. Ten minutes from the door of the car to wheels up. Meridian sells one thing: your time, handed back to you, quietly. Every section teaches ready: the hero arrives at an aircraft already waiting, the steps section counts down to the stairs, the interactive moment is a press-and-hold that says wheels up, and the one call to action is a flight quote answered in fifteen minutes.

## 2. The palette as CSS tokens (direction now, sampled from footage after the gate)

```css
:root{
  --canvas:#0f151d;        /* dusk blue-slate, the sky after the sun is gone */
  --panel:#171f2a;         /* wet tarmac raised a step */
  --accent:#e8d6b0;        /* pale champagne, the cabin light */
  --accent-hover:#f3e6c8;
  --accent-muted:rgba(232,214,176,.16);
  --text-secondary:#a7b1bf; /* cloud grey */
  --text-primary:#f2f0ea;   /* warm off-white */
}
```

Design direction said out loud: the default reach for this world is near-black with amber and a thin high-contrast serif. Deviating: blue-slate canvas, champagne accent, and a low-contrast Roman capital display face.

## 3. The type trio

- Display: **Marcellus** 400 (the only weight it has). Quiet Roman capitals, letter-spaced.
- Body: **Albert Sans** 300 and 500.
- Mono: **JetBrains Mono** 400 for small labels, flight codes, the HUD chips.

## 4. The band map (hero, 500vh, scroll range 400vh; widened from the 400vh default after the flick test so every beat survives five normal flicks)

| Band | Range (starting point) | Footage moment | Copy (verbatim) | Entrance |
|---|---|---|---|---|
| 1 | 0.00 to 0.21 | High above, cloud drifting, jet a small light far below | "Wheels up in ten minutes." / "From the door of the car to the door of the sky." | Drift-down (words settle from above, echoing the descent) |
| 2 | 0.25 to 0.47 | Descending, the cloud thinning, mist across the lens | "No lines. No gates. No waiting." | Blur-to-sharp (mist clearing) |
| 3 | 0.51 to 0.73 | Breaking out below the cloud, tarmac and the cabin light growing | "The aircraft is ready before you ask." | Approach-from-depth (grows toward the camera) |
| 4 | 0.77 to 1.00 | At rest on the aircraft, stairs down, cabin light glowing | Headline: "Meridian" / Subline: "Private aviation, said quietly." / CTA: "Request a flight quote" | Word-by-word rise into a staged settle |

Text lives upper-left in every band. The action lane (the jet, lower right) stays clear.

## 5. The static-hero copy block (phones, reduced motion)

Over the ending frame:
- Kicker: "Meridian Private Aviation"
- Headline: "Wheels up in ten minutes."
- Subline: "Private aviation, said quietly. Your aircraft is ready before you ask."
- CTA: "Request a flight quote"

## 6. The below-fold outline (every section funnels to #quote)

Nav: Meridian mark, links: Fleet, How it works, Pricing, Questions, and the button "Request a quote".

**A. The settle strip (right under the hero).** Three mono chips in a row, baseline aligned: "15 min quote response", "2,400 aircraft on call", "7 continents, 24 hours". Living element: a slow shimmer along the runway centerline.

**B. Your time, returned.** Kicker "Why private". Headline "You do not wait for the aircraft. The aircraft waits for you." Three items, each with an image (equal treatment):
1. "Arrive ten minutes before." Body: "Drive to the aircraft. Walk up the stairs. Sit down. Security takes seconds at a private terminal, not hours."
2. "Land where you are going." Body: "Five thousand airports instead of five hundred. Closer to the meeting, the house, the mountain."
3. "Your cabin, your company." Body: "No strangers, no announcements, no one in the aisle. Work, sleep, or say nothing at all."

**C. How it works, the countdown to the stairs.** Kicker "How it works". Steps drawn along the runway centerline, each with a mono time code:
- T minus 15 min: "Tell us the route, the date, the number of seats. A real person answers within fifteen minutes with real aircraft and real prices."
- T minus 24 hr: "Choose the aircraft. Confirm the crew, the catering, the car. One price, in writing, nothing added later."
- T minus 10 min: "Your car pulls to the foot of the stairs. Wheels up."
Living element: a soft pulse traveling down the centerline.

**D. The interactive moment: Wheels up.** Headline "Hold to say wheels up." Instruction "Press and hold." A row of runway lights fills while the visitor holds; releasing early eases the lights back down. Completing it lights the section's content in sequence: "That is the whole process." / "Your time, in your hands." and a button "Request a flight quote". Reduced motion: lights on, content shown, no hold required.

**E. Fleet.** Kicker "Fleet". Headline "The right aircraft, not the biggest one." Three cards, each with an image (equal treatment) and mono spec chips:
1. "Light jet" / "Up to 7 seats. 3 hours. New York to Miami, London to Nice." / chips: "7 seats", "3 hr range", "from 5,800 per hour"
2. "Midsize" / "Up to 9 seats. 5 hours. Coast to coast without a stop." / chips: "9 seats", "5 hr range", "from 7,900 per hour"
3. "Long range" / "Up to 14 seats. 13 hours. Sleep over the Atlantic, land rested." / chips: "14 seats", "13 hr range", "from 12,500 per hour"
Small line below: "Hourly rates are examples for a fictional brand and change with route, season and aircraft."

**F. Pricing, no surprises.** Kicker "Pricing". Headline "One price. In writing. Before you fly." Body: "Every quote includes positioning, crew, overnight fees, airport charges and catering. If it is not on the quote, you do not pay it." Three mono rows: "Positioning and crew: included", "Airport and handling fees: included", "Catering and ground car: included". Living element: a faint glow pulse on the word "included".

**G. Quotes.** Two testimonials, styled as flight logs:
- "I sent the request from the back of a taxi. Fifteen minutes later I had three aircraft and one price. We flew that evening." / "J. Okafor, London to Geneva"
- "No surprises on the invoice. It matched the quote to the pound. That is why we came back." / "M. Lindqvist, Stockholm to Palma"
Below: "Names and quotes are illustrative for a fictional brand."

**H. Questions (FAQ), in the buyers' words.**
- "How fast do you actually reply?" / "Within fifteen minutes, day or night, by a person. Most quotes arrive sooner. Tell us if you need to fly today and we start with the aircraft closest to you."
- "Are there hidden fees?" / "No. The quote includes positioning, crew, overnight charges, airport fees and catering. The invoice matches the quote."
- "Can you fly today?" / "Usually, yes. With 2,400 aircraft on call, a departure within four hours is common on major routes."
- "What if I need to cancel?" / "Cancel free up to 48 hours before departure on most aircraft. The terms are on the quote, in plain words, before you confirm."
- "Will the aircraft be swapped for an older one?" / "The aircraft on your quote is the aircraft you fly. If an operator needs to change it, we tell you first and you choose."

**I. The quote form (#quote).** Kicker "Request a quote". Headline "Where to, and when?" Fields: "From" (placeholder "City or airport"), "To" (placeholder "City or airport"), "Date" (placeholder "Any date, or today"), "Seats" (placeholder "How many of you"), "Email or phone" (placeholder "Where the quote should arrive"). Button: "Request a flight quote". Below the button: "A person replies within fifteen minutes. No account, no obligation." Success state: "Received. A flight advisor is on it. Expect a reply within fifteen minutes." Handling choice: JS-only success state, because the brand is fictional; the page says nothing is sent. (For a real business this switches to mailto or a form service.)

**J. Footer.** Meridian mark and "Meridian Private Aviation". Line: "Meridian is a fictional brand created to showcase a cinematic scroll website. The aircraft, people and prices are illustrative. Imagery is AI generated." Links: Fleet, How it works, Pricing, Questions, Request a quote. Small mono: "MERIDIAN / EST. NOWHERE / 2026".

## 7. The vector layer plan

- The signature: a runway centerline (a dashed vertical SVG line) that draws itself down the page as the visitor scrolls, from the settle strip through How it works to the form. Drawn with stroke-dashoffset off scroll progress. Reduced motion: fully drawn.
- A thin horizon line under each section kicker that draws on entrance.
- Whisper particles: a handful of drifting mist dots in the fixed background layer, cycling at 70 seconds or more, plus a slow drifting radial glow toward the lower right (the cabin light's direction).
- Runway lights for the interactive moment: a row of small circles, filled in sequence by hold progress.
- The favicon: an inline SVG of a horizon line crossed by a thin vertical line (a meridian).

## 8. The engineering list

Blob fetch with a loading ring and 20 second watchdog, poster painted first; dt-normalized lerp in a rAF loop that rests; deadlock-safe gated seeks; delta-gated DOM writes; band pacing in scroll distance with the flick test; the four-layer legibility system (global scrim, per-band scrim, text-shadow token, chip scrim) audited against worst frames at 3.5:1; the five static-hero gates identical in CSS and JS with live change listeners; complete-without-video via the error path; the full quality floor and the whole-site-animated standard; overflow-x clip on html and body; reduced motion honored live in both directions.

## 9. The copy gate line

Every viewer-facing line above ships verbatim. The built page must pass the Phase 9 grep gate (zero em dashes, zero of: leverage, seamless, empower, unlock, robust, actionable, data-driven, solutions) and the body-copy sweep for AI tells. The designed staccato "No lines. No gates. No waiting." and the triplet chips are brand devices and stay.
