# Midjourney Prompt Library

**Tool:** Midjourney
**Version:** v6.1 (as of November 2025)
**Purpose:** Generate consistent, high-quality images for video content
**Outcome:** Copy-paste prompts that produce usable results

---

## Midjourney Basics

### Prompt Structure
```
/imagine [subject] [style] [composition] [lighting] [parameters]
```

### Essential Parameters
- `--ar 16:9` - Aspect ratio (16:9 for YouTube, 9:16 for TikTok, 1:1 for Instagram)
- `--v 6.1` - Use latest version
- `--style raw` - More photorealistic, less "AI art" look
- `--stylize 50` - Lower = more literal, higher = more artistic (0-1000)
- `--quality 1` - Standard quality (0.25, 0.5, 1, or 2)
- `--seed 12345` - Reproducible results (use same seed for consistency)

### Quality Tips
- Use `--style raw` for realistic photos
- Add `--stylize 50` for commercial content
- Include camera/lens details for photorealistic shots
- Reference specific photographers or brands for style

---

## Prompt Library by Use Case

### 1. YouTube Thumbnails (16:9)

#### Generic Excited Person
```
/imagine portrait of professional content creator, genuine excited expression, pointing at camera, warm studio lighting, colorful background with motion blur, shot on Canon EOS R5, 50mm f/1.2, shallow depth of field --ar 16:9 --style raw --v 6.1 --stylize 50
```

#### Faceless Tech Thumbnail
```
/imagine overhead flat lay of modern desk setup, laptop displaying code, smartphone, coffee mug, wireless earbuds, minimal aesthetic, soft natural lighting, product photography style, clean white desk --ar 16:9 --style raw --v 6.1 --stylize 25
```

#### Before/After Split
```
/imagine split screen composition, left side: cluttered messy desk setup dim lighting, right side: organized minimalist workspace bright natural light, clear visual contrast, professional photography --ar 16:9 --style raw --v 6.1
```

**Usage notes:**
- Replace subject (content creator, desk, etc.) with your niche
- Adjust lighting and colors to match brand
- Export at 1280x720 minimum for YouTube

---

### 2. Social Media Graphics (1:1)

#### Quote Card
```
/imagine minimalist inspirational quote card, bold sans-serif typography, "Your Quote Here" centered, gradient background in [brand colors], professional graphic design, clean composition, Behance style --ar 1:1 --v 6.1 --stylize 75
```

#### Product Showcase
```
/imagine single product floating on pastel [color] background, dramatic studio lighting, product photography, commercial style, clean shadows, sharp focus, shot on Phase One XF IQ4, 80mm lens --ar 1:1 --style raw --v 6.1 --stylize 50
```

#### Abstract Background
```
/imagine abstract fluid gradients, [color palette], smooth color transitions, wallpaper design, 4K digital art, no subjects, peaceful aesthetic --ar 1:1 --v 6.1 --stylize 100
```

---

### 3. Video B-Roll Alternatives (9:16)

#### Cinematic City Scene
```
/imagine cinematic shot of modern city skyline at golden hour, dramatic clouds, volumetric lighting, wide angle lens, establishing shot, Blade Runner aesthetic, moody color grade, shot on ARRI Alexa Mini --ar 9:16 --style raw --v 6.1 --stylize 75
```

#### Nature Landscape
```
/imagine epic mountain landscape, misty morning light, pine forest foreground, dramatic peaks in background, national geographic photography style, wide angle, rich colors, shot on Sony A7R V --ar 9:16 --style raw --v 6.1 --stylize 50
```

#### Technology Abstract
```
/imagine futuristic technology abstract, glowing circuit boards, flowing data visualization, blue and purple neon lights, depth of field, macro photography, tech aesthetic --ar 9:16 --style raw --v 6.1 --stylize 100
```

**Usage notes:**
- Use for intro/outro backgrounds
- Layer text overlay in your video editor
- Add motion blur in post for video feel

---

### 4. Brand Assets

#### Logo Background
```
/imagine seamless pattern, [describe elements], [brand colors], minimal design, repeating geometric shapes, professional branding style, clean and modern --ar 16:9 --v 6.1 --stylize 50 --tile
```

#### Hero Image
```
/imagine modern website hero section, [industry] themed, professional atmosphere, bright and inviting, corporate photography style, people collaborating, diverse team, natural lighting --ar 16:9 --style raw --v 6.1 --stylize 50
```

#### Icon Set
```
/imagine minimalist icon representing [concept], line art style, simple geometric shapes, single color [color], vector art aesthetic, clean and professional, white background --ar 1:1 --v 6.1 --stylize 25
```

---

## Style Consistency Techniques

### Method 1: Use a Consistent Seed
```
/imagine [your prompt] --seed 123456 --v 6.1
```
**Tip:** Save successful seeds in a spreadsheet. Reuse for similar shots.

### Method 2: Reference an Image
```
/imagine [URL of reference image] [your prompt] --iw 1.5 --v 6.1
```
**`--iw`** (image weight): 0.5-2, controls how much to match reference

### Method 3: Style Reference
```
/imagine [prompt] --sref [URL of style reference] --v 6.1
```
**Use for:** Maintaining brand visual identity across images

### Method 4: Consistent Parameters
Save these as a preset:
```
--ar 16:9 --style raw --v 6.1 --stylize 50 --quality 1
```

---

## Photography Styles by Niche

### Tech/SaaS
```
Keywords: clean, minimal, white background, product photography, professional lighting, sharp focus
Style: --style raw --stylize 25
```

### Lifestyle/Wellness
```
Keywords: natural lighting, organic, warm tones, candid moments, lifestyle photography
Style: --style raw --stylize 75
```

### Finance/Business
```
Keywords: corporate, professional, suit and tie, modern office, confident expression, editorial photography
Style: --style raw --stylize 50
```

### Creative/Agency
```
Keywords: bold colors, dramatic lighting, artistic composition, creative direction, fashion editorial
Style: --stylize 150
```

---

## Advanced Techniques

### Multi-Prompt Weighting
```
/imagine coffee mug::2 laptop::1 workspace --ar 16:9 --v 6.1
```
**`::2`** means coffee mug is twice as important as laptop

### Negative Prompting
```
/imagine professional headshot --no glasses, beard, hat --ar 1:1 --style raw --v 6.1
```
**Use to remove unwanted elements**

### Chaos Parameter
```
/imagine abstract art --chaos 50 --v 6.1
```
**`--chaos`** (0-100): Higher = more varied/unexpected results

### Repeat for Variations
```
/imagine [prompt] --repeat 4 --v 6.1
```
**Generates 4 variations at once (requires fast mode)**

---

## Quality Control Checklist

Before using generated images:

- [ ] No obvious AI artifacts (extra fingers, distorted faces)
- [ ] Colors match your brand palette
- [ ] Composition is clean (no distracting elements)
- [ ] Resolution is high enough for intended use
- [ ] Lighting is consistent with your other content
- [ ] Style aligns with brand voice
- [ ] No recognizable copyrighted elements

**Fix issues:**
- Regenerate with modified prompt
- Use `/describe` command on image to understand what worked
- Upscale with `U1`, `U2`, etc. buttons
- Use variations `V1`, `V2`, etc. for alternatives

---

## Prompt Templates (Fill-in-the-Blank)

### Portrait
```
/imagine [subject], [expression], [clothing style], [environment], [lighting], shot on [camera], [lens] --ar [ratio] --style raw --v 6.1 --stylize 50
```

### Scene
```
/imagine [location/setting], [time of day], [weather/mood], [composition angle], [photography style], dramatic [lighting type] --ar [ratio] --style raw --v 6.1 --stylize 75
```

### Product
```
/imagine [product] on [background], [lighting setup], commercial product photography, [mood/aesthetic], studio quality --ar [ratio] --style raw --v 6.1 --stylize 25
```

### Abstract
```
/imagine abstract [theme], [color palette], [style keywords], digital art, [mood] --ar [ratio] --v 6.1 --stylize 100
```

---

## Common Mistakes to Avoid

❌ **Too long/complex prompts**
→ Keep it under 60 words

❌ **No style parameters**
→ Always use `--style raw` for realistic content

❌ **Ignoring aspect ratio**
→ Use `--ar` for your target platform

❌ **Generic descriptions**
→ Be specific: "golden hour lighting" not just "good lighting"

❌ **Forgetting version parameter**
→ Always include `--v 6.1` for latest model

❌ **No quality control**
→ Check for AI artifacts before using

---

## Midjourney vs Other Tools

**Use Midjourney for:**
- Artistic/creative images
- Conceptual illustrations
- Stylized graphics
- When you need multiple variations

**Use DALL-E 3 for:**
- Precise text in images
- Simpler/faster results
- Integration with ChatGPT

**Use Stable Diffusion for:**
- Complete control over parameters
- Local generation (privacy)
- Custom model fine-tuning

---

## Batch Image Generation Workflow

1. **Define style guide:**
```
Base parameters: --ar 16:9 --style raw --v 6.1 --stylize 50 --seed 987654
```

2. **Create prompt variations:**
```
Scene 1: [base prompt] morning light
Scene 2: [base prompt] sunset
Scene 3: [base prompt] overcast
```

3. **Generate in bulk:**
Use `--repeat 10` for multiple variations

4. **Select best:**
Upscale winners with `U1`, `U2`, etc.

5. **Organize:**
Download and rename: `YYYY-MM-DD-[description]-v[number].png`

---

## Cost Optimization Tips

**Fast mode:** $30/month unlimited (lower quality, faster)
**Relax mode:** Included in subscription (slower, same quality)

**Strategy:**
1. Use fast mode for initial concepts/variations
2. Switch to relax mode for final high-quality renders
3. Use `--quality 0.5` for drafts, `--quality 1` for finals
4. Delete failed generations to free up fast hours

---

## Resources & Learning

**Official:**
- [Midjourney Docs](https://docs.midjourney.com)
- Discord server: discord.gg/midjourney
- `/help` command in Discord

**Community:**
- [Midjourney Community Feed](https://midjourney.com/showcase/)
- Use `/describe` on good images to learn prompts
- Study top-rated images for prompt structure

**Tools:**
- [PromptHero](https://prompthero.com) - Prompt library
- [Midlibrary](https://midlibrary.io) - Style references
- [Lexica](https://lexica.art) - Search existing generations

---

## Example: Creating Consistent Thumbnail Series

**Goal:** 5 thumbnails for "AI Tools" series

**Base prompt:**
```
professional content creator at modern desk, excited expression, pointing gesture, [specific tool] visible on screen, bright studio lighting, colorful background, shot on Canon EOS R5 --ar 16:9 --style raw --v 6.1 --stylize 50 --seed 445566
```

**Variations:**
1. Replace `[specific tool]` with: "ChatGPT interface"
2. Replace with: "Midjourney interface"
3. Replace with: "Runway ML interface"
4. Replace with: "ElevenLabs interface"
5. Replace with: "CapCut interface"

**Result:** Consistent style, different tools featured

---

## Brand Voice Reminder

**Promise:** From blank to posted in one sitting
**Enemy:** Overwhelm

**Keep prompts:**
- Specific (not vague)
- Repeatable (document what works)
- Efficient (don't over-complicate)

**Ship with receipts. Every time.**

---

**Last Updated:** November 4, 2025
**Midjourney Version:** v6.1
**Repository:** [AI-Video-Factory-Resources](https://github.com/jmanhype/AI-Video-Factory-Resources)
