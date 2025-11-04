# Advanced AI Video Workflow Template

**Purpose:** Streamline your multi-tool AI video production workflow
**Duration:** ~30 minutes per video
**Outcome:** Professional AI-generated video ready to post

---

## Pre-Production (5 minutes)

### Define Outcome
**Target platform:** [TikTok / YouTube / Instagram / LinkedIn]
**Video length:** [15s / 30s / 60s / 3-5min]
**Aspect ratio:** [9:16 / 16:9 / 1:1]

**One-line outcome:**
From [starting point] to [posted result]

Example: "From product photo to 30-second demo video posted on Instagram"

---

### Gather Assets

**Required:**
- [ ] Source images/video (with usage rights)
- [ ] Script or talking points
- [ ] Brand assets (logo, colors, fonts)

**Optional:**
- [ ] Voiceover audio
- [ ] Background music
- [ ] B-roll footage

**Usage rights check:**
- [ ] All assets are owned or licensed
- [ ] Digital twin subjects have provided consent
- [ ] Stock footage is royalty-free or purchased

---

## Production (15 minutes)

### Step 1: Generate Base Video
**Tool:** [Runway / Pika / Stable Diffusion Video]
**Version:** [Tool version number]

**Settings:**
```
Prompt: [Your detailed prompt here]
Duration: [2s / 4s / 8s per clip]
Resolution: [1920x1080 / 1080x1920]
Motion: [Low / Medium / High]
Seed: [Optional - for consistency]
```

**Output:**
- [ ] Generated clip saved as `raw-01-[description].mp4`
- [ ] Backup prompt saved for future use

---

### Step 2: Enhance/Upscale (Optional)
**Tool:** [Topaz Video AI / Runway Upscaler]

**Settings:**
```
Target resolution: [4K / 1080p]
Enhancement: [Slow Motion / Stabilization / Sharpen]
```

---

### Step 3: Add Voiceover/Audio
**Tool:** [ElevenLabs / Murf / Adobe Audition]

**Voiceover settings:**
```
Voice: [Rachel / Adam / Custom clone]
Stability: [50%]
Clarity: [75%]
Style: [Conversational / Professional / Energetic]
```

**Background music:**
```
Source: [Epidemic Sound / Artlist / YouTube Audio Library]
Track: [Track name]
Volume: [-20dB to -15dB below dialogue]
```

- [ ] Audio synced to video
- [ ] Volume levels balanced

---

### Step 4: Edit & Composite
**Tool:** [Premiere Pro / DaVinci Resolve / CapCut]

**Timeline structure:**
```
Track 1: Base AI-generated video
Track 2: B-roll overlays
Track 3: Text/graphics
Track 4: Voiceover
Track 5: Background music
```

**Effects to add:**
- [ ] Intro card (3 seconds)
- [ ] Text overlays (brand name, key points)
- [ ] Transitions (cuts, fades - keep it simple)
- [ ] Color grade (maintain consistency)
- [ ] Outro card (3 seconds) with CTA

**Brand consistency:**
- [ ] Logo in [top-right / bottom-left]
- [ ] Font: [Montserrat Bold / Your brand font]
- [ ] Colors: [#HEX codes from brand guide]

---

## Post-Production (10 minutes)

### Step 5: Quality Control

**Technical check:**
- [ ] Audio levels: -3dB peak, -14dB average
- [ ] No visual glitches or artifacts
- [ ] Text readable on mobile screens
- [ ] Brand assets correctly placed
- [ ] Smooth transitions

**Content check:**
- [ ] Script matches voiceover
- [ ] Key message is clear in first 3 seconds
- [ ] CTA is obvious and actionable
- [ ] No spelling/grammar errors
- [ ] Platform-appropriate content (no ToS violations)

---

### Step 6: Export

**Settings by platform:**

#### TikTok / Instagram Reels / YouTube Shorts
```
Resolution: 1080x1920 (9:16)
Frame rate: 30 FPS
Format: MP4 (H.264)
Bitrate: 8-10 Mbps
Audio: AAC, 48kHz, stereo, 192kbps
Max file size: 50 MB
```

#### YouTube / Facebook (Landscape)
```
Resolution: 1920x1080 (16:9)
Frame rate: 30 FPS (or 60 FPS for smooth motion)
Format: MP4 (H.264)
Bitrate: 12-15 Mbps
Audio: AAC, 48kHz, stereo, 192kbps
Max file size: 500 MB
```

#### LinkedIn
```
Resolution: 1920x1080 (16:9) or 1080x1080 (1:1)
Frame rate: 30 FPS
Format: MP4 (H.264)
Max duration: 10 minutes
Max file size: 200 MB
```

**Export checklist:**
- [ ] Filename: `YYYY-MM-DD-[platform]-[title].mp4`
- [ ] Saved to organized folder
- [ ] Backup project file saved

---

### Step 7: Post & Track

**Caption template:**
```
[Hook in first line - make it scroll-stopping]

[One paragraph describing the outcome/benefit]

Tools used:
• [Tool 1]
• [Tool 2]
• [Tool 3]

[CTA: Comment / Share / Follow]

#[3-5 relevant hashtags]
```

**Posting checklist:**
- [ ] Caption written
- [ ] Hashtags added (3-5 max)
- [ ] Thumbnail/cover image set
- [ ] Posted at optimal time
- [ ] Cross-posted to other platforms (if applicable)
- [ ] Link shared in community (Skool, Discord, etc.)

**Track performance:**
- [ ] Impressions: _____
- [ ] Engagement rate: _____%
- [ ] Comments: _____
- [ ] Shares: _____
- [ ] Link clicks: _____

---

## Workflow Optimization Tips

### Time-Savers
1. **Batch generate:** Create multiple clips in one session
2. **Template effects:** Save preset transitions and color grades
3. **Reuse prompts:** Keep a library of successful prompts
4. **Keyboard shortcuts:** Learn 10 most-used shortcuts in your editor
5. **Auto-export:** Set up export presets for each platform

### Common Mistakes to Avoid
❌ Over-editing (keep it simple)
❌ Inconsistent branding across videos
❌ Skipping quality control
❌ Uploading without caption ready
❌ Forgetting to backup project files

### Quality Improvements
✅ Add subtle motion to static elements
✅ Use consistent color palette
✅ Keep text on screen for 2-3 seconds minimum
✅ Match audio to on-screen action
✅ Test on mobile device before posting

---

## Tool Versions Used

Document your tool versions for reproducibility:

| Tool | Version | Date |
|------|---------|------|
| Runway ML | [v2.5] | [2025-11-04] |
| Premiere Pro | [v24.0] | [2025-11-04] |
| ElevenLabs | [API v1] | [2025-11-04] |

---

## Example Workflows

### Workflow A: Product Demo (30 seconds)
1. Product photo → Runway (zoom + rotate)
2. ElevenLabs voiceover (15 seconds)
3. CapCut: overlay text, add music
4. Export 1080x1920, post to TikTok

**Time:** ~20 minutes

### Workflow B: Tutorial Snippet (60 seconds)
1. Screen recording (tool demo)
2. Digital twin narration (HeyGen)
3. Premiere: picture-in-picture layout
4. Export 1920x1080, post to YouTube

**Time:** ~30 minutes

### Workflow C: Brand Story (3 minutes)
1. Stock footage + AI-generated B-roll
2. Scripted voiceover (professional narrator)
3. DaVinci: color grade, motion graphics
4. Export 1920x1080, post to LinkedIn

**Time:** ~45 minutes

---

## Checklist Summary

**Before starting:**
- [ ] Outcome defined
- [ ] Assets gathered
- [ ] Rights verified

**During production:**
- [ ] Base video generated
- [ ] Audio added and synced
- [ ] Edited and branded

**Before posting:**
- [ ] Quality control passed
- [ ] Exported in correct format
- [ ] Caption written
- [ ] Posted and tracked

---

## Customization Notes

**Adapt this template by:**
- Removing steps not needed for your workflow
- Adding your brand-specific guidelines
- Documenting your most-used tools and settings
- Creating presets for common video types

**Save time by:**
- Creating project templates in your editor
- Building a prompt library
- Organizing assets in consistent folder structure
- Using automation scripts (see `../scripts/` folder)

---

## Brand Voice Reminder

**Promise:** From blank to posted in one sitting
**Enemy:** Overwhelm
**Voice:** Direct over polite · Demonstrate, don't speculate

Keep this workflow fast, focused, and repeatable.

---

**Last Updated:** November 4, 2025
**Repository:** [AI-Video-Factory-Resources](https://github.com/jmanhype/AI-Video-Factory-Resources)
