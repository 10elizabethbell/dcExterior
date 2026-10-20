# DC Exterior — handoff at ~60%

**Live:** https://10elizabethbell.github.io/dcExterior/ · **Repo:** https://github.com/10elizabethbell/dcExterior · **Built:** 2026-10-20 from Muse brief 2026-10-20 (Essex County Contractor Referrals group post)

## What's built
- One page, calm band style: navy header + hero → paper services → deep-navy "How a free quote works" → paper quote form → navy close → deep-navy footer.
- Palette from their own material: the ad's navy band (#0d2c4d / deep #061b31), the ad's headline yellow (#f8d404) as the one fill accent, the logo's blue (#038df8) for service icons and form hover/focus outlines.
- Real logo (their Facebook profile image) with the black square keyed out so it sits on navy: house+DC mark in the header, full logo on the desktop hero, favicon and home-screen icon from the house+DC mark, og.png for link previews.
- Hero: plain textured navy (no real job photos exist). Eyebrow "Free quotes", H1 "Keep the rain out of your home." with the letter bounce-in, one promise line, "Get a free quote" (yellow) + "What we fix" (outlined).
- Services: Roof, Chimney, Gutters, Pointing and brickwork, Exterior painting, each with the signs from their own ad ("Missing or damaged shingles · leaks…"). Tapping a row jumps to the form with that job pre-selected.
- Contact is Facebook Messenger only (no phone or email exists): top-right "Message us", the floating circle (after the hero, hidden while the form is on screen), and the quote form, which writes the message, copies it to the clipboard, and opens `m.me/61558693145112?text=…`. If Messenger opens empty, the page shows the message with Copy and Open Messenger buttons.
- Facebook: "See our work on Facebook" card in the close band, and in the footer.

## Assumptions I made
- **"We" voice:** the ad says "Contact us"; no owner name, so it speaks as a crew.
- **Painting** is listed because it's on their logo ("Painting · Gutters · Roof Repairs"); it isn't in the ad.
- **"How a free quote works"** steps (message → we take a look → we fix it once you're happy) are inferred from "Free quotes"; the owner should confirm whether they quote from photos or visit first.
- **Ad wording lightly edited for plain English:** "Water penetration/infiltration" → "water getting in", "Deteriorating brickwork" → "crumbling brick".
- **"Front roof to roots"** (caption) is not used: the image doesn't contain it, and it reads like a typo for "From roof to roots". Ask the owner.
- **H1 has no place in it** (calm style wants one) because the brief forbids inferring a location. Once their area is known: e.g. "Keep the rain out in <Town>."
- Town is a required form field so the owner knows where the job is.

## Placeholders and gaps
- **No phone number and no email** anywhere. The header slot for the phone holds "Message us" instead; the footer has no email. Add both to the header/footer once the owner gives them (and make the form text the phone instead, if they take texts).
- **No service area**, address, hours, owner name, years in business, insurance/licence, reviews, prices.
- **No photos of their work.** The ad graphic is an illustrated house, not their job, so it isn't used. Hero stays plain navy until real photos arrive (then: photo hero under navy overlay, plus work cards above the Facebook link).

## Questions for the owner
- Phone number (and does it take texts)? Email?
- Which towns do you cover?
- Your first name, so the page can speak as you?
- Do you quote from photos, or come out to look?
- A few before/after photos of roof, chimney, gutter or pointing jobs?
- Licensed/insured in NJ? Any years-in-business or reviews we can show?
- Is "Front roof to roots" meant to be "From roof to roots"?

## Ideas not built (yours to pick)
- **Runner-up worlds (opt-in signature motion):** (1) rain that runs down the hero and pours off a drawn roof edge into a gutter, which the visitor can clear by dragging (best fit); (2) repointing: drag across a brick wall to fill cracked mortar joints; (3) rain beading on glass that wipes clear under the finger; (4) a weather vane that swings with the pointer.
- Before/after sliders once photos exist.
- A "Signs to look for after a storm" seasonal checklist page (the ad is already this content).
- Impeccable conflicts kept on purpose (Ellie's calm-style choices): eyebrow pills, the H1 letter bounce-in, the floating circle, Cal Sans, the diagonal band texture.

## Not verified
- Messenger's `?text=` prefill on real iPhone/Android, and inside Facebook's in-app browser (the page also copies the message, and shows it with Copy/Open buttons as a fallback).
- Clipboard copy inside the Facebook in-app browser.
- Real-device touch and frame rate on old phones (checked in Playwright Chromium and WebKit at 360/390/430/1440).
