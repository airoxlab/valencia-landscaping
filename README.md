# Valencia Landscaping — Placerville, CA

Single-page **bilingual (English/Spanish)** sample site for a licensed C-27
landscaping contractor in Placerville, California (El Dorado County).

## Business details

| | |
|---|---|
| Business | Valencia Landscaping |
| Owner | **Cesar Raul Valencia** (per BuildZoom) — **not named on the site**, see below |
| Phone | (530) 748-6991 (mobile — call and text both offered) |
| Location shown | Placerville, CA |
| Website | None |
| Google Maps | **Not listed** |

## Licence — verified

Checked against the CSLB database on **2026-10-13**, licence **#1146950**:

- **VALENCIA LANDSCAPING**, 5543 Davidson Rd, Placerville, CA 95667
- Business phone (530) 748-6991 — matches the number he was texted on
- Issued **11/26/2025**, expires **11/30/2027**
- **This licence is current and active.**
- Classification **C-27 — Landscaping** (this record holds C-27 only)
- Contractor's bond with **American Contractors Indemnity Company**, **$25,000**
- **Workers' compensation** with Employers Compensation Insurance Company,
  policy #EIG6514872, to **07/30/2027**

He carries real workers' comp, so he has a crew, and the site says
**"licensed, bonded and insured"**.

Note: BuildZoom says he "holds a Landscaping license and 1 other license". The
CSLB record for #1146950 lists **C-27 only**, so the site claims only that.
Worth asking him what the second one is — if it is a B or C-12, that widens what
he can legitimately advertise.

## ⚠️ The Facebook page in the brief is NOT his business

The brief lists `facebook.com/ValencialandscapingLLC/` as his page. **It is a
different company in South Carolina.** Evidence:

- Its own service card reads **"JERSON VALENCIA : 843-532-9291"** — area code
  **843 is South Carolina**. Your lead is **Cesar Raul Valencia, (530) 748-6991,
  Placerville, California**.
- Its contact email is **sanchezlandscaping420@gmail.com**, not a Valencia address.
- A post reads *"We Do It All Brand New Privacy Fence — James Island Area"*.
  James Island is in Charleston County, SC.

**Sixteen photos were scraped from that page and all sixteen were discarded.**
Using them would have published another contractor's job photos — and his phone
number, visible in the service-card image — on your client's website, 2,500 miles
from where he works.

**So he has no usable photos at all**, and the brief's "use photos from his
Facebook page" cannot be followed. All five images on the site are stock,
disclosed under the gallery and in the footer. **Job photos are the single
biggest upgrade available**, and he must be asked for them directly.

## Other things that could not be verified

- **BuildZoom is geo-blocked** from this machine ("BuildZoom is unavailable in
  your region"), so the score of 101 and the customer review mentioning *"10+
  years on their rental properties"* could not be read first-hand. Neither is
  claimed on the site.
- **No Google listing exists**, so there are no reviews to quote.

## What was deliberately not built

- **No owner name.** "Cesar Raul Valencia" comes from BuildZoom, which could not
  be loaded directly to confirm, and he has not published it himself. Confirm
  with him, then add a short owner story — it is the main thing the page lacks.
- **No years-in-business claim.** The licence dates to November 2025. The
  BuildZoom review suggesting 10+ years could not be verified, so no number is
  used. **Ask him** — "licensed 2025" badly undersells a decade of work.
- **No reviews section.** Nothing genuine exists to quote.
- **No street address.** 5543 Davidson Rd is shown as "Placerville, CA".
- **No second licence classification** (see above).

## His own words, used

Two phrases on the page are his:

- **"We Take Pride Good Job Done"** — his Facebook tagline, tidied to
  *"We take pride in a job well done"* for the footer.
- **"I do everything, my friend"** — what he replied in the SMS thread. It is the
  pull quote on the services band, because it is both charming and the actual
  commercial point: one licensed crew for the whole property instead of three
  numbers to call.

Note the tagline comes from the Facebook page that is **not his** — but the
phrase matches the business name and tone, and the brief attributes it to him.
**Confirm it is his before going live**; if not, it is one line to remove.

## Bilingual

Every visible string exists as `data-en` / `data-es` siblings, with a header
EN/ES switch. Defaults to Spanish for `es-*` browsers, remembers the choice in
`localStorage`, and updates `<html lang>` for screen readers.

**Tested in a browser:** default EN, toggle to ES (headline, nav and body all
swap, `html lang="es"`), toggle back, preference persisted, no JS errors.

The Spanish is written as a Spanish-speaking customer in California would say it
(*adoquines*, *orillado*, *deshierbe*, *césped*), not literal translation.

## Design — his own logo and brand colours

**The client sent a photo of his work shirt** and said *"My logo and I like the
lettuce and red"*. Both are now the basis of the site.

**Colours sampled directly from that photo:**

| | |
|---|---|
| Maroon / burgundy (his "red") | `#8C2F4C` |
| Leaf green (his "lettuce") | `#4FCC60` |

The whole palette was rebuilt around them — maroon `#4E1A2E` for headings, the
bright green for buttons and accents, and a warm off-white `#FBF7F8` page. The
dark-mode palette was re-derived to match.

**The logo was redrawn as SVG, not traced from the extraction.** The PNG supplied
(`Valencia Landscaping Green Horseshoe Logo.png`) is unusable — heavy glow,
blown-out highlights, the horseshoe and laurel detail lost, and it sits on black
rather than transparent. It was rebuilt from the client's original photo instead:

- `img/logo.svg` — the full crest: arched **VALENCIA**, green horseshoe with nail
  holes, sprout inside, laurel wreath both sides, **LANDSCAPING** curved below.

**The navbar is maroon**, at the client's direction, so the full crest sits
directly on it with no chip or backing — green icon, white lettering, exactly as
it appears on his shirt. Nav links, the language switch and the call button are
all white on the maroon. The crest runs at 62px in the header and 96px in the
footer; both were checked at 2x for legibility.

Other design notes:

- Fraunces (display serif) + Nunito Sans (body).
- Eight sections: hero, credential strip, services, "I do everything" band,
  process, licensing, work gallery, service areas, contact.
- Full dark mode, sticky header, `scroll-margin-top` anchors, reduced-motion
  respected, inline CSS, no build step.
- Sendra visit-tracking script before `</body>`.

Eleven stock candidates were discarded for showing the wrong subject (a bathroom
labelled "pavers", a power drill labelled "irrigation", a salad plate, a living
room, seedlings, farm planting, a building facade).

## Open questions for the client

1. **Confirm his name** (Cesar?) and whether he wants it on the site.
2. **Job photos** — essential; there are none anywhere online.
3. **How long has he been landscaping?** BuildZoom hints at 10+ years.
4. **Is the Facebook tagline his?** (The page carrying it is a different company.)
   Note his shirt reads "...NCE" on a banner under the crest — probably
   "EXPERIENCE", but it is cut off in the photo. **Ask him what it says**, and it
   can be added to the logo.
5. **What is the second CSLB licence** BuildZoom mentions?
6. **Maintenance contracts or installs** — which does he want more of?

## The name problem

Searching **"Valencia Landscaping Placerville"** on Google Maps returns **two
different local competitors**:

- "Valencia yard Maintenance/landscaping", 4.7★, (530) 308-6225
- "Valencia Landscape Care", 5.0★, (916) 756-5806

He is not on Maps at all. So customers looking for *him* by name are being handed
to two rivals with the same surname and visible star ratings — a worse version of
the problem All Pacific Roofing and Arcline Electric have, because these two are
local and credible.

**A verified Google Business Profile is the highest-value next step**, well ahead
of the website on its own. Pitch them together.

Not to be confused with: R Valencia Landscape LLC (Livermore), Valencia Tree &
Landscape (Santa Barbara), or the South Carolina Facebook page above.
