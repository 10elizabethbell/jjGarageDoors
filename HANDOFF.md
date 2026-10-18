# J&J Garage Doors LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/jjGarageDoors/ · **Repo:** https://github.com/10elizabethbell/jjGarageDoors · **Built:** 2026-10-18 from Muse brief (run 2026-10-18, found via the "CONTRACTORS NJ/PA Conncted" Facebook group post)

## What's built
- One page, `index.html`, bilingual EN/ES (toggle top right; follows the browser's language on first visit and remembers the choice). Phone-first.
- World: J&J's own black-and-gold flyer, made physical. Slate-night ground (#1a2330, not black), logo gold #f3b324, heavy stacked caps.
- Signature: the hero is a lit garage at night. The door lifts and lowers by itself until you touch it, then follows your finger or mouse up and down. Like a balanced door, it stays where you leave it. Sections hinge-wobble and light leaks through the seams. Dust drifts in the light and gets pushed by the pointer. If you put a finger in the safety-sensor beam while the door is closing, it reverses and the sensor blinks. Arrow keys, Home and End work too (it's a `role="slider"`).
- Carried through: the section dividers are the bottom hem of a steel roll-up door that rolls up as you scroll, and the work photo sits behind a roll-up door that opens when it scrolls into view.
- Sections: header (logo mark, Español, number top right), hero (two buttons: Get a quote / Text a photo), What we fix (rows that pre-select the problem in the form), Our work (1 photo + big Facebook link), We speak English / Hablamos español / Falamos português + family, How it works, quote form, closing "We do it all." with all three contacts, Facebook.
- Contact: the header number calls Jimmy (908) 374-8196. The quote form and "Text a photo" open a pre-written text to Jimmy's number, in the visitor's language. On a computer, a note appears after sending saying to call instead. The footer lists Jimmy, Jimmy Jr and Nancy as tap-to-call.

## Assumptions I made
- **Jimmy's number takes texts.** The brief says "Accepts texts: unknown", and the post caption says "llamenos" (call us). Both text buttons depend on it. If he doesn't text, swap the form's handoff to a call and change "Text a photo" to something else.
- **The work photo is their install.** It's the other image in the same Facebook post as the flyer (two black doors with glass), not confirmed as J&J's job. The flyer's door renders look like stock/AI images, so I didn't use them.
- **"Over 15 years"**: from Jimmy's Facebook bio, which is cut off: "J&J Garage Doors LLC honestly Reliable fare prices been doing residential and commercial over 15 yea…". "Honest" and "fair price" in the copy come from the same bio.
- **"Family owned" and "Elizabeth, New Jersey"**: from the Facebook profile flyer (not in Muse's brief, which only had the 908 area code).
- How it works says "Tell us what it's doing / We give you a price (honest answer, fair price) / We fix it (or install your new door)". I kept it free of promises nobody confirmed (free estimates, on-site visits, testing with the customer, same-day).
- **Primary number**: Jimmy's, because the post caption names it. Nancy's role (office? scheduling?) is unknown.
- Spanish copy is mine. I used "estimado" for quote and "motor (abridor)" for opener, as NJ Latino customers say them. Worth a read by a native speaker or Jimmy.
- Logo: redrawn as an SVG mark (gold house with garage door) from the flyer, because the flyer's logo is low-res and sits on a photo. The favicon, iPhone icon and og image use the redraw.

## Placeholders and gaps
- No email (none published; none invented). The footer has no email line.
- No hours, no prices, no reviews, no street address: the page says nothing about them.
- Only one work photo. "Photos wanted": jobs, before/afters, rolling steel doors (commercial).
- The original flyer image (fbid 2922525571437007) couldn't be fetched; the service list comes from Muse's OCR, which the brief says is partly garbled. "Cables, Pulleys" may be truncated on the flyer.
- Facebook link goes to Jimmy's personal profile (no business page exists).

## Questions for the owner
- Can customers text (908) 374-8196? Should texts go to someone else?
- Is the two-black-door photo your work? Can you send 5–10 more job photos?
- Who should customers call first: Jimmy, Jimmy Jr or Nancy? Should all three numbers be on the site?
- Hours? Emergency or same-day service? Free estimates? (I avoided saying any of these.)
- Which towns do you go to most? Anything in PA/NY you don't cover?
- Do you want a business Facebook page or Google Business Profile? (No Maps listing exists.)
- Do you want Portuguese as a third page language?

## Ideas not built (yours to pick)
- **Runner-up world:** a commercial steel roll-up door as the hero (corrugated curtain you pull down and push up), slats as the page's motif throughout. Stronger for the commercial side, less warm for homeowners.
- **Overdrive:** draw the torsion spring and cables above the door inside the garage, winding as the door lifts, with a "broken spring" moment where it goes slack. Ties the hero to their first service.
- The steel slats on the dividers and photo door are CSS gradients with light falloff and rails; a canvas or raster version with real corrugation and rivets would read even more like steel.
- Before/after sliders as soon as Jimmy sends pairs.
- Portuguese language option.
- Desktop: the work photo is only 800×600 (all Facebook gives without login), so it's a little soft on big retina screens. A larger original from Jimmy fixes it.

## Impeccable review status
Ran critique, audit, harden, optimize, adapt, polish, typeset, layout, colorize, clarify, distill, animate, delight, bolder, quieter and overdrive (as review agents), the detector, and the finish reviewer (2 rounds, the unattended limit). Skipped `live` (needs you in the browser) and `onboard` (no first-run flow). The last verdict was still **fix**. These are open:
- **Steel slats** (dividers + photo door) are CSS gradients with falloff, rails and shadow. The reviewer wants real corrugation/end-locks, as a canvas or raster asset.
- **Desktop services:** a small gap beside the last repair row ("Openers"); 7 repairs don't split evenly into two columns.
- Fixed since that verdict, not re-scored: the step 3 filler line, the orange seam strokes, the driveway light cone (now visible from a quarter open) and motes on dark asphalt.
- Detector ignores recorded in `.impeccable/config.json`: roll-door stripes (they're the product), system font (house rule), padding on ruled lists, and the type-scale check (it only counts body sizes).

## Not verified
- Real-device touch (tested with simulated touch in Chromium and WebKit/Playwright at 360, 390, 414, 430 and 844×390).
- The real `sms:` handoff on iOS and Android, especially inside Facebook's in-app browser (link format `sms:+1…?&body=`; encoding checked for &, #, accents).
- Frame rate on old Android phones.
- Whether Jimmy's number receives texts at all.
