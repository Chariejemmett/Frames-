# Review: Gosforth Roofing logo sting

**Output:** `renders/gosforth-logo-sting.mp4`, 1920 x 1080, 60 fps, 11 s (660 frames), H.264 + AAC, 4.4 MB.

## Creative calls
- Modelled on the LinkedIn logo reel the person sent: whip in, the mark acts like a character, a loose dot,
  the wordmark grows out beside the mark, the dot drops home last, hold, whip out.
- The red dot in the Gosforth mark plays the LinkedIn i-dot. It is launched out of frame early and falls back
  at the end; it ricochets off the right slash and drops down that slash's slope into place, like water off a roof pitch.
- Extended ending: after the lockup, the letters sink back, and copies of the mark ripple out into a full-frame
  pattern of red and black rows, like courses of roof tiles. Rows slide, a flip wave runs across them, then the
  pattern collapses inward as the camera pushes in, and the film ends on the icon alone, held 1.4 s.
- The mark's jump is a half-turn flip: the two slashes swap places and land looking identical.
- A camera starts at 2.4x so the small mark reads as the hero, then pulls back to 1x as the wordmark builds.
- White ground and the logo's own colours, matching the supplied PNG. Colours are variables
  (Background, Wordmark, Mark red), so a dark version like the existing black logomark clip is a variable change.
- Sound: Pixabay-licensed effects bundled with HyperFrames on each visible action (whoosh in, taps on landings,
  a pop when the dot appears and when it lands home, a cinematic whoosh as the pattern spreads, a whoosh on the
  row slide, a sub-bass hit when the icon lands). The supplied woosh also plays as the letters sink back and on
  the flip wave. No music.
- The wordmark's sound is the "Woosh" the person supplied, cut from their sound-effects reel (4.195-4.525 s of
  the source) into `assets/sfx/woosh-reference.wav`. It plays once for the whole text build, at 0.8x speed so it
  sweeps a little longer (0.41 s), peaking at 2.6 s as the first letters grow in.

## Measured
- The logo is the supplied PNG traced to vectors, one path per piece. The final lockup at 5.0 s against the PNG:
  mean difference 0.30/255; remaining differences are anti-aliased edges.
- `hyperframes check`: ok, 0 errors. Every sound sits one frame after its picture (peaks measured per file).
- Render audio: -18.9 LUFS integrated, -1.6 dBTP, no clipping. Measured, not heard.

## Kept on purpose
- `first_frame_empty`: the film starts on the empty ground, like the reference. It now ends on the icon, so it no longer loops.

## Weakest moment, and what I would change with more time
- 2.6-3.0 s: the letters grow while the camera is still pulling back, so the motion blur smears them; they
  read cleanly from 3.2 s. Starting the letters ~0.2 s later would make them crisper at the cost of length.
