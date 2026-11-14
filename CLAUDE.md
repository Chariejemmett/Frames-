# Frames

This repository holds the HyperFrames skill set for making motion videos as HTML rendered to MP4.

- For any request to make, edit, animate or render a video, read `.claude/skills/hyperframes/SKILL.md` first
  and follow its contract and work loop. It routes to `hyperframes-cli`, `hyperframes-registry` and `media-use`.
- Run the CLI as `npx hyperframes <command>` from the video project's own directory (Node.js 22+, FFmpeg).
- Each video project lives in its own folder at the repository root, scaffolded with
  `npx hyperframes init <name> --skip-skills`. Never hand-build the project layout.
