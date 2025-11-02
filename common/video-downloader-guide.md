# Video Downloader Skill - Usage Guide

**Skill:** video-downloader
**Purpose:** Download reference videos from YouTube and other platforms for course creation
**Status:** Installed at `~/.config/claude-code/skills/video-downloader/`

---

## When to Use This Skill

- Downloading YouTube tutorials for reference
- Saving competitor content for analysis
- Archiving educational videos
- Getting examples for "what to do" / "what not to do" lessons
- Downloading your own content from platforms

---

## How to Use (Step-by-Step)

### Method 1: Direct Request

Simply ask Claude:
```
Download this YouTube video: https://youtube.com/watch?v=VIDEO_ID
```

Claude will use yt-dlp to download the video to your specified folder.

### Method 2: Batch Download

For multiple videos:
```
Download these 3 YouTube videos for course reference:
1. https://youtube.com/watch?v=VIDEO_ID_1
2. https://youtube.com/watch?v=VIDEO_ID_2
3. https://youtube.com/watch?v=VIDEO_ID_3
```

### Method 3: Quality Specification

```
Download this video in 720p quality: [URL]
```

Or for audio only:
```
Download the audio from this video as MP3: [URL]
```

---

## AI Video Factory Use Cases

### For Course Creation

**Digital Twin Foundations:**
```bash
# Download HeyGen tutorial for reference
cd ~/Documents/Brand\ OS\ \(AI\ Video\ Factory\)/AI-Video-Factory-Resources/digital-twin-foundations/videos
yt-dlp -o "reference-heygen-tutorial.mp4" [YOUTUBE_URL]
```

**AI Video Mastery (Shorts + Reels):**
```bash
# Download viral short-form examples
cd ~/Documents/Brand\ OS\ \(AI\ Video\ Factory\)/AI-Video-Factory-Resources/ai-video-mastery-shorts-reels/videos
yt-dlp -o "example-viral-short-%(title)s.mp4" [YOUTUBE_URL]
```

**Image Factory:**
```bash
# Download Midjourney/DALLE tutorials
cd ~/Documents/Brand\ OS\ \(AI\ Video\ Factory\)/AI-Video-Factory-Resources/image-factory/videos
yt-dlp -o "reference-midjourney-tutorial.mp4" [YOUTUBE_URL]
```

---

## Important Copyright Notes

⚠️ **Legal & Ethical Requirements:**

1. **Only download for Fair Use purposes:**
   - Educational reference
   - Commentary and criticism
   - Research
   - Personal study

2. **Do NOT:**
   - Redistribute downloaded content
   - Use in commercial projects without permission
   - Claim content as your own
   - Upload to other platforms

3. **AI Video Factory Standard:**
   - Download for analysis only
   - Create original content inspired by techniques
   - Always credit original creators
   - Respect copyright and platform ToS

**Remember our brand:** Rebel + Lover = Challenge systems, respect creators

---

## Troubleshooting

### Issue: "HTTP Error 403: Forbidden"

YouTube may block downloads. Solutions:

1. **Update yt-dlp:**
```bash
pip install --upgrade yt-dlp
```

2. **Use cookies (if you have permission):**
```bash
yt-dlp --cookies-from-browser firefox [URL]
```

3. **Alternative: Screen recording**
   - Use OBS Studio or QuickTime to record your screen
   - Play the video and capture it legally
   - Only for personal reference use

### Issue: "Video unavailable"

- Video may be private or region-locked
- Check if video still exists
- Try accessing from browser first

### Issue: "Format not available"

```bash
# List available formats
yt-dlp -F [URL]

# Select specific format
yt-dlp -f FORMAT_ID [URL]
```

---

## Reference Videos Found (Examples)

### HeyGen Digital Twin Tutorial
**URL:** https://www.youtube.com/watch?v=7zVARy9Njzw
**Title:** "How to Create an AI Video Avatar with HeyGen"
**Use:** Digital Twin Foundations course reference
**Status:** Located, download blocked (use official HeyGen docs instead)

### Alternative Resources

Since direct download may be blocked, use official documentation:

1. **HeyGen Official:**
   - Community Hub: https://community.heygen.com/
   - Help Center: https://help.heygen.com/
   - Official tutorials (no download needed)

2. **Platform Demos:**
   - Run demos yourself and screen record
   - Create your own tutorial footage
   - More authentic for courses

3. **Your Own Content:**
   - Best for course material
   - Full rights to use
   - Demonstrates real results

---

## Best Practice: Create Your Own

**AI Video Factory approach:**

Instead of downloading others' content:

1. **Create your own demos** (10-min Build Friday sessions)
2. **Record your screen** while using tools
3. **Share real receipts** from your own projects
4. **Post and share link** (you own the content)

**This aligns with:**
- ✅ Promise: "From blank to posted in one sitting"
- ✅ Voice: "Zero fluff; receipts win"
- ✅ Enemy: Overwhelm (creating is faster than searching)

---

## Claude Code Integration

The video-downloader skill is active in Claude Code. Just ask:

```
Download this YouTube video for course reference: [URL]
```

Claude will:
1. Check if yt-dlp is installed
2. Navigate to appropriate course folder
3. Download with proper naming
4. Report file size and location
5. Respect copyright guidelines

---

**Last Updated:** November 1, 2025
**Skill Status:** ✅ Installed and Active
**Repository:** https://github.com/jmanhype/AI-Video-Factory-Resources
