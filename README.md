# Nikki Prompt Lab

A Claude Code skill by Nicola Harvey for writing generation-ready prompts for AI image and video tools. It covers three modes: image prompts, single-shot video prompts, and multi-shot video sequences.

## What it does

**Mode 1: Image prompts**
Builds structured prompts for Midjourney, Flux, Stable Diffusion, Firefly, DALL-E, and similar tools. Covers subject, composition, lighting, lens, color grading, and style signature. Outputs a clean prompt block ready to paste, with optional iteration notes.

**Mode 2: Single-shot video prompts**
Builds one-clip prompts for Veo, Kling, Runway, Seedance, Hailuo, Sora, and similar tools. Covers shot type, camera movement, subject action, lighting, color grade, and audio direction (for platforms that support it). Outputs a prompt block with suggested clip duration and platform notes.

**Mode 3: Multi-shot video sequences**
Builds a complete timestamped shot sequence for multi-shot video work. Used for Veo 3.1 timestamp prompting, Kling scene planning, Runway multi-shot, or as a director's shot list for any AI video tool. Output has four sections: scene header, timestamped shot sequence, audio map, and director's notes.

## Platform support

| Platform | Shot duration | Audio support | Multi-shot |
|----------|--------------|---------------|------------|
| Veo 3.1 | 4-8s | Full | Timestamp format |
| Kling 2.1 | 5-10s | Partial | Scene planning |
| Runway Gen-4 | 5-10s | No | Manual |
| Seedance 2.0 | 4-8s | No | Manual |
| Hailuo | 6s | No | Manual |
| Sora | Up to 20s | No | Storyboard mode |
| Midjourney | Still | No | No |
| Flux | Still | No | No |
| Firefly | Still | No | No |

## Honest limits

- The skill writes prompts. It does not run them. You still need access to the tool you are generating for.
- Platform capabilities change frequently. Model versions, parameter names, and supported features in the table above may have changed since the skill was written. Check the platform's own docs for current specs.
- Multi-shot character consistency across clips is still a genuine challenge in AI video. Good prompts improve the odds but do not guarantee it.
- Audio direction is only useful on platforms that support audio generation (currently Veo 3.1 and Kling 2.1). Including it in prompts for other platforms has no effect.

## Installing for Claude Code

Clone the repo directly into your skills directory:

```bash
git clone https://github.com/nicolakharvey/nikki-prompt-lab.git ~/.claude/skills/nikki-prompt-lab
```

Claude Code picks up skills from `~/.claude/skills/` automatically. No restart needed.

## Installing for Claude desktop

1. Download or clone this repo.
2. Zip the `nikki-prompt-lab` folder.
3. In Claude desktop, go to Settings > Capabilities > Skills.
4. Upload the zip file.

## Using the skill

Once installed, describe what you want to generate and Claude will use this skill automatically. You can also ask directly:

> "Write me a Midjourney prompt for..."
> "Write a video prompt for Kling for..."
> "Build me a multi-shot sequence for a 30-second video about..."

If your request is ambiguous between image and video, Claude will ask one clarifying question before building the prompt.

---

Part of the **Nikki** suite of AI tools by [Nicola Harvey](https://linkedin.com/in/nicolakharvey).
