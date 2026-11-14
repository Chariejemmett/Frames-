# Review: Gosforth Roofing logo sting

**Output:** `renders/gosforth-logo-sting.mp4`, 1920 x 1080, 60 fps, 6.4 s (384 frames), H.264 + AAC, 1.0 MB.

## Creative calls
- Modelled on the LinkedIn logo reel the person sent: whip in, the mark acts like a character, a loose dot,
  the wordmark grows out beside the mark, the dot drops home last, hold, whip out.
- The red dot in the Gosforth mark plays the LinkedIn i-dot. It is launched out of frame early and falls back
  at the end; it ricochets off the right slash and drops down that slash's slope into place, like water off a roof pitch.
- The mark's jump is a half-turn flip: the two slashes swap places and land looking identical.
- A camera starts at 2.4x so the small mark reads as the hero, then pulls back to 1x as the wordmark builds.
- White ground and the logo's own colours, matching the supplied PNG. Colours are variables
  (Background, Wordmark, Mark red), so a dark version like the existing black logomark clip is a variable change.
- Sound: Pixabay-licensed effects bundled with HyperFrames on each visible action (whoosh in and out, taps on
  landings, a pop when the dot appears and when it lands home). No music.
- The wordmark's sound is the "Woosh" the person supplied, cut from their sound-effects reel (4.195-4.525 s of
  the source) into `assets/sfx/woosh-reference.wav`. It plays once per word: as GOSFORTH grows in (2.48 s) and as
  ROOFING follows (2.91 s, 6% faster for variation). It replaced 15 per-letter key ticks.

## Measured
- The logo is the supplied PNG traced to vectors, one path per piece. The final lockup at 5.0 s against the PNG:
  mean difference 0.30/255; remaining differences are anti-aliased edges.
- `hyperframes check`: ok, 0 errors. Every sound sits one frame after its picture (peaks measured per file).
- Render audio: -19.1 LUFS integrated, -1.1 dBTP, no clipping. Measured, not heard.

## Kept on purpose
- `first_frame_empty`: the sting starts and ends on the empty ground, like the reference, so it loops.

## Weakest moment, and what I would change with more time
- 2.6-3.0 s: the letters grow while the camera is still pulling back, so the motion blur smears them; they
  read cleanly from 3.2 s. Starting the letters ~0.2 s later would make them crisper at the cost of length.
