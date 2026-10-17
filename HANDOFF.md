# ClearedCo — handoff at ~60%

**Live:** https://10elizabethbell.github.io/clearedCo/ · **Repo:** https://github.com/10elizabethbell/clearedCo · **Built:** 2026-10-17 from Muse brief 2026-10-17 (Essex County Contractor Referrals post)

## What's built
- One page, phone first: header (logo + "Cleared Co / Canfield, Ohio", **Message us** top-right), hero, What we clean, Where we work, How it works, Recent work, free-quote form, footer.
- World: the logo's indigo-to-violet as the ground, lavender-white painted window frames, heavy uppercase system type.
- Signature: the hero is a **fogged dusk window** (canvas). It wipes itself in loose passes until touched; a finger or mouse wipes it clear in any direction (vertical drags wipe instead of scrolling); the fog creeps back; drops run down in stop-go jerks, leave clear trails, soak up beads, and get nudged by the finger. Tunables are in `T` at the top of the `glass` IIFE (`REGROW`, `BRUSH`, `GHOST_IDLE`, `SPAWN`...).
- Moving water-line seams between sections (`S.SPEED`, `S.AMP` in `seams`).
- Contact: **no phone exists**, so everything goes to Messenger (`m.me/61589631985029`). The form builds a pre-written message, copies it, and opens Messenger with `?text=`; if that doesn't fill in, the message stays on the page with Copy / Open Messenger.
- **One-line switch:** set `CONFIG.PHONE = '3305551234'` and the header becomes the tap-to-call number, the footer shows it, and the form sends by text (`sms:`) instead.
- Service rows link to the form and tick that service.

## Assumptions I made
- **Area:** Boardman and Canfield, from the Facebook page meta ("Cleared Co LLC | Canfield OH", "Professional pressure washing services in Boardman, OH"). Muse missed these; the Essex County group is unrelated to the area. "and nearby" is my inference.
- **Services:** taken from the page description ("Interior/Exterior windows, driveways, decks, patios & house washing") plus "mold & buildup on wood" from the post. The description is truncated after "Free..."; there may be more.
- **Voice:** "we", because it's an LLC with no named owner. Switch to "I" if it's one person.
- **Promise copy is mine:** "done like it's our own home. We don't pack up until you can see the difference." and step 3, "we're not done until you can see the difference." They echo the owner's "What a difference!", but the owner hasn't said them. Confirm or rewrite.
- **"Free quote… a price before any work starts"**: follows from "free quote" but is worded by me.
- Headline "See the difference." (alternative: their own phrase, "What a difference.").
- Colors are from the logo. The cyan focus color on form fields is mine (it needed to stand out from the indigo button).
- Favicon: a white "C" on the logo's gradient (the wordmark can't be read at 16px). The iPhone icon is the full logo.

## Placeholders and gaps
- **Phone: none published anywhere.** This is the biggest gap. Messenger stands in for now; `CONFIG.PHONE` is ready.
- Email: none. The footer has no email line; add one there (and only there) once known.
- **Only one photo, and it's a BEFORE frame** (video thumbnail from the group post; the after is in the video, which can't be downloaded). It's labelled "Before" so nobody mistakes it for the result, and the Facebook link says "Click to see the after, and more of our work." Original video: https://www.facebook.com/groups/1043573412799214/posts/2504644293358778/
- No reviews, prices, hours, owner name, insurance, years. None are on the page.
- Page timeline is closed to fetches (403); no more photos without the owner.

## Questions for the owner
- Phone number, and do you take texts?
- Email for the footer?
- The "after" from the porch-ceiling video (and any before/after pairs). These would turn Recent work into before/after sliders.
- Towns you'll drive to beyond Boardman and Canfield (Poland, Austintown, Youngstown…)?
- Owner name and one line about why you started. The finishing rules want the owner's own voice.
- One person or a crew ("I" vs "we")?
- Insured? Any services missing (gutters, roofs, soft washing, screens)?

## Ideas not built (yours to pick)
- **Runner-up world:** a squeegee pass on a wet window: one blade pulls a clean band across soapy glass, with a water line along its edge. More "window cleaner", less "dusk".
- Before/after slider in a window frame once a pair exists (plain solid divider, per the finishing rules).
- A small second window under the services rows on desktop, fogging back over a photo of each service.
- A rain-on-glass ambient effect in the proof frame's top edge (skipped: it risks a film over the photo, which Ellie bans).
- `book.html` booking page in the same world, if the owner wants more than Messenger.

## Not verified
- Real-device touch (tested with simulated touch in Chromium and WebKit via Playwright).
- Whether `m.me/61589631985029?text=` actually pre-fills on iOS/Android Messenger for a new-style profile Page. If it doesn't, the copy fallback covers it.
- Frame rate on old phones (the canvas is capped at 1.5x density with fewer beads on phones, and pauses off screen).
- The Facebook in-app browser specifically (clipboard may be blocked there; the message box covers it).
