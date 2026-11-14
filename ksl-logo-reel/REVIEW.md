# Review: KSL logo, LinkedIn-reel style

**Output:** `renders/ksl-logo-reel.mp4`, 1920 x 1080, 60 fps, 6.3 s (378 frames), H.264 + AAC.

- `hyperframes check`: ok, 0 errors. Kept warnings: `rotation_pivot_drift` twice (the K's flip while it jumps and the
  leg's spin while it flies are meant to travel), `first_frame_empty` (the K whips in from off screen, as in the reel).
- Render audio: -21 LUFS integrated (sparse effects), -3.0 dBTP, no clipping; onsets match the picture. Measured,
  not heard. The reel's own soundtrack was not used; all effects are Pixabay-licensed.
- Left out on purpose: the reel's whip-out at the end. Adding it is a 0.4 s tween on the lockup and one whoosh.
