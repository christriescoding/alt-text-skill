# Alt-Text Generator — Claude Code Skill

A proof of concept for AI-assisted alt-text generation, built as a Claude Code Skill. This tool is designed to help Editorial teams generate accurate, accessibility-compliant alt-text for images used on news editorial websites.

---

## What This Does

When given an image, this Skill uses Claude to analyse the visual content and return a concise, accurate alt-text string that follows accessibility best practices. The output is ready to review and use directly in a CMS.

---

## Who This Is For

This prototype is intended for review by Editorial and Product stakeholders to assess whether AI-generated alt-text is sufficiently accurate for use in a production content workflow.

---

## How to Use It

### Prerequisites
- [Claude Code](https://claude.ai/code) installed on your machine
- A folder of images you want to test

### Steps

1. **Clone or download this repository**
   ```bash
   git clone https://github.com/christriescoding/alt-text-skill.git
   ```

2. **Open the project folder in Claude Code**
   ```bash
   cd alt-text-skill
   ```

3. **Run the Skill**
   - In Claude Code, type `/generate-alt-text` in the command bar
   - When prompted, attach or reference the image you want to generate alt-text for
   - Claude will return a single alt-text string ready to copy and use

---

## Example

**Input:** A photo of a politician speaking at a podium with a flag in the background

**Output:**
```
A politician stands at a podium with arms outstretched in front of a large national flag.
```

---

## Folder Structure

```
alt-text-skill/
├── .claude/
│   └── commands/
│       └── generate-alt-text.md   ← The Skill instructions
├── example-images/                ← Sample images for testing
│   └── (add your test images here)
└── README.md                      ← This file
```

---

## Limitations of This Prototype

- This is a proof of concept only and has not been tested at production scale
- Accuracy may vary for complex or abstract images — human review is always recommended
- The Skill does not currently integrate directly with Statamic or any CMS; that would be the next phase of development

---

## Testing Guide

When testing, ask yourself:

- Is the description factually accurate?
- Is it the right level of detail — not too vague, not too verbose?
- Does it read naturally for a screen reader user?
- Are there any images where it struggles or gets things wrong?

Run it against as many different image types as you can — portraits, crowds, landscapes, graphics, screenshots — to build a picture of where it excels and where it might need the prompt refining. Note down any examples where the output is inaccurate or too vague, as well as any patterns in where it struggles — that feedback is really valuable for refining the Skill instructions.

---

## Next Steps

If this prototype demonstrates sufficient accuracy, the recommended next step is to integrate this capability directly into Statamic as a custom addon, allowing Editorial to generate and review alt-text without leaving the CMS.

---

## Questions or Feedback

Please raise any issues or suggestions via the GitHub Issues tab on this repository.
