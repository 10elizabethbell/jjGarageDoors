# J&J Garage Doors LLC — handoff at ~60% (calm revamp)

**Live:** https://10elizabethbell.github.io/jjGarageDoors/ · **Repo:** https://github.com/10elizabethbell/jjGarageDoors · **Built:** 2026-10-18 from Muse brief (run 2026-10-18, "CONTRACTORS NJ/PA Conncted" Facebook group post) · **Revamped:** 2026-10-19 to the calm band style

## What changed in the revamp (2026-10-19)
The business hasn't been contacted yet, so the whole page was rebuilt under the new house default (`calm-photo-style.md`, copied from DPG's `index.html`). Facts, the photo, both languages and the text-message wiring carried over.
- **Gone:** the slate-night liftable garage-door canvas hero, the roll-up-door dividers and photo reveal, hinge wobble, dust, sensor beam, heavy system-font caps. (All in git history up to `b527e9f` if you ever want the drag-to-lift door back as an opt-in signature.)
- **Look:** paper (#f4f6fb), night navy (#183a63) and deep navy (#0d2138, faint diagonal lines) bands, J&J's logo gold (#f3b324) as the only accent, used as a fill; gold as text on light is the darker #7a5400. Cal Sans headings, system body at 16/1.7, pill buttons, 24px cards.
- **Hero:** J&J's own two-black-door photo under a navy overlay (phone: full-bleed, cropped to the right door; desktop: the photo sits on the right at near its real size and fades into navy on the left, so it never gets blown up soft). Measured by sampling the brightest photo pixel behind each element (final build): the H1 8.6:1, the promise line 5.4:1, the outlined button 6.8:1 on phones (360/390/320), 6.1:1 or more at 768 and 1024, and 10:1 or more on desktop.
- **H1:** "Garage doors in New Jersey? We do it all." / "¿Puertas de garaje en New Jersey? Lo hacemos todo." The place is in the H1 and "We do it all" is their own flyer slogan. It bounces in letter by letter (only the language on screen), then the plain heading is restored. Reduced motion and no-JS show it at once.
- **Motion:** the H1 bounce-in, one 12px fade-up for things below the first screen, and the floating gold text circle (hidden on the hero and while the quote form is on screen; it texts Jimmy in the visitor's language).
- **New order:** hero → family (Jimmy, Jimmy Jr and Nancy; homes and businesses, over 15 years, three languages) → services as nine rows on navy (tap pre-picks the problem in the form) → our work (photo + big Facebook link) → how it works (3 steps) → quote form → close (name, Jimmy's number big, Jimmy Jr and Nancy) → footer.
- **Icons:** favicon, iPhone icon and og image redone in the new navy (og image is the hero photo + headline).
- `DESIGN.md` and `.impeccable/design.json` rewritten from the new page; old detector ignores cleared.

## What's built
- One page, `index.html`, bilingual EN/ES (Español/English toggle in the header; follows the browser language on first visit and remembers the choice).
- Header: gold house mark + "J&J / Garage Doors LLC", the toggle, and Jimmy's number top right (the only number on the first screen).
- Hero buttons: "Get a quote" (gold, jumps to the form) and "Text a photo" (outlined, opens a pre-written text to Jimmy).
- Quote form: problem chips, home/business, town, name, optional details; composes a text to (908) 374-8196 in the visitor's language. If the page wasn't hidden within 1.2s (no Messages app, e.g. desktop), a line appears with Jimmy's number to call; if Messages opened, it stays off.
- Footer: name, Elizabeth NJ, Jimmy's number, Facebook. No email (none exists).

## Assumptions I made
- **Jimmy's number takes texts.** The brief says "Accepts texts: unknown", and the post caption says "llamenos" (call us). The hero's second button, the form and the floating circle all depend on it. If he doesn't text, switch those to calls.
- **The work photo is their install.** It's the other image in the same Facebook post as the flyer, not confirmed as J&J's job. It's now used twice (hero backdrop and Our work) because it's the only one.
- **"Over 15 years"** comes from Jimmy's truncated Facebook bio ("…been doing residential and commercial over 15 yea…"). "Honest" and "fair price" come from the same bio.
- **"Family owned" and "Elizabeth, New Jersey"** come from the Facebook profile flyer.
- The H1 says "New Jersey" (their base, and the 908 area code); PA and NY are named lower down and in the close.
- Spanish copy is mine ("estimado" for quote, "motor (abridor)" for opener). Worth a read by Jimmy or a native speaker.
- Logo redrawn as an SVG mark from the flyer (the flyer's logo is low-res and sits on a photo).

## Placeholders and gaps
- No email, hours, prices, reviews or street address: the page says nothing about them.
- Only one work photo. Photos wanted: jobs, before/afters, rolling steel doors (commercial).
- The original flyer image couldn't be fetched; the service list comes from Muse's OCR, which the brief says is partly garbled ("Cables, Pulleys" may be truncated).
- Facebook link goes to Jimmy's personal profile (no business page exists).

## Questions for the owner
- Can customers text (908) 374-8196? Should texts go to someone else?
- Is the two-black-door photo your work? Can you send 5–10 more job photos?
- Who should customers call first: Jimmy, Jimmy Jr or Nancy?
- Hours? Emergency or same-day service? Free estimates? (I avoided saying any of these.)
- Which towns do you go to most? Anything in PA/NY you don't cover?
- Do you want a business Facebook page or Google Business Profile?
- Portuguese as a third page language?

## Ideas not built (yours to pick)
- **Runner-up signature (opt-in):** the old drag-to-lift garage door hero, or a commercial steel roll-up curtain you pull down and push up. Other worlds from the trade: a torsion spring that winds as you scroll, the safety-sensor beam as a section divider, a door-panel grid for the work gallery.
- Before/after sliders as soon as Jimmy sends pairs.
- A three-photo work row (4:5 cards) once there are more photos; then the hero and Our work can stop sharing a photo.
- Atkinson Hyperlegible or a larger body size if Ellie decides the audience skews older (the brief doesn't say so, so the full calm motion is on).

## Impeccable review status
Ran the detector, the finish reviewer (verdict: fix) and a sweep of every mode except `live` and `onboard` (critique, audit, harden, optimize, adapt, polish, typeset, layout, colorize, clarify, distill, animate, delight, bolder, quieter, overdrive, extract). Applied: second "Family owned" pill → "Who you'll talk to"; Spanish H1 keeps "Lo hacemos todo." on one line; Facebook row text balanced and now "See more of our work on Facebook."; gold focus ring on the Facebook arrow (was 1.8:1); "fair price" / "homes and businesses" repeats trimmed; 320px header fix; `text-wrap:pretty` on copy; H1 bounce waits for Cal Sans (max 400ms); a service row flashes the chip it picks; dead CSS removed; lighter overlay low in the phone hero.
Not applied: removing Jimmy's number from the footer (finishing rules allow the footer to repeat it). House-style conflicts kept on purpose: eyebrow pills (the craft floor bans them), and the #e6ecf5 field fill (1.2:1 on white, the house's chosen value).
Detector ignores: band texture stripes (house style), flat-type-hierarchy (it only sees 14-22px UI sizes).

## Not verified
- Real-device touch and the real `sms:` handoff on iOS and Android, especially inside Facebook's in-app browser (link format `sms:+1…?&body=`; encoding checked in Chromium for &, #, accents and ¿).
- Tested in Chromium and WebKit (Playwright) at 360, 390, 430 and 1440 wide, English and Spanish, reduced motion and no-JS.
- Whether Jimmy's number receives texts at all.
