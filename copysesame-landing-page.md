# Copy Sesame — Landing Page Build Guide (Carrd)

A single-page, single-purpose site you can build in Carrd in about an hour. The goal of this page is one thing: get a cold prospect to book a call or reply to an email. Everything below is in service of that.

---

## 0. Brand quick-set

Lean into the "Sesame" angle — it's memorable, warm, and gives you a hook ("Open Sesame" = unlock conversions). Keep the palette tight.

**Palette**

- Background: `#FAF6EE` (warm cream / sesame milk)
- Ink (text + headlines): `#1A1A1A`
- Accent (buttons, links, highlights): `#C9582B` (toasted sesame / terracotta)
- Muted (section dividers, captions): `#7A7368`

**Typography** (both free in Carrd's Google Fonts picker)

- Headlines: **Fraunces** — 700 weight, slight serif personality, feels premium
- Body / UI: **Inter** — 400 body, 600 buttons

**Sizing rule of thumb**

- H1: 56–64px desktop / 36px mobile
- H2: 36–40px / 28px mobile
- Body: 18px / 16px mobile
- Line height: 1.25 on headlines, 1.6 on body

**Carrd setup**

- Pro tier (so you can use a custom domain, forms, and Google Fonts)
- Site → Style → set background and font defaults globally so you don't repeat per-section
- Use **Container** elements for each section so spacing stays consistent (96px top/bottom desktop, 56px mobile)

---

## 1. Nav bar (sticky, minimal)

Left: `Copy Sesame` wordmark in Fraunces 600, 22px.
Right: two text links — `Services` `FAQ` — and one button.

| Element | Text | Style |
|---|---|---|
| Logo | Copy Sesame | Ink, Fraunces 600 |
| Link | Services | Ink, Inter 500 |
| Link | FAQ | Ink, Inter 500 |
| Button | Book a free audit | Solid accent, white text, 10px radius |

In Carrd: use a **Container** with three columns (logo / spacer / links+button). Toggle "Sticky" on so it follows the scroll.

---

## 2. Hero

The hero does 90% of the work for cold traffic. Keep it to four things: pre-headline, headline, sub-headline, CTA.

```
[ Small pre-headline, accent color, uppercase, letter-spaced ]
EMAIL & LANDING PAGE COPY THAT PAYS FOR ITSELF

[ Headline, big, Fraunces ]
Open the floodgates.

[ Sub-headline, body size, max ~60ch ]
I write emails and landing pages for founders and small teams
who are tired of writing copy that sounds smart but doesn't sell.
Clear words. Real conversions. Usually live in under a week.

[ Primary button — accent ]   [ Secondary text link — ink ]
Book a free 15-min audit       See how it works ↓
```

**Layout:** centered, max-width 760px. Lots of whitespace above and below. No hero image — a clean type-driven hero reads as confident and loads instantly.

**Optional flourish:** under the headline, a thin row of trust signals once you have them — "Worked with [logo] · [logo] · [logo]". Until then, leave it out. An empty logo bar is worse than no logo bar.

---

## 3. Services (the two things you sell)

Two side-by-side cards. Keep them visually identical so neither looks like the "main" one.

**Section heading:** `What I write` (H2, centered)
**Sub-heading:** `Two services. Both built to move a specific number.`

### Card A — Email Marketing

```
[ Small icon or emoji — optional, e.g. an envelope ]

Email Marketing
For ecommerce brands and creators who have a list but aren't squeezing it.

What you get
• Welcome / abandoned cart / post-purchase flows
• Weekly campaign calendar + writing
• Subject lines tested against your last 30 days

Starts at $X / month
[ Button: Talk about email ]
```

### Card B — Landing Pages

```
[ Optional icon — a page or a key ]

Landing Pages
For founders launching something and one page has to do all the talking.

What you get
• Research call + voice-of-customer mining
• Long-form sales page or focused lead-gen page
• Two rounds of revisions, Carrd/Webflow-ready

Starts at $X / project
[ Button: Talk about a landing page ]
```

**Carrd build:** use a **Container with two columns**. Inside each, stack: heading → one-line description → bullet list → price line → button. Border the cards lightly (`1px solid #E8E0D2`, radius 14px, padding 32px). Both buttons can go to the same contact form — use a hidden form field to capture which service they clicked.

> Pricing note: leave "$X" as placeholders until you've sold one of each. "Starts at" is honest and lets you move it. If you really don't want to show numbers, use `From $—` or replace the line with `Project-based pricing`. Do not write "contact for pricing" — it reads evasive.

---

## 4. How it works (3 steps)

A reassurance section. Cold prospects want to know what they're agreeing to before they book.

**Section heading:** `How it works`

Three columns, numbered. Big numerals in accent color, then a short label and one sentence.

```
01  Free audit
    A 15-minute call. I look at your current emails or page
    and tell you what I'd change — whether you hire me or not.

02  Scope + quote
    If it makes sense to work together, I send a one-page proposal
    with deliverables, timeline, and a fixed price.

03  Draft in 5–7 days
    You get a draft within a week. Two rounds of revisions included.
    Most clients are live inside two weeks.
```

**Carrd build:** Container with three columns. The big "01/02/03" is a separate text element above each step — Fraunces 700, 48px, accent color.

---

## 5. Why me (mini-bio + a real photo of you)

People hire people. One paragraph, one photo, one quote.

**Layout:** two columns — photo on the left (square crop, ~320px), copy on the right.

```
[ Photo of you, square, soft corners 12px ]

I'm [Your Name].
I've been writing copy for [X years / since I realized
spreadsheets weren't for me]. Before Copy Sesame I [one line —
e.g. ran email for a 7-figure DTC brand / wrote landing pages
freelance for SaaS founders]. I work with a small number of
clients at a time so the work stays sharp.

I care about two things: copy that sounds like a human wrote it,
and copy that moves the number you actually care about.
```

If you don't have a usable photo yet, ship the page without this section and add it within the first week. Don't use a stock photo or an AI portrait — it kills the trust this section is supposed to build.

---

## 6. Proof (testimonials or sample work)

You won't have testimonials on day one. That's fine — show work instead.

**If you have testimonials:** three short pull-quotes in a row. Name + role + small avatar. Keep each under 25 words.

**If you don't yet:** rename the section `Recent work` and show 2–3 thumbnails of pages or emails you've written (even spec pieces or rewrites of public pages). Each thumbnail links to a one-page case study you can add later. For now the links can go to a simple "Case study coming soon" anchor — what matters is that the page looks complete.

**If you have neither:** delete this section entirely until you do. An empty proof section is worse than no proof section. Replace it with a second small CTA block:

```
Not ready to book?
Reply to my email with one sentence about what you're working on
and I'll send back two specific things I'd change. No pitch.
```

---

## 7. FAQ

Four to six questions, accordion style (Carrd has this as a built-in element under "Toggles"). Address the objections that come up in cold outreach.

```
How fast can you turn something around?
Most landing pages: 5–7 business days for the first draft.
Email flows: 7–10 days depending on how many.

Do you work with my niche?
I focus on ecommerce, SaaS, and creators. If you're outside that,
ask anyway — I'll tell you honestly if I'm the right fit.

What do you need from me to start?
A 30-minute kickoff call, access to your existing copy and analytics,
and one round of customer interviews (I'll run them).

Do you offer revisions?
Two rounds included on every project. Most clients use one.

What if I'm not happy with the draft?
If the first draft misses the mark, I rewrite it once at no charge.
If it still misses, you pay 50% and we part ways.

How do I pay?
50% to start, 50% on delivery. Stripe invoice.
```

---

## 8. Final CTA

After the FAQ, one more chance to convert. Big, centered, single button. No distractions.

```
[ H2 ]
Want better copy by next week?

[ Body, one line ]
Free 15-minute audit. No slide deck. No pitch.

[ Big button — accent ]
Book the audit →
```

---

## 9. Footer

Three lines, muted text, small.

```
Copy Sesame · copysesame.com · hello@copysesame.com
[ Twitter/X ] [ LinkedIn ]
© 2026 Copy Sesame
```

---

## 10. The CTA target — what "Book a free audit" actually does

You have two reasonable options:

1. **Calendly / Cal.com embed** in a Carrd "Embed" element on a second section that scrolls into view, OR opens in a popup (Carrd supports popups via the element settings → "Use as overlay"). This is the lower-friction option and what I'd pick.
2. **Simple contact form** — name, email, what they want help with (radio: email / landing page / both), one open text field. Carrd's built-in form works fine; pipe it to your inbox. Use this if you'd rather screen leads before giving up calendar slots.

Either way, every button on the page should go to the **same** destination. Don't make people choose which form to fill out.

---

## Section order recap (for Carrd's section list)

1. Nav (sticky)
2. Hero
3. Services
4. How it works
5. Why me
6. Proof / Recent work *(skip on launch if empty)*
7. FAQ
8. Final CTA
9. Footer

---

## Pre-launch checklist

- [ ] Custom domain `copysesame.com` pointed at Carrd (Carrd → Publish → Domain)
- [ ] Favicon uploaded (a single sesame seed silhouette or a stylized "C" works)
- [ ] Page title: `Copy Sesame — Email & landing page copy that pays for itself`
- [ ] Meta description: same line as the hero sub-headline
- [ ] OG image: 1200×630, hero headline on cream background, accent button rendered
- [ ] Form submissions tested end-to-end (send yourself one)
- [ ] Mobile preview checked — Carrd shows mobile in the preview pane; tap through every button
- [ ] One typo pass out loud (read it to yourself; if you stumble, rewrite)

---

## What to do first when you sit down to build it

1. Buy a Carrd Pro plan and point `copysesame.com` at it.
2. Set background, font, and accent color in Site → Style. Everything else inherits.
3. Build only the Hero and the Final CTA. Publish.
4. Send the link to five people you trust and ask: *"In one sentence, what does this person sell?"* If four out of five get it right, build the rest. If they don't, fix the hero before anything else.

That's it. Don't redesign — fill it in.
