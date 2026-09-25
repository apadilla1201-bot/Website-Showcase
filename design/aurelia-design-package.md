# Aurelia Clinic, Miami Beach: design package (Tier 1, single journey)

## 1. The brand premise

Aurelia is built on one word from the world of its footage: morning light. Light flatters without changing anything. It shows what is already there, well. Every treatment at Aurelia aims for exactly that: results people read as rest, not as work. Cosmetic dentistry, injectables and skin treatments, dosed low, priced in writing, done by the doctor you met, with time to think. The site teaches restraint and sells one thing: a 45-minute consultation that starts with a conversation and never ends in a sales pitch.

## 2. The palette as CSS tokens (direction now, finalized from the approved footage)

Sampled from the curtain world: warm pearl linen, honeyed sun, pale sand plaster, one cool sea-green note from the shadow. A deviation said out loud: warm cream with a serif is close to a look this skill bans as a default reach. Here it is the footage's own material world (linen, plaster, morning sun), so it is earned, and the accent stays away from terracotta or gold: it is a deep sea green, which is Miami's water and a clinic's calm at once.

```css
:root{
  --canvas:#F4EFE7;        /* warm pearl, never pure white */
  --panel:#FBF8F2;         /* raised linen */
  --panel-deep:#EAE2D6;    /* recessed sand */
  --accent:#1F5F5B;        /* deep sea green: the CTA and rare emphasis */
  --accent-hover:#174C49;
  --accent-muted:rgba(31,95,91,.14);
  --sun:#E8C689;           /* the sunbeam, whisper level only */
  --text-secondary:#6A6158;
  --text-primary:#28231F;
}
```

## 3. The type trio

- Display: Instrument Serif, regular 400 and italic 400 (the italic carries the one emphasized word per headline).
- Body: Figtree, 400 and 500.
- Labels: DM Mono, 400, letterspaced small caps for kickers, prices and the hold readout.

## 4. The band map (hero 500vh, scroll range 400vh, 0.02 progress = 8vh)

The footage: the camera drifts straight down a sheer sunlit linen curtain that fills the right two thirds of frame and arrives at a calm treatment room counter. The left third is quiet plaster shadow the whole way down. Captions live in that left lane. The action lane (the curtain, the light, the counter) stays clear.

| Band | Range (starting point) | Footage moment | Copy (verbatim) | Entrance |
|---|---|---|---|---|
| 1 | 0.00 to 0.30 | The top of the curtain glows, fabric breathing, dust in the sunbeam | Kicker: "Aurelia Clinic, Miami Beach" / Headline: "You should still look like *you*." | Drift-down: words start above their rest and settle downward, echoing the light falling and the camera's descent. One-time load ramp. |
| 2 | 0.34 to 0.64 | Mid-curtain, folds shifting, the room's depth opening on the left | Headline: "Less product. More time. A doctor in the room." | Blur-to-sharp: the line arrives through the sheer weave into focus. |
| 3 | 0.68 to 1.00 | Arrival: the counter, the glass of water, the light at rest | Headline: "Teeth, skin and face, done *quietly*." / Subline: "Cosmetic dentistry, injectables and skin treatments in Miami Beach. Every visit starts with a conversation. Nothing is sold in it." / CTA: "Book a consultation" / Secondary: "See the treatments" | Word-by-word rise into a staged settle: headline words rise in order, then the subline, then the buttons. |

Band 1 skips its ease-in, band 3 skips its ease-out. Plateaus are 120vh each; ramps are 8vh (0.02). The flick test validates or moves these.

## 5. The static-hero copy block (phones, portrait tablets, reduced motion)

Over the ending frame: Kicker "Aurelia Clinic, Miami Beach". Headline "You should still look like *you*." Subline "Cosmetic dentistry, injectables and skin treatments in Miami Beach. Every visit starts with a conversation, not a sales pitch." CTA "Book a consultation".

## 6. The below-fold outline (every section funnels to #book)

**Nav:** Aurelia wordmark with the sun-line mark. Links: Treatments, Approach, Consultation, Questions, Visit. Button: "Book".

**Section A, Approach** (statement plus three columns; living element: a slow sunbeam drift behind the statement)
- Kicker: "How we work"
- Headline: "The best work is the work nobody *notices*."
- Lede: "Patients tell us the same three things. They are scared of looking done. They have been upsold before. They felt rushed. So we built the clinic around the opposite."
- Principle 1: "Start small." / "Wrinkle relaxers and fillers are dosed to the smallest amount that does the job. You come back at two weeks and we adjust, at no charge. More can always be added. Less cannot."
- Principle 2: "Say the real price." / "Every number is on the table before anything begins, in writing. Follow-ups, touch-ups and aftercare are inside the quote, not added at the desk."
- Principle 3: "Take the time." / "Consultations run 45 minutes with the doctor who treats you. Not a coordinator. Not a sales team. Nobody calls you afterwards to chase a decision."

**Section B, Treatments** (three tall image cards, each with equal treatment: image, name, one line, four items)
- Kicker: "Treatments"
- Headline: "Three rooms. One *standard*."
- Smile: "Porcelain veneers, bonding and whitening, shaded to your skin, your age and your other teeth. Never a white that gives you away." Items: Porcelain veneers · Composite bonding · Whitening · Clear aligners
- Face: "Wrinkle relaxers and fillers placed by a physician, in doses that leave your expression alone." Items: Wrinkle relaxers · Lip and cheek filler · Under-eye · Jawline and chin
- Skin: "Lasers, peels and medical facials, with the real downtime explained day by day before you book." Items: Laser resurfacing · Chemical peels · Medical facials · Pigmentation and redness
- Card link on each: "Ask about this" (to #book, pre-selects the room)

**Section C, The consultation: the one interactive moment** (press and hold)
- Kicker: "The consultation"
- Headline: "Forty-five minutes, no *pressure*."
- Instruction: "Hold to take a minute." Readout in mono: "0:00" counting toward "0:45" as the hold completes (compressed to about 1.6 seconds of holding). Releasing early eases back. Completing lights the four moments in sequence.
- Moment 1: "Minute 0" / "You talk. We listen. What bothers you, what you have tried, what you are afraid of."
- Moment 2: "Minute 10" / "The doctor examines and explains, with a mirror and a pencil, what would help and what would not."
- Moment 3: "Minute 30" / "A written plan with every price on it. Nothing is missing from it later."
- Moment 4: "Minute 45" / "You go home and think about it. No deposit today. No follow-up calls."
- Under the moments: "Consultations are $150, credited to any treatment you choose."
- Reduced motion: all four moments shown, readout at 0:45, no hold needed.

**Section D, Words from patients** (three quotes over the ending frame used as a design image)
- Kicker: "Words from patients"
- Quote 1: "I told her I did not want anyone to know. Two months later my sister asked if I had been sleeping better." / "Dana R., wrinkle relaxers"
- Quote 2: "I came in wanting ten veneers. I left with four, and my smile finally looks like mine." / "Marcus L., porcelain veneers"
- Quote 3: "They showed me photos of day three and day five before I booked. Nothing surprised me." / "Priya S., laser resurfacing"

**Section E, Questions** (accordion, the real objections)
- Kicker: "Questions"
- Headline: "The things people are *afraid* to ask."
- Q: "Will I look frozen or overdone?" / A: "No. We dose low and place carefully, and a check at two weeks is included. Your expression stays. If you want more, we add it then. We cannot take it away, so we never start high."
- Q: "Will veneers look fake?" / A: "Only bad ones do. Ours are shaded to your skin and your other teeth and shaped to your face. We often recommend fewer than you came in asking for."
- Q: "What does it cost?" / A: "Consultations are $150 and credited to treatment. Wrinkle relaxers start at $14 a unit. Porcelain veneers start at $1,800 a tooth. Laser resurfacing starts at $450 a session. Every quote is written down before you decide, with follow-ups included."
- Q: "Who does the injecting?" / A: "A physician, every time. Not a technician, and never someone you have not met."
- Q: "What is the real downtime for lasers?" / A: "It depends on the laser. Light resurfacing means three to five days of pink skin. Deeper treatments mean seven to ten. We show you photos of each day before you book, including the ugly middle ones."
- Q: "Do I have to decide on the day?" / A: "No. Take your written plan home. Nobody will call to chase it."

**Section F, Visit** (address block beside a still)
- Kicker: "Visit"
- Headline: "Alton Road, *Miami Beach*."
- Address: "Aurelia Clinic / 1200 Alton Road, Suite 4 / Miami Beach, FL 33139"
- Hours: "Monday to Friday, 9am to 6pm / Saturday, 9am to 2pm"
- Phone: "(305) 555-0142" / Email: "hello@aureliaclinic.com"
- Note: "Free parking behind the building. Two blocks from the beach."

**Section G, Book (the single call to action, id="book")**
- Kicker: "Book a consultation"
- Headline: "Start with a *conversation*."
- Lede: "Tell us a little and we will reply within one business day to find a time. No deposit. Nothing to decide yet."
- Fields: "Your name" (placeholder "First and last name") · "Email" (placeholder "you@example.com") · "Phone" (placeholder "(305) 555-0100") · "What are you thinking about?" (options: "Not sure yet", "Smile", "Face", "Skin") · "Anything you want us to know?" (placeholder "Optional")
- Button: "Request a consultation"
- Microcopy: "$150, credited to any treatment. Nobody calls to chase you."
- Success state: "Thank you. We will reply within one business day to find a time. Nothing to decide until then."
- Handling on this static demo site: JS-only success state. The form shows its thank-you and the submission goes nowhere. Said plainly to the user. Switch to mailto or a form service when the clinic is real.

**Footer:** "Aurelia Clinic · Miami Beach, Florida" · links: Treatments, Consultation, Questions, Visit, Book · "A demonstration website. Aurelia Clinic is a concept brand; imagery is AI generated." · "© 2026 Aurelia Clinic".

## 7. The vector layer plan

- **Signature element: the sunbeam.** One fixed background layer behind the whole page: a soft diagonal shaft of warm light (the `--sun` token at whisper alpha) drifting on a 90-second cycle, with a dozen dust-mote particles rising slowly through it. Remove it and the page becomes stacked sections instead of a sunlit room. That is the test it passes.
- **The light line.** A thin SVG path under every section headline that draws itself from left to right on entrance (stroke-dashoffset), with a small gap of light near its end, echoing the gap between curtain and wall.
- **Section dividers.** A single hand-drawn SVG "curtain fold" curve between Approach and Treatments and between Questions and Visit, drawn on scroll.
- **The hold ring.** The consultation section's press-and-hold is an SVG ring that fills as the hold progresses, with the mono readout inside it.
- Reduced motion: lines shown fully drawn, motes and sunbeam frozen at a designed frame, the ring full, the four moments visible.

## 8. The engineering list

The full standard in `references/scrub-pipeline.md`: plain Blob fetch behind the poster-first race (the clip is expected under 8 MB; the streamed ring variant if it lands over), dt-normalized lerp in a resting rAF loop, gated seeks with the error escape, delta-gated DOM writes, band pacing in vh validated by the flick test, the four-layer legibility system with a worst-frame audit at 3.5:1 or better, the five static-hero gates kept live with change listeners, complete-without-video, overflow-x clip on html and body, reduced motion honored live in both directions, one living element per section paused off-screen and on hidden tabs, entrances prefixed by container class with retired stagger delays, and the whole-site-animated standard from Phase 8 of the skill.

## 9. The copy gate line

Every viewer-facing line above ships verbatim. The built page must pass the Phase 9 gate before anyone sees it: zero em dashes, zero stock words (leverage, seamless, empower, unlock, robust, actionable, data-driven, solutions), plus the body-copy sweep for AI tells. The designed devices here are craft and stay: the triplet "Less product. More time. A doctor in the room.", the staccato "No deposit today. No follow-up calls.", and the italic emphasized word per headline.

## Appendix: generation prompts (Phase 6)

**Start frame** (Nano Banana Pro, 16:9, 2k, about 2 credits):

A tall sheer white linen curtain fills the right two thirds of the frame, softly backlit by low warm morning sun, the fabric breathing gently inward with a faint breeze, fine dust motes glowing in a shaft of light. The camera looks slightly upward at the top of the curtain, composed as the first moment of a slow downward drift that will descend the length of the curtain and arrive at a calm treatment room counter below. On the left third the same room continues edge to edge: a plain pale plaster wall in soft warm shadow, receding quietly into depth, uncluttered. Palette: warm pearl white linen, honeyed sunlight, pale sand plaster, a hint of cool sea green in the deepest shadow. Atmosphere: still air, floating dust, soft haze. Cinematic, photorealistic, shallow depth, 16:9. No text, no logos, no lettering anywhere.

**Video** (image-to-video, 16:9, 6 seconds, 1080p, no audio):

One continuous shot, no cuts. The camera drifts slowly and steadily straight down the length of a sheer white linen curtain, from its sunlit top to the calm treatment room counter at its foot, along a smooth vertical path at constant speed. The curtain stays alive throughout: it breathes gently inward and back with a faint breeze, folds shifting softly. The scene stays alive: dust motes drift in the warm shaft of morning sun, light shifts subtly through the weave. The shot ends at rest: a pale stone counter at the foot of the curtain, a single clear glass of water catching the light, a small white ceramic dish, soft shadow on the plain plaster wall to the left, the curtain edge glowing on the right, generous empty wall above the counter, everything still and arrived. No text or lettering anywhere.

**Supporting stills** (three, same world, about 2 credits each): Smile, a single pale porcelain dish and a pearl on ivory linen in the same morning light; Face, one white orchid stem in a clear glass of water on the stone counter; Skin, a smooth pale river stone beaded with water in the sunbeam. All: warm pearl, honeyed light, sand plaster, no text, no logos.
