# Frames

Claude Code skills for making motion videos with [HyperFrames](https://github.com/heygen-com/hyperframes),
HeyGen's open-source "write HTML, render video" framework (Apache-2.0). A video is an `index.html` that mounts
one scene per file, animated with GSAP (or CSS, Lottie, Three.js) on a paused timeline; the CLI seeks that
timeline frame by frame in headless Chrome and encodes an MP4 with FFmpeg, so every render is identical and
every layer, scene and keyframe stays editable as source.

## What is here

`.claude/skills/` holds the HyperFrames **core skill set**, copied from `heygen-com/hyperframes` at release
v0.9.45 (commit `b5e9bc6`, 2026-11-14). Claude Code loads project skills from `.claude/skills/<name>/SKILL.md`,
so any session opened on this repository has them.

| Skill | Use it for |
| --- | --- |
| `hyperframes` | Read first for any request to make, edit, animate or render a video. The render contract, the work loop, and references for format, motion, story, spec, storyboard, review, sound, captions and film types. |
| `hyperframes-cli` | The CLI by job: `init`, `lint`, `check`, `snapshot`, `timeline`, `preview`, `render`, `doctor`. |
| `hyperframes-registry` | About 450 ready-made blocks and components (transitions, titles, kinetic type, captions, charts, camera moves, 3D) installed as editable source with `npx hyperframes add`. |
| `media-use` | Music, sound effects, images, logos, voiceover, cutouts and colour grades through HeyGen or free local tools. |
| `reverse-any-video` | Rebuild an existing video as an editable HyperFrames project (HyperFrames Pro). |
| `style-sampling` | A new episode in one of five proven styles, including Collage Explainer (HyperFrames Pro). |

## Requirements

- Node.js 22+ and FFmpeg on the machine that renders.
- HyperFrames downloads its pinned Chrome on first use (`npx hyperframes browser ensure`).
- Check a new machine once with `npx hyperframes doctor`.

## Making a video

```bash
npx hyperframes init my-video --skip-skills   # scaffold a project folder
cd my-video
npx hyperframes check --json                   # lint, runtime, layout and contrast checks
npx hyperframes snapshot                       # PNG frames to look at
npx hyperframes preview --background           # Studio preview with live reload
npx hyperframes render --quality looks -o out.mp4
```

Or ask Claude in this repository: "Using /hyperframes, make a 10-second …". The skill plans the film
(three storylines, then a numeric `SPEC.md`), builds the scenes, checks and reviews them, and renders when
you approve the preview.

## Keeping the skills current

Skills are versioned with the CLI. From this directory, `npx hyperframes skills update` refreshes the core
set to match the installed CLI; `npx hyperframes skills update <name>` adds an on-demand skill
(`figma`, `slideshow`, `remotion-to-hyperframes`).
