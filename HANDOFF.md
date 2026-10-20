# ClearedCo — handoff at ~60%

**Live:** https://10elizabethbell.github.io/clearedCo/ · **Repo:** https://github.com/10elizabethbell/clearedCo · **Built:** 2026-10-17 from Muse brief 2026-10-17 (Essex County Contractor Referrals post) · **Revamped:** 2026-10-19 in the calm band style

## Revamp, 2026-10-19: what changed
The business hasn't been contacted, so the whole page was rebuilt under the new house default (`calm-photo-style.md`, learned from lpmr.co.uk), copied from DPG's `index.html`.
- **Gone:** the fogged-window canvas hero, the soapy-glass artwork, the pane-by-pane fog clearing, the moving water-line seams, the painted window frames, the heavy uppercase system headings. All of it is in git history (`fdba680`) if you want any of it back as an opt-in signature.
- **Look:** paper (#f5f4fb) and indigo bands from the logo (navy #2e2768, deep #1c1840 with the faint line texture), one warm gold (#f5c451) used as a fill with indigo text on it, the logo's violet (#5a4fc0) for form hover/focus. Cal Sans headings, system body 16/1.7, pill buttons, 24px cards.
- **Hero:** ClearedCo's own washed front driveway (the "after" from pair 4) under an indigo overlay; eyebrow "Window cleaning & pressure washing", H1 "See the difference in **Canfield & Boardman.**" (bounces in letter by letter), the promise "We clean your home the way we'd clean our own, from the glass to the driveway.", Get a free quote (gold) + See our work (outlined). On phones the photo is blurred 3px so the concrete joints don't run through the text (finishing rule). White text measures 8.8:1 or better, gold 5.2:1, the promise 6:1 against the brightest pixel behind it (sampled at 360, 390, 1440).
- **Order:** header → hero → What we clean (6 rows on indigo: windows inside and out, house washing, driveways, decks, patios, mold on wood; the arrow fills gold on hover, and tapping a row ticks it in the form) → Recent work (the same three before/after sliders, now 24px cards with a plain gold divider; from tablet width up the tall garage one sits beside the other two at the same height, capped at 880px wide so the 586/695px photos aren't blown up) → "Click to see more of our work." Facebook row → How it works (deep band, 3 gold numbered steps) → free-quote form in a white card → closing indigo band (name, area, big "Message us") → footer.
- **Motion:** H1 bounce-in, one 12px fade-up for things below the first screen, the slider's one-time hint sweep. All off under reduced motion; everything shows without JS.
- **Floating circle:** gold, bottom right, opens Messenger (switches to a pre-filled text once `CONFIG.PHONE` is set). Hidden on the hero and wherever it would sit on another control: the service rows, the Facebook row, the form, and the closing band (which has its own big Message us).
- New `img/og.png` (the new hero), `img/hero-driveway.webp` (40KB, provenance sidecar), Cal Sans loads without blocking the first paint.

## What's built
- One page, phone first: header (round logo + "Cleared Co / Canfield, Ohio", **Message us** top-right), hero, services, recent work, how it works, quote form, closing band, footer.
- Contact: **no phone exists**, so everything goes to Messenger (`m.me/61589631985029`). The form builds a pre-written message, copies it, and opens Messenger with `?text=`; if that doesn't fill in, the message stays on the page with Open Messenger / Copy message.
- **One-line switch:** set `CONFIG.PHONE = '3305551234'` and the header and closing band become the tap-to-call number, the footer lists it, step 1 reads "Text or call us.", and the form and floating circle send by text (`sms:`) instead.
- Before/after sliders: drag or tap anywhere on the photo; arrow keys via a hidden range input; on touch only a sideways drag or a tap moves it, so a scroll that starts on a photo still scrolls.

## Assumptions I made
- **Gold accent:** the logo has no warm colour (indigo, violet, lavender, white). The calm style wants one warm accent, so I picked a soft gold that sits well on the indigo. Alternative: the logo's lavender (#c9c2ff) as the fill, which keeps strictly to the brand but isn't warm.
- **Hero photo:** the front-driveway after shot, cropped to drop the "After" sticker and the parked pickup; the white car is side-on (no plate), the mailbox shows no number. It's 1170px wide, so it's softened by about 1.2x on a 1440 screen; the overlay hides that.
- **Area:** Boardman and Canfield, from the Facebook page meta ("Cleared Co LLC | Canfield OH", "Professional pressure washing services in Boardman, OH"). "and nearby" is my inference.
- **Services:** from the page description ("Interior/Exterior windows, driveways, decks, patios & house washing") plus "mold & buildup on wood" from the post. The description is truncated after "Free..."; there may be more.
- **Voice:** "we", because it's an LLC with no named owner. Switch to "I" if it's one person.
- **Copy I wrote:** the hero promise ("We clean your home the way we'd clean our own, from the glass to the driveway.") and the How it works lines. I cut "at the price we quoted" from step 3 because the owner never promised it. Nothing on the page is a claim the owner made; confirm or rewrite in their words. The headline is built on their own phrase "What a difference!".
- **Name:** "ClearedCo" everywhere it's displayed (their own spelling in the post caption); the footer also gives the legal "Cleared Co LLC". The logo reads "CLEARED CO"; switch the wordmark if the owner prefers that.
- Favicon: a white "C" on the logo's gradient (the wordmark can't be read at 16px). The iPhone icon is the full logo.

## Placeholders and gaps
- **Phone: none published anywhere.** The biggest gap. Messenger stands in; `CONFIG.PHONE` is ready.
- Email: none. Add it to the footer (and only there) once known.
- No reviews, prices, hours, owner name, insurance, years. None are on the page.
- Page timeline is closed to fetches (403); no more photos without the owner.

## Questions for the owner
- Phone number, and do you take texts?
- Email for the footer?
- More before/after pairs, ideally shot from the same spot (each becomes another slider), and a window-cleaning one (all three are pressure washing).
- Towns you'll drive to beyond Boardman and Canfield (Poland, Austintown, Youngstown…)?
- Owner name and one line about why you started.
- One person or a crew ("I" vs "we")?
- Insured? Any services missing (gutters, roofs, soft washing, screens)?

## Ideas not built (yours to pick)
- **Runner-up signature (opt-in):** the old fogged window you wipe clear with a finger (in history at `fdba680`), or a squeegee pass pulling a clean band across soapy glass. Other worlds from the trade: a pressure-washer wand that cleans a grimy driveway strip under your finger; water beading and sheeting off a clean pane; a before/after "wipe" on the hero photo itself.
- Lavender instead of gold as the fill accent (see Assumptions).
- `book.html` booking page in the same style, if the owner wants more than Messenger.
- Sharper desktop work photos: re-crop the garage and driveway pairs from `src-assets/pair-3…6` (978–1290px) at matching framing, add `srcset`, then lift the 880px cap.
- Impeccable flags these, but they're your calm-style choices and stay: the eyebrow pills (hero, Recent work, Free quote), the H1 letter bounce-in, the floating circle, Cal Sans, and the faint line texture on the deep bands (suppressed in `.impeccable/config.json` with the reason).

## Review status
- **Impeccable, every mode except `live`:** audit, critique (by the finish reviewer), harden, optimize, adapt, typeset, layout, colorize, clarify, distill, quieter, animate, delight, bolder, overdrive, extract (an assessment only: the tokens already live in `:root`), polish and document. `onboard` doesn't apply (no first-run flow).
  - Fixes applied: Cal Sans no longer blocks first paint; a no-JS line in the form; side-by-side work from 760px.
  - Bolder/delight/overdrive point at a signature motion. That's opt-in now, so it's listed under Ideas instead.
- **Detector:** the remaining findings were all from the old fog-world `DESIGN.md`. They clear once the new `DESIGN.md` is in. The line texture is suppressed in `.impeccable/config.json` (your calm-style choice), and I dropped the old build's stale suppressions.
- **Finish reviewer:** one round, verdict "fix", 8 material fixes, all applied:
  - WebKit collapsed the work grid at 1024px and up (Safari desktop lost the proof section).
  - The floating circle sat on row arrows.
  - A concrete joint in the photo ran through the phone hero text.
  - Work photos were upscaled on desktop (now capped at 880px).
  - "Mold on wood" was left alone in the desktop grid (window rows merged).
  - Generic promise and the unpromised "price we quoted" (rewritten).
  - Two spellings of the name.
  - Stale `DESIGN.md`.
- **Checked by me:** Chromium and WebKit at 360, 390, 430 and 1440, plus 768 and 844 landscape:
  - no sideways scroll; the hero and primary button sit inside the first screen on every phone
  - bounce-in caught mid-flight, settled, and the plain H1 restored, with the same line breaks
  - with reduced motion and with no JS, all content shows
  - the circle shows and hides as intended
  - the form's errors and its Messenger text decode correctly
  - template-leftover grep is clean
- **Left standing:**
  - The desktop work grid leaves about 200px empty on the right at 1440 (the cost of not upscaling the photos). Sharper re-exports from `src-assets/pair-*` would let it go full width; matching the pairs' framing needs care.
  - Form fields are #e8e6f4 on white (about 1.2:1 against the card). This is the house fix for DPG's field fill; the labels and the focus outline carry it.

## Not verified
- Real-device touch (tested with simulated touch in Chromium and WebKit via Playwright).
- Whether `m.me/61589631985029?text=` actually pre-fills on iOS/Android Messenger for a new-style profile page. If it doesn't, the copy fallback covers it.
- The Facebook in-app browser specifically (clipboard may be blocked there; the message box covers it).
