# FUTURE_PE_02 — AI Content Marketing using UGC Ads

**Track:** Prompt Engineering (PE)
**Business used:** Prime Relocations — premium packers & movers, Nellore, Andhra Pradesh
**Tools used:** Claude (claude.ai)

---

## 1. Objective

Produce a complete AI-generated UGC (user-generated-content style) ad pack — multiple scripts, hooks, and captions across platforms — for the same business used in Task 1, focused on conversions rather than generic brand awareness content.

---

## 2. Prompt Engineering Approach

UGC ads work because they *feel* unscripted, so the key prompt engineering challenge here was stopping the model from writing polished "brand voice" copy and instead getting it to sound like a real customer talking to camera. I handled this in three prompt stages.

### Step 1 — Persona & Constraint Prompt

```
You are writing UGC-style ad scripts — the kind a real customer would
film on their phone, not a brand's marketing team. Rules:
- Use first-person, conversational language ("I was so stressed about...")
- No corporate phrases ("state-of-the-art," "customer-centric")
- Include natural pauses, casual phrasing, and mild imperfection
- Each script should follow a Problem → Discovery → Solution → CTA arc
Business: Prime Relocations, a premium packers & movers service in
Nellore. Target customer: someone relocating homes or offices who is
anxious about damage, hidden costs, or unreliable movers.
```

### Step 2 — Hook Generation Prompt

```
Generate 6 different scroll-stopping opening lines (hooks) for a
UGC ad about a moving/relocation service. Each hook must:
- Be under 12 words
- Create curiosity or tension in the first 3 seconds
- Avoid sounding like an ad
Vary the angle across hooks: fear of damage, hidden costs, time pressure,
disbelief/surprise, relatable frustration, and social proof.
```

### Step 3 — Full Script + Caption Prompt

```
Using 3 of the hooks above, write full 30-45 second UGC ad scripts
(spoken lines only, with brief camera direction in brackets) for:
1. Instagram Reels / TikTok style (casual, fast-paced)
2. YouTube Shorts (slightly longer, more narrative)
3. Facebook (slightly more descriptive, older audience)
For each script also write a caption (with 3-5 relevant hashtags)
and a one-line CTA suited to that platform.
```

---

## 3. Final Output

### 🎣 Hooks (6 variations)

| # | Angle | Hook |
|---|-------|------|
| 1 | Fear of damage | "My movers dropped my TV. This time was different." |
| 2 | Hidden costs | "They quoted me one price. The final bill? Also that price." |
| 3 | Time pressure | "I had 48 hours to pack my entire house. Here's what happened." |
| 4 | Disbelief/surprise | "I didn't think movers could actually be... nice?" |
| 5 | Relatable frustration | "If you've ever cried over bubble wrap, this is for you." |
| 6 | Social proof | "My whole building uses the same moving company now." |

---

### 🎬 Script 1 — Instagram Reels / TikTok (Hook #2)

**Caption:** Nobody warns you about the "surprise fees" until moving day 😩 #MovingDay #PackersAndMovers #Nellore #RelocationTips #HomeMove

```
[Standing in half-packed living room, phone selfie angle]

"Okay so — every mover I called quoted me one price on the phone,
and then moving day comes and suddenly there's a 'stairs fee,' a
'heavy item fee,' a 'we-felt-like-it fee'...

[cut to boxes being loaded]

...except Prime Relocations. The quote they gave me? That's what
I paid. No surprises. My anxiety about moving day was honestly
the sponsor of this video.

[cut to final shot, thumbs up next to moving truck]

If you're moving soon, just — save yourself the stress."
```

**CTA:** "Link in bio for a free quote 📦"

---

### 🎬 Script 2 — YouTube Shorts (Hook #4)

**Caption:** I genuinely did not expect movers to be this good. #MovingCompany #PrimeRelocations #HomeRelocation #Nellore

```
[Sitting on a box, talking directly to camera, slightly narrative tone]

"So I've moved four times in my life, and every single time the
movers were... fine. Just fine. Nothing broken, but also nothing
that made me think 'wow, they actually cared.'

[cut to packing footage]

This time I used Prime Relocations, and my dad's old record player —
the one thing I was terrified about — arrived without a scratch.
They wrapped it like it was going into a museum.

[cut back to camera]

I didn't think movers could surprise me anymore. These guys did."
```

**CTA:** "Check the description for booking details."

---

### 🎬 Script 3 — Facebook (Hook #3)

**Caption:** 48 hours. One move. Zero disasters. Here's how it went. 🏠📦 #Relocation #Nellore #MovingStory

```
[Talking to camera in empty apartment, more descriptive pacing]

"So my landlord gave me exactly 48 hours' notice to move out —
I'm not exaggerating. I panicked, called Prime Relocations, and
told them the situation.

[cut to team packing quickly]

They sent a team out the same afternoon. Packed my entire two-bedroom
apartment, labeled every box, and had everything at my new place by
the next evening. I didn't lift a single box.

[cut to new apartment, unpacked boxes visible]

If you're ever in a moving emergency, I can't recommend them enough."
```

**CTA:** "Message their page for same-day availability."

---

## 4. Notes on Prompt Engineering Decisions

- Explicitly banning corporate phrasing ("state-of-the-art," "customer-centric") was necessary — without that constraint, the model defaulted back to brand-voice language even when asked for UGC style.
- Requesting hooks *before* full scripts let me pick the strongest angle per platform rather than getting one generic script and hoping it worked everywhere.
- Platform-specific pacing notes (fast-paced for Reels, narrative for Shorts, descriptive for Facebook) were added deliberately since audience attention spans and expectations differ meaningfully by platform.
