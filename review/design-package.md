# Design Package: Datum Design + Build

Tier 1, single 4-second journey. Invented showcase brand. Every viewer-facing line below ships verbatim.

## Research (buyers' own words)

Pains: "stuck in the middle" between the architect and the builder. "The architect points to the builder's work and the builder points to flaws in the plans." "The little things that add up that were not included." Change orders. Estimates "25% higher than anticipated". "Way over budget and schedule." "Nearly every screw up was blamed on" something else.

Desires: "one point of contact", "one firm accountable for budget, timeline, and quality", questions "answered in a quick conversation" instead of formal paperwork, faster delivery.

Objection: if the architect and the builder are the same company, who keeps the price honest? Loss of checks and balances.

One call to action: Start a conversation (the form at the bottom, anchor `#start`).

## 1. The brand premise

A datum is the reference line on an architectural drawing that every other measurement is taken from. Datum Design + Build is built on one line: the people who draw the building are the people who build it, under one contract, with one number, from the first sketch to the final key. Every section on the page teaches and sells that one idea. The signature element is a single continuous line that draws itself down the whole page as the visitor scrolls, threading every section together.

## 2. The palette as CSS tokens

Sampled from a dusk facade: slate-blue sky, warm timber, board-formed concrete, verdigris copper trim, warm interior light. Deliberately not the near-black-plus-amber default; the accent is verdigris (weathered copper), which is a real material in the footage's world. Values finalize from the approved footage.

```css
:root{
  --canvas:#14181d;
  --panel:#1b2128;
  --accent:#7cbba8;
  --accent-hover:#97d1bf;
  --accent-muted:rgba(124,187,168,.16);
  --text-secondary:#a4abb4;
  --text-primary:#ece7de;
  --timber:#c7955a;
}
```

## 3. The type trio

- Display: Big Shoulders Display, weights 500 and 700. Tall, architectural, drawn with a ruler.
- Body: Instrument Sans, weights 400 and 500. Quiet and modern.
- Mono: IBM Plex Mono, weight 400. Small labels, survey marks, numbers.

## 4. The concept and the band map

Concept A, "The Descent": dusk. The camera starts high at the roofline of a finished modern house (board-formed concrete, warm vertical timber cladding, tall glass, a thin verdigris copper fascia) and glides straight down the facade to eye level, arriving at rest on the lit entry with a still reflecting pool in the foreground. The house holds the left two thirds of the frame. The right third is open dusk sky over quiet landscape, the caption lane. Hero height 400vh.

| Band | Range (starting point) | Footage moment | Copy (verbatim) | Entrance |
|---|---|---|---|---|
| 1 | 0.00 to 0.24 | Roofline against the dusk sky, camera begins to descend | Kicker: "Datum Design + Build" / "Every good building starts with one line." | Drift-down (words settle downward as the camera descends) |
| 2 | 0.28 to 0.52 | Mid facade, timber and glass sliding up past the lens | "The people who draw it are the people who build it." | Grid snap-align (characters slide into place like cladding boards) |
| 3 | 0.56 to 0.78 | Approaching eye level, the entry light grows | "One contract. One number. One phone to call." | Word-punch with overshoot on "One" (three arrivals) |
| 4 (settle) | 0.82 to 1.00 | At rest: the lit entry, the pool reflection | Headline: "Built on one line." / Subline: "Datum is a design-build studio. Architect and builder, one team, one contract, from the first sketch to the final key." / CTA: "Start a conversation" / Secondary: "See the work" | Word-by-word rise into a staged settle |

## 5. The static-hero copy block

Over the ending frame, for phones and reduced motion:

- Kicker: "Datum Design + Build"
- Headline: "Built on one line."
- Subline: "Architect and builder, one team, one contract, from the first sketch to the final key."
- CTA: "Start a conversation"
- Secondary: "See the work"

## 6. The below-fold outline

Nav: mark + "Datum", links Work, Process, Studio, Questions, CTA button "Start a project".

### Section A: The middle
Kicker: "The old way"
Headline: "You should never be stuck in the middle."
Body: "Hire an architect, then hire a builder. When something goes wrong, the architect points at the build and the builder points at the drawings. You hold the bill."
Turn: "At Datum there is no middle. The drawing and the building come from the same table."
Visual: the datum line splits into two lines (drawn, labeled "Architect" and "Builder" in mono) and merges back into one.

### Section B: Process (three steps, drawn icons, equal treatment)
Kicker: "How it works"
Headline: "Three moves. One line."
1. "01 Sketch": "We design with the cost sheet open. Every line we draw has a price beside it before you fall in love with it."
2. "02 Number": "One fixed number before we break ground. It covers what the drawings show, and the drawings show everything."
3. "03 Build": "The team that drew it is the team on site. Questions get answered in a conversation, not a change order."

### Section C: The interactive moment (lives here, mid-page)
Kicker: "Try it"
Headline: "Hold to draw the line."
Instruction: "Press and hold. Let go early and the line eases back."
Mechanic: while the visitor holds, the datum line draws across a simple elevation drawing of the house. When it completes, the line drawing crossfades into supporting still 1 (the finished exterior in daylight) and three lines light up in sequence: "Drawn by us." "Priced by us." "Built by us." Reduced motion: final state shown, no hold required.

### Section D: Work (two projects, equal cards)
Kicker: "Selected work"
Headline: "Quiet buildings that keep their promises."
Card 1 (still 2, interior): "Larkspur House" / "Family home. 3,400 square feet. Design to keys in fourteen months, on the number we signed."
Card 2 (ending frame, exterior dusk): "Ridge Studio" / "A workshop and guest house on a steep lot. One contract, one crew, zero unplanned change orders."
Link under both: "See the work" anchors here.

### Section E: Questions (the real objections)
Kicker: "Questions"
Headline: "Fair questions. Straight answers."
1. Q: "If the architect and the builder are the same company, who keeps the price honest?" A: "You do. Our pricing is open book. You see every subcontractor bid and every material cost, and our fee is a fixed percentage written into the contract on day one."
2. Q: "What happens when I change my mind?" A: "You will, and that is fine. We price the change in writing before anyone builds it. You say yes or no. Nothing gets added to the bill that you did not sign."
3. Q: "How long does a house take?" A: "Most homes run twelve to sixteen months from first sketch to keys. Because design and construction overlap, that is usually several months faster than hiring the two separately."
4. Q: "Can I bring my own architect?" A: "Yes. We build for other architects often. You lose the single contract, but you keep a builder who reads drawings like a designer."

### Section F: Voices (fictional, labeled in the footer)
Quote 1: "We never had to referee an argument. There was one phone number and it always picked up." Attribution: "Maren and Theo, Larkspur House"
Quote 2: "The number we signed was the number we paid. I did not know that was possible." Attribution: "Priya S., Ridge Studio"

### Section G: Start (the single call to action)
Kicker: "Start"
Headline: "Tell us about your site."
Body: "A conversation costs nothing. Bring a lot, a sketch, or just an idea."
Form labels: "Your name", "Email", "What are you building?" Placeholder for the last: "A family home on a sloped lot, about 3,000 square feet"
Button: "Start a conversation"
Success state (JS-only, honest): "Thank you. This is a showcase site, so nothing was sent. A real studio would call you within two days."

### Footer
"Datum Design + Build is a fictional studio created to showcase this website. Every image and quote on this page is AI generated or invented." Links: Work, Process, Questions, Start. Small line: "Built as a design showcase."

## 7. The vector layer plan

- The datum line: one SVG path in the left gutter of the page (moves to a top rule on phones) that draws itself with `stroke-dashoffset` as the page scrolls, passing behind each section heading. Survey tick marks and a small mono readout at each section ("DATUM 01", "02"...).
- Section A split-and-merge line, drawn on entrance.
- Process icons: three hand-drawn SVG glyphs (a pencil line, a number box, a wall section) that draw on entrance.
- Elevation drawing for the hold moment: a simple SVG house elevation.
- Whisper particles: eight slow dust motes on a fixed background layer with a 70-second gradient drift toward the dusk grade.
- Reduced motion: every path shown fully drawn, drives stopped.

## 8. The engineering list

The full standard in scrub-pipeline.md: Blob fetch (plain form under 8 MB, poster painted first, video only inside the gated path), dt-normalized lerp that rests, gated seeks with the error escape, delta-gated DOM writes, band pacing in scroll distance with the flick test, the four-layer legibility system (base scrim, per-band scrim, text shadow token, chip scrim), the five static-hero gates identical in CSS and JS with live change listeners, complete-without-video, reduced motion honored live in both directions, overflow-x clip on html and body, the quality floor, and the whole-site-animated standard.

## 9. The copy gate line

Every viewer-facing line above ships verbatim. The built page must pass the Phase 9 grep gate: zero em dashes, zero stock words (leverage, seamless, empower, unlock, robust, actionable, data-driven, solutions), plus the sweep for AI tells. The designed devices here are craft and stay: "One contract. One number. One phone to call." and "Drawn by us. Priced by us. Built by us."
