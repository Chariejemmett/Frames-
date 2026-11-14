# Review: KSL Commercial Cleaning logo animation

**Output:** `renders/ksl-logo.mp4`, 1920 x 1080, 60 fps, 7.5 s (450 frames), H.264 + AAC.

## Creative calls
- No reference video was given, so this follows the build the person liked in their Charlie G Studio animation:
  pieces arrive one by one on whooshes and thumps, the logo punches, pulls apart over a riser and snaps back on a
  bass hit, then the tagline types in.
- Each letter enters its own way: the K's stem drops from the top, its navy leg kicks in along its own diagonal,
  the S rolls in with a full turn, the L slides in and completes KSL.
- For a cleaning company, one white shine sweeps across the letters after the snap, clipped to the letter shapes.
- Colours and shapes are the supplied SVG's own (no tracing). Ground, light blue and navy are variables.

## Sound
- No music. 36 effects, all from the HyperFrames bundle (Pixabay licence, free for commercial use): a whoosh as
  each piece flies in, a click and a low thump as each lands, a bass hit when the L completes KSL, a thump under the
  punch, a riser through the pull-apart cut off by a bass hit on the snap, a sparkle with the shine, and a key
  press per tagline letter (three playback rates rotated).

## Measured
- `hyperframes check`: ok, 0 errors. Final frame vs the supplied SVG at the same scale: mean difference 0.29/255
  (anti-aliased edges).
- Render audio: -17.2 LUFS integrated, -4.1 dBTP, no clipping; onsets in the render match the picture times.
  Measured, not heard.

## Kept on purpose
- `rotation_pivot_drift` (check warning): the S spins about its own centre while it slides in 1300 px; the check
  reads the slide as drift.
- The first frame is the empty ground; the K drops in at 0.2 s.

## Weakest moment
- 1.3 s: the S's roll is fast enough that motion blur softens it to a smear for a few frames. A slower roll
  (0.55 s) would show the letter turning.
