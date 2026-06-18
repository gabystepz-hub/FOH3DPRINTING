# FOH3D Printing — Sound Design & Audio Branding Guide

**Prepared for:** Website intro experience (logo reveal → site transition) and full sonic identity
**Audience:** Live audio engineers, touring engineers, production managers, RF coordinators, system engineers
**Reference tier:** Apple · Dolby · Bang & Olufsen · Universal Audio · Tesla
**Implementation:** Pro Tools / Logic Pro / Ableton Live / Adobe Audition

---

## Design Philosophy (read this first)

The single biggest risk with this project is sounding like every other "tech" intro: a whoosh into a synthetic *ding*. Your audience hears more audio in a day than most sound designers do in a month. They will instantly clock anything fake, over-compressed, or borrowed from a stock library. They respond to one thing above all: **truth.** Real transients, real space, real signal behavior.

So the governing rule for the entire FOH3D sonic identity is:

> **Sounds like real equipment, captured by someone who knows how it should sound.**

Not synthesized "futurism." Not Hollywood braams. The sonic world of a touring rig at load-in: the *thunk* of a road-case latch, the controlled hum of a powered amp rack coming up, the clean self-noise floor of a high-end converter, the mechanical precision of a 3D printer's stepper motors laying a perfect layer. That is your palette. It is unique to you and impossible to fake convincingly — which is exactly why it will land with this crowd.

---

## 1. Logo Reveal Sound

### Concept
**"Precision Power-Up."** A piece of professional equipment coming to life — the moment a console boots, a converter locks to clock, an amp rack arms. It should feel engineered, not magical. One confident gesture, no clutter.

### Sound style
Hybrid **organic-mechanical + tuned sub**. Foreground is a real mechanical/electro-mechanical transient (the "engagement"); underneath is a single tuned sub-bass swell that gives it body and confidence; on top is a high-frequency "lock" detail that signals precision. Think Universal Audio's hardware aesthetic crossed with the restraint of an Apple product chime.

### Emotional impact
Confidence, control, arrival. The listener should feel a small involuntary "that's solid." Not excitement — *reassurance from competence.* The emotional target is the feeling a system tech gets when the PA passes a sweep cleanly: everything is right.

### Sound layers (foreground → background)
1. **Engagement transient (the hero):** a real relay/latch/contactor *thunk* or a road-case latch snap, pitched and tightened. This is the "on." 8–15 ms attack.
2. **Mechanical precision detail:** a short stepper-motor or servo movement (the 3D-printer signature) — a brief, tightly-gated mechanical "zzt-click" placed 30–60 ms after the transient. This is the brand fingerprint; keep it subtle.
3. **Tuned sub swell:** a single sine/triangle sub at **41 Hz (E1)** or **55 Hz (A1)**, rising over ~250 ms with a soft knee. Gives weight and "power on" without boom.
4. **Converter "lock" shimmer:** a very short, clean high-frequency element — a soft bell partial or filtered noise burst at **8–12 kHz**, decaying fast. Signals digital precision and clock-lock.
5. **Air/space tail:** a short, controlled reverb tail (plate or small chamber, ~0.8–1.2 s) that places everything in a real room and then gets cut by the transition.

### Frequency focus
- **Sub (30–60 Hz):** body and confidence — but mono and controlled, one note only.
- **Low-mid (120–300 Hz):** keep *clean*. Carve here to avoid "boom." This is where cheap intros get muddy.
- **Presence (3–6 kHz):** the mechanical detail and transient bite — where "precision" lives perceptually.
- **Air (8–14 kHz):** the lock shimmer. A gentle high shelf, never harsh.
- Overall: **wide-band but uncluttered.** A spectrum analyzer should show a clean sub, a scooped low-mid, and two tasteful upper peaks.

### Duration
**1.4–1.8 seconds** total. Hero transient at 0 ms, sub peak around 250–300 ms, full decay/tail resolving by ~1.5 s. Short enough to never feel like a gate; long enough to feel premium.

### Reference brands / audio branding to study
- **Universal Audio** — hardware-truthful, warm, "pro gear" character.
- **Dolby** ("Dolby Atmos" idents) — controlled sub, sense of space and precision, restraint.
- **Apple** (Mac startup chime, Apple Silicon idents) — single confident gesture, perfectly tuned, zero clutter.
- **Bang & Olufsen** — refined, minimal, expensive-sounding transients.
- **Tesla** UI/unlock sounds — mechanical-meets-digital, premium but understated.
- **THX** (as a *contrast* — do NOT go this big; note its sense of arrival and control).

### Suggested sound effects (source material)
- Road-case latch / butterfly latch snaps (record your own — instant brand authenticity).
- Relay, contactor, or power-sequencer engagement clicks.
- 3D-printer stepper-motor moves and homing chirps (your literal product — record these).
- Powered amp rack / console power-on hum swell.
- Neutrik connector lock/seat clicks (XLR, speakON) for the high-detail layer.
- Clean converter self-noise / clock-lock blips.

### Recommended sound libraries
- **Soundly** (Pro) — high-quality mechanical, switch, and relay content.
- **Boom Library** — *Mechanical Trailer*, *Cinematic Metal*, *Sci-Fi* (use the organic, not the cheesy, hits).
- **A Sound Effect** — boutique mechanical/industrial packs (search "relay," "latch," "servo," "stepper").
- **Krotos Reformer Pro** — real-time resynthesis to morph mechanical sources into a signature hit.
- **Output Rev / Portal**, **Native Instruments Straylight & Form** — for the tuned sub and lock shimmer (used sparingly, processed to sound real).
- **GuitarRig/Amp tones** are not needed; avoid synth-preset "tech" packs entirely.

---

## 2. Website Transition Sound

### Concept
**"Signal handoff."** The logo's energy doesn't stop — it *passes through* into the interface, like patching a clean signal from one stage to the next. Where the logo reveal is a vertical *impact*, the transition is a horizontal *motion*. It should feel like air moving, not a whoosh cliché.

### Layer breakdown
1. **Filtered air-motion** (not a whoosh): pink/brown noise through a band-pass filter sweeping **400 Hz → 6 kHz**, very short, with a fast Doppler-style pitch lift. Keep level low — felt more than heard.
2. **Sub release:** as the logo's tuned sub resolves, let a soft downward sub glide carry the listener forward — a gentle 55 Hz → 41 Hz fall, like settling into the room.
3. **Single UI "seat" tick:** one clean, short transient at the resolve point — the interface "arriving" and locking into place. This becomes your master UI sound (see §3).
4. **Ambience bed-in (optional):** a barely-perceptible room tone / converter floor fades up under the homepage for 1–2 s, then settles to silence. Gives the site a sense of "the room is now live."

### Duration
**400–700 ms.** Fast and non-intrusive. It overlaps the *tail* of the logo sound by ~150–200 ms so there's no gap — the energy is continuous.

### Dynamics
- Peak well below the logo sound (aim **−6 to −9 dB** relative to the logo's peak).
- Soft attack, smooth release — no hard transient except the single seat tick.
- Sidechain the ambience bed to duck slightly under the tick so the resolve reads clearly.

### Processing recommendations
- **Band-pass + automated filter sweep** (e.g., FabFilter Pro-Q 3 or stock EQ with envelope) for the air-motion.
- **Doppler / pitch automation** for forward motion without a literal whoosh.
- **Short reverb send** (200–400 ms) shared with the logo's tail so they sit in the same space.
- **High-pass everything below ~30 Hz** to protect laptop/phone speakers.
- **Gentle limiter** for consistency, but preserve transient life — do not crush.

### UX considerations
- **Mute by default or honor browser autoplay policies.** Provide a visible, elegant sound toggle (most browsers block autoplay audio anyway).
- **Play once per session**, not on every navigation. Cache the user's mute preference.
- **Total intro audio under ~2.5 s** so it never blocks interaction.
- **Loudness target −16 to −14 LUFS integrated** for web; true peak ≤ −1 dBTP.
- **Test on laptop speakers and phones first**, not studio monitors — most visitors hear it there.
- **Respect `prefers-reduced-motion`/accessibility:** pair audio with the visual and let it be skippable.
- Keep file size tiny: short AAC/Opus, ~48 kHz, well under 200 KB.

---

## 3. Audio Branding Strategy

### Sonic identity
**"Engineered, not synthesized."** Every FOH3D sound is rooted in a real, physical, professional-audio or precision-manufacturing source. The brand sounds like the inside of a well-run touring rig: clean, mechanical, confident, spacious, and quiet where it should be quiet. The through-line across logo, UI, and any video content is *real transients placed in real space.*

### Signature sound elements
- **The Engagement** — the logo's hero transient (relay/latch). The brand's "voice."
- **The Stepper Signature** — a short, recognizable 3D-printer servo motif. Your unique fingerprint; reuse it (quietly) across touchpoints.
- **The Seat Tick** — the single clean lock/seat click used at the transition and as the primary UI confirm. Connector-seat or latch-close in origin.
- **The Room** — a consistent, subtle ambience/converter-floor that says "the system is live."

### Tonal direction
Warm, precise, controlled, expensive. Low-end is present but disciplined (one note, mono, tuned to **E/A** so it's harmonically consistent). Highs are detailed but never harsh. Mids are clean and uncluttered. The overall impression is *high headroom and low noise* — the sonic equivalent of a great converter.

### Sound palette
- **Tonal center:** tune sustained/sub elements to **E** (41/82 Hz) or **A** (55/110 Hz) so all brand sounds are musically related.
- **Texture family:** metal, relay/contact, servo/stepper, connector seat, amp-rack hum, room tone.
- **Color:** dark and warm with precise highlights — think graphite, brushed aluminum, a single LED indicator.

### Recommended instruments / synthesizers / textures
- **Sub/body:** pure sine or triangle sub (Serum, Operator, or a recorded amp-rack hum tuned to pitch). One oscillator. No detuned supersaws.
- **Texture/space:** granular/convolution tools — **Native Instruments Straylight, Form, Reaktor**; **Output Portal**; **Krotos Reformer Pro** to fuse mechanical sources.
- **Impacts:** real metal/relay recordings layered with a tuned sub thump; avoid trailer-braam presets.
- **Risers (use sparingly):** filtered-noise rise + rising room tone, NOT a synth riser preset. Keep them short and clean.
- **Convolution reverb:** **Altiverb** or **FabFilter Pro-R** with a small, real room/plate — one shared space for the whole brand.

### UI sound system (for the site and any product UI)
Keep it minimal — 4 to 6 sounds maximum, all derived from the same physical sources so they feel like one family:
- **Hover / focus:** ultra-subtle high tick (connector touch), −20 dB, < 40 ms.
- **Confirm / click:** the **Seat Tick** (primary signature).
- **Success / add-to-cart:** seat tick + soft tuned sub note (E or A).
- **Error / unavailable:** a short, damped *un-seated* click (the latch that doesn't catch) — lower, duller, no sub.
- **Page/section transition:** the §2 air-motion, scaled down.
- **Rule:** all UI sounds share the same reverb space and tuning, sit at conversational level, and are individually mutable.

---

## 4. Final Recommendation

### The one combination

**A. Logo Reveal — "Precision Power-Up"**
A real **road-case latch / relay engagement** as the hero transient (8–12 ms attack), layered with a **3D-printer stepper-motor micro-move** at +40 ms for the brand fingerprint, a **tuned sub swell at 41 Hz (E1)** rising over 250 ms for confident body, and a **clean 10 kHz "clock-lock" shimmer** decaying fast on top. Resolved in a small real plate/chamber (≈1 s tail). Total length **~1.6 s.**

**B. Website Transition — "Signal Handoff"**
A **low, band-passed air-motion** (400 Hz→6 kHz, ~500 ms) that overlaps the logo's tail by ~180 ms, carrying a **gentle 55→41 Hz sub glide** into a **single clean Seat Tick** at the resolve, with a **whisper of room tone** fading up under the homepage. Peaks ~6–9 dB below the logo. Total length **~600 ms.**

### Why this is the strongest choice for this audience

This crowd's entire professional identity is built on making real signals sound right in real rooms. A synthetic, generic "tech" intro reads to them as *amateur* — the audio equivalent of a fake plugin GUI. By sourcing the identity from **actual professional-audio and 3D-printing hardware** (latches, relays, connectors, stepper motors, amp-rack hum), the brand earns instant credibility: these are sounds they live inside every day, captured with care. The **tuned, mono, disciplined sub** signals headroom and control — the things a system engineer respects most. The **clock-lock shimmer** is an inside reference to digital audio precision. And the **restraint** (short, clean, uncluttered, low noise floor) mirrors the aesthetic of the gear they trust: Apple, Dolby, B&O, Universal Audio. It says "we are engineers, like you" without saying a word. It avoids corporate stingers, cheesy synth swells, and game-style effects entirely because every element is physically real and tastefully placed.

---

## 5. Production Guide (Pro Tools / Logic / Ableton / Audition)

### Session setup
- **48 kHz / 24-bit**, stereo master. Export web deliverables at 48 kHz.
- Build the logo and transition as **two separate stems** that overlap, plus a combined master render.
- Reference monitoring: check on monitors, laptop speakers, and phone before sign-off.

### Track layout
| Track | Content | Key processing |
|---|---|---|
| 1 — Engagement | Latch/relay hero transient | Transient shaper (fast attack), tight gate, HPF @ 80 Hz |
| 2 — Stepper | 3D-printer servo micro-move | Heavy gate, band-pass 1–5 kHz, low level |
| 3 — Sub | Sine/triangle @ 41 Hz (E1) | Volume automation swell, mono, soft saturation |
| 4 — Lock shimmer | Bell partial / filtered noise @ 8–12 kHz | Fast decay, high shelf, de-ess if harsh |
| 5 — Air motion | Band-passed pink/brown noise | Filter sweep automation + pitch lift (transition) |
| 6 — Room/verb | Send-only ambience + tail | Convolution (small plate/chamber), shared bus |

### Step-by-step

**Logo reveal**
1. Drop the latch/relay transient at 0:00. Tighten with a transient designer (boost attack, reduce sustain). HPF @ ~80 Hz to remove rumble.
2. Place the stepper micro-move at +40 ms. Gate hard, band-pass 1–5 kHz, set ~12–15 dB below the hero. It should register subliminally.
3. On the sub track, draw a volume swell on a 41 Hz sine starting at 0:00, peaking at ~250–300 ms, soft knee. Add gentle saturation (e.g., a tape/console emulation) for harmonics so it reads on small speakers. Keep mono.
4. Add the lock shimmer at the sub's peak — a short bell partial or filtered noise burst at 10 kHz, ~150 ms decay. High shelf for air; tame any harshness with dynamic EQ.
5. Bus tracks 1–4 to a reverb send (small plate/chamber, ~0.9–1.1 s, predelay ~20 ms). Blend ~12–18% wet.
6. Carve **150–350 Hz** on the bus to keep the low-mid clean. Confirm a scooped low-mid on the analyzer.

**Transition**
7. On the air-motion track, automate a band-pass filter 400 Hz → 6 kHz over ~500 ms, plus a small upward pitch automation for forward motion (no literal whoosh).
8. Add a 55 → 41 Hz sub glide that begins as the logo sub resolves; keep it gentle and low.
9. Place one clean Seat Tick at the resolve point — the moment the homepage "arrives."
10. Fade a whisper of room tone up under the resolve, then settle to near-silence over 1–2 s. Sidechain it to duck under the tick.
11. Overlap the transition so it starts ~180 ms before the logo tail ends — continuous energy, no gap.

### Mix & master
- **Logo bus:** gentle bus compression (1.5–2:1, slow attack to keep transients), then a limiter for consistency — preserve transient life, do not crush.
- **Loudness:** master to **−16 to −14 LUFS** integrated, **true peak ≤ −1 dBTP**.
- **Low end:** HPF the whole master at ~30 Hz. Keep sub mono below ~120 Hz.
- **A/B** against an Apple or Dolby ident for tonal balance and restraint — if yours is busier or louder, pull back.

### Deliverables to export
- `FOH3D_logo.wav` (48 kHz/24-bit master) + `FOH3D_logo.m4a`/`.opus` (web).
- `FOH3D_transition.wav` + web version.
- `FOH3D_intro_combined.wav` (logo+transition rendered together) + web version.
- UI sound set: `ui_hover`, `ui_click`, `ui_success`, `ui_error`, `ui_nav` (short AAC/Opus, normalized to a consistent −20 to −16 LUFS, individually mutable).
- Keep each web file well under 200 KB.

### Quick-win shortcut
The fastest path to an authentic, un-fakeable identity: **record your own product and rig.** A phone or field recorder capturing a real road-case latch, a few Neutrik connector seats, and your 3D printer homing and laying a layer will give you 80% of this palette with built-in brand truth. Layer those with one tuned sub and one tasteful shimmer, and you have something no competitor can copy from a stock library.
