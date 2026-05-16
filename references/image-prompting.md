# Image Prompting Reference

## The formula

`[Subject + Action] + [Location / Context] + [Composition] + [Lighting] + [Style / Aesthetic] + [Camera / Lens] + [Color grading]`

Not every element is required for every image. But specificity in each category improves accuracy dramatically.

---

## Subject & Action

Start with a strong, clear noun. Then describe what the subject is doing.

- Weak: "a woman in a dress"
- Strong: "a striking fashion model in a tailored emerald silk dress, posing with a confident, slightly turned stance"

Describe physical attributes that matter: posture, expression, clothing detail, age range, mood. Don't leave ambiguity that the model will fill in arbitrarily.

---

## Location & Context

Ground the scene. Where is this happening? What's in the background?

- Vague: "outdoors"
- Specific: "a desolate salt flat at dusk, cracked earth stretching to the horizon, a faint purple sky overhead"

Use real-world reference points when helpful: "an early-1900s Parisian apartment," "a brutalist Soviet-era gymnasium," "a neon-lit Tokyo alleyway."

---

## Composition

Tell the model how to frame the shot. Use photography terminology.

**Shot types:**
- Full shot, medium shot, medium-close-up, close-up, extreme close-up
- Low angle, high angle, bird's eye, worm's eye, eye level
- Over-the-shoulder, POV, two-shot

**Compositional rules (invoke them directly):**
- "Center-framed, symmetrical"
- "Rule of thirds, subject offset left"
- "Dutch angle, approximately 15°"

---

## Lighting

Lighting sets emotional tone more than anything else. Be explicit.

**Natural light:**
- Golden hour backlighting creating long shadows
- Overcast diffused light, no harsh shadows
- Hard midday sun, high contrast
- Blue hour, cool ambient glow

**Studio / artificial:**
- Three-point softbox setup, evenly lit
- Single dramatic spotlight from above
- Chiaroscuro — deep shadow, single source light
- Neon ambient fill, colored gels

**Atmospheric:**
- God rays through forest canopy
- Fog diffusing a streetlight from behind
- Candlelight, warm and flickering

---

## Camera & Lens

Specify this to control depth, distortion, and intimacy.

**Cameras (each has a visual DNA):**
- GoPro → immersive, distorted, action
- Fujifilm X100 → warm color science, slightly filmic
- Hasselblad / medium format → rich tonal depth
- Disposable camera → flash-lit, raw, nostalgic
- ARRI Alexa → cinematic, clean, professional
- iPhone → everyday, naturalistic

**Lenses:**
- 85mm portrait lens, shallow depth of field (f/1.4)
- 24mm wide-angle, slight barrel distortion
- 50mm, natural perspective
- 200mm telephoto, compressed depth
- Macro lens, extreme detail

**Focus:**
- Razor-sharp focus on subject, background bokeh
- Soft focus overall, dreamlike
- Deep focus, sharp front to back

---

## Style & Aesthetic

The style signature gives the model a visual vocabulary to work from.

**Photographic:**
- Editorial fashion, shot on medium-format analog film, grain, high saturation
- Documentary photography, available light, candid
- Product photography, clean white background, studio
- Architectural photography, geometric precision

**Cinematic:**
- Shot on 35mm film, 1970s color grading
- Cinematic color grading, muted teal and orange tones
- Anamorphic lens, horizontal lens flare

**Art / illustration:**
- Oil painting, loose brushwork, impressionist
- Watercolor illustration, soft edges
- Graphic novel, high contrast ink
- Studio Ghibli aesthetic, soft backgrounds
- Hyperrealistic digital render, 8K

**Era-specific:**
- 1970s Kodachrome film, saturated, warm
- 1990s point-and-shoot aesthetic
- Early 2000s digital, slight noise, flat color

---

## Color Grading

Describe the final color treatment.

- Vibrant, fully saturated, punchy
- Desaturated, washed-out, melancholic
- Warm tones, amber and gold
- Cool tones, blue and teal
- High contrast, deep blacks
- Flat, matte finish, lifted shadows
- Duotone (specify two colors)

---

## Text in images

For tools that support it (Nano Banana / Gemini Image, Firefly):
- Enclose text in quotes: "URBAN EXPLORER"
- Specify font style: bold Impact, flowing Brush Script, thin Century Gothic
- Place text instruction after the main scene description
- Text-first hack: generate the text concept in conversation first, then request the image

---

## Multi-reference prompting

When using reference images (Nano Banana, Midjourney --ref, Firefly reference):
- Identify the relationship: "using the attached fabric texture, apply it to this character's clothing"
- Use up to 4 references for best results; each reference should serve a distinct purpose (character, texture, style, environment)
- Be explicit about what carries over and what changes

---

## Prompt examples (annotated)

### Fashion editorial
```
[Subject] A striking fashion model wearing a tailored brown tweed dress,
sleek ankle boots, holding a structured leather handbag.
[Action] Posing with a confident, statuesque stance, slightly turned to camera.
[Context] Seamless deep cherry red studio backdrop.
[Composition] Medium-full shot, center-framed.
[Style] Fashion magazine editorial.
[Camera] Shot on medium-format analog film, pronounced grain, high saturation.
[Lighting] Cinematic three-point lighting.
```

### Product shot
```
[Subject] Sleek minimalist nude-colored glass moisturizer jar.
[Context] Resting on a warm marble surface, scattered dried botanicals nearby.
[Lighting] Soft diffused studio light, radiant glow.
[Composition] Close-up, slightly elevated angle.
[Style] High-end commercial beauty photography.
[Camera] Shot on a Hasselblad, deep tonal range, no harsh shadows.
```

### Cinematic portrait
```
[Subject] A weathered fisherman in his 60s, deep-set eyes, calloused hands.
[Action] Staring out at the sea, unposed, caught in thought.
[Context] Rugged coastal cliff, overcast sky, distant fog.
[Composition] Medium close-up, rule of thirds, subject left-framed.
[Lighting] Flat, diffused overcast light, no shadows, grey tonal palette.
[Style] Documentary photography. Shot on Kodak Portra 400.
[Grading] Desaturated, lifted shadows, slightly cool.
```
