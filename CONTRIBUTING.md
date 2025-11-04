# Contributing to AI Video Factory Resources

Thank you for contributing to the AI Video Factory community! This guide ensures all assets maintain quality and consistency.

---

## Quick Start

1. **Choose your course folder**
   - `advanced-ai-video-creation/`
   - `digital-twin-foundations/`
   - `ai-video-mastery-shorts-reels/`
   - `image-factory/`
   - `common/` (universal resources)

2. **Follow naming conventions** (see below)
3. **Add your asset**
4. **Update the course README**
5. **Submit a pull request**

---

## File Naming Conventions

### Videos
**Format:** `##-descriptive-name.mp4`

**Examples:**
```
✅ 01-intro-to-advanced-tools.mp4
✅ 03-prompt-engineering-masterclass.mp4
❌ intro.mp4
❌ Lesson 1.mp4
```

### Templates
**Format:** `descriptive-name-template.{md|pdf|xlsx}`

**Examples:**
```
✅ workflow-template.md
✅ consent-agreement-template.pdf
✅ posting-schedule-template.xlsx
❌ template.md
❌ My Template.docx
```

### Scripts
**Format:** `descriptive-name.{sh|py|js}`

**Examples:**
```
✅ batch-video-export.sh
✅ video-optimization.py
❌ script.sh
❌ my_script.py
```

### Docs
**Format:** `descriptive-name.{md|pdf}`

**Examples:**
```
✅ ethics-whitepaper.pdf
✅ privacy-best-practices.md
❌ document.pdf
❌ README2.md
```

---

## Asset Requirements by Type

### Videos (`.mp4`)

**Technical specs:**
- **Resolution:** 1920x1080 (16:9) or 1080x1920 (9:16)
- **Frame rate:** 30 FPS minimum
- **Format:** MP4 (H.264 codec)
- **Audio:** AAC, 48kHz, stereo
- **Max file size:** 500 MB (use Git LFS for larger files)

**Content requirements:**
- Clear audio (no background noise)
- Screen recordings at native resolution
- Include intro/outro cards (optional but recommended)
- Closed captions encouraged

**Where to upload:**
1. Add file to appropriate `videos/` folder
2. For files >100MB, use Git LFS or host externally (YouTube, Vimeo)
3. Update course README with direct link

---

### Templates (`.md`, `.pdf`, `.xlsx`)

**Markdown templates** (`.md`):
- Use standard markdown syntax
- Include clear section headers
- Add placeholders in `[brackets]`
- Provide usage examples

**PDF templates** (`.pdf`):
- Fillable form fields preferred
- Include instructions on first page
- Keep file size under 5 MB
- Use standard fonts (Arial, Helvetica)

**Spreadsheet templates** (`.xlsx`):
- First sheet = Instructions
- Protected cells for formulas
- Example data in first row
- Compatible with Google Sheets

**Required sections:**
- Purpose/overview
- How to use
- Customization notes
- Example/sample filled out

---

### Scripts (`.sh`, `.py`, `.js`)

**All scripts must include:**

1. **Header comment block:**
```python
#!/usr/bin/env python3
"""
Script Name: video-optimization.py
Purpose: Batch optimize videos for social media
Usage: python video-optimization.py input_folder output_folder
Requirements: ffmpeg, python 3.8+
Author: AI Video Factory
Last Updated: 2025-11-04
"""
```

2. **Dependencies listed:**
```bash
# Requirements:
# - ffmpeg 4.0+
# - python 3.8+
# - pip install pillow
```

3. **Usage examples:**
```bash
# Example usage:
# ./batch-video-export.sh input/ output/ 1080x1920
```

4. **Error handling:**
- Check for required dependencies
- Validate input parameters
- Provide helpful error messages

5. **Testing:**
- Test on sample data before committing
- Include sample input files if possible
- Document expected output

---

### Docs & Guides (`.md`, `.pdf`)

**Content structure:**
- **Hook:** Why this matters (first paragraph)
- **Body:** Step-by-step instructions
- **Examples:** Screenshots or code blocks
- **Takeaways:** 3-5 key points
- **Next steps:** Clear call to action

**Style guidelines:**
- Use second person ("You will...")
- Active voice, short sentences
- Bullet points over long paragraphs
- Code blocks for technical content
- Screenshots with captions

**Brand voice checklist:**
- [ ] Direct over polite (no "please" or "thanks for reading")
- [ ] Demonstrate, don't speculate (show examples)
- [ ] Zero fluff (no unnecessary intros)
- [ ] Call-to-Build (end with action)

---

## Course-Specific Guidelines

### Advanced AI Video Creation
- Focus on advanced techniques (not beginner tutorials)
- Include tool version numbers
- Provide optimization tips
- Scripts must handle errors gracefully

### Digital Twin Foundations
- **ETHICS FIRST:** All examples must have documented consent
- Include consent templates with all digital twin content
- Disclose AI-generated content clearly
- No celebrity/public figure examples without permission

### AI Video Mastery (Shorts + Reels)
- Keep tutorials under 10 minutes
- Export settings must match platform requirements
- Stock footage must be royalty-free
- Include posting strategy notes

### Image Factory
- Prompt libraries must include tool version
- Show before/after examples
- Note copyright considerations
- Include parameter explanations

---

## Submission Process

### 1. Fork and Clone
```bash
git clone https://github.com/[your-username]/AI-Video-Factory-Resources.git
cd AI-Video-Factory-Resources
```

### 2. Create a Branch
```bash
git checkout -b add-[asset-name]
```

### 3. Add Your Asset
```bash
# Add file to appropriate folder
cp your-file.mp4 advanced-ai-video-creation/videos/01-your-lesson.mp4
```

### 4. Update Course README
Edit the course's `README.md`:
- Add file to asset table
- Update asset status counts
- Link from lesson structure

### 5. Update Main README
Edit the root `README.md`:
- Update asset status table
- Increment file counts

### 6. Commit Changes
```bash
git add .
git commit -m "Add [asset type]: [brief description]

- Added [file name] to [course name]
- Updated README with asset details
- [Any other relevant notes]"
```

### 7. Push and Create PR
```bash
git push origin add-[asset-name]
```
Then create a pull request on GitHub.

---

## Pull Request Checklist

Before submitting, verify:

- [ ] File follows naming convention
- [ ] File is in correct directory
- [ ] Course README updated
- [ ] Main README updated (if needed)
- [ ] Asset meets technical requirements
- [ ] Content follows brand voice
- [ ] (Scripts only) Tested and includes usage docs
- [ ] (Digital twins only) Consent documented
- [ ] PR description explains what and why

---

## Asset Status Indicators

Use these in README files:

- ✅ **Complete** - File exists and tested
- 📦 **Awaiting upload** - Planned but not yet added
- 🚧 **In progress** - Currently being created
- ⚠️ **Needs review** - Uploaded but requires quality check
- ❌ **Deprecated** - No longer recommended

---

## Common Mistakes to Avoid

❌ **Don't:**
- Upload files without updating READMEs
- Use generic names (template.md, script.py)
- Skip documentation headers in scripts
- Add large files without Git LFS
- Include personal credentials or API keys
- Use copyrighted content without permission

✅ **Do:**
- Follow naming conventions exactly
- Test scripts before committing
- Document everything
- Use royalty-free assets
- Get consent for digital twin content
- Keep file sizes reasonable

---

## Getting Help

- **Questions:** Open a GitHub issue
- **Bug reports:** Open a GitHub issue with "Bug:" prefix
- **Feature requests:** Open a GitHub issue with "Enhancement:" prefix
- **Community:** Join the AI Video Factory Skool group

---

## Brand Voice Reminder

**Promise:** From blank to posted in one sitting
**Enemy:** Overwhelm
**Voice Rules:**
- Direct over polite
- Demonstrate, don't speculate
- Zero fluff; receipts win
- Respect consent + credit

Every asset should help users ship faster and avoid overwhelm.

---

## License

By contributing, you agree that your contributions will be licensed under the same license as this repository.

See [LICENSE](LICENSE) for details.

---

**Last Updated:** November 4, 2025
**Maintained by:** AI Video Factory Team
**Repository:** [AI-Video-Factory-Resources](https://github.com/jmanhype/AI-Video-Factory-Resources)
