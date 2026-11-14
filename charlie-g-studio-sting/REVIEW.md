# Review: Charlie G Studio logo animation

**Output:** `renders/charlie-g-studio-logo.mp4`, 1920 x 1080, 60 fps, 4.7 s (282 frames), H.264 + AAC.

## Creative calls
- Modelled on the Fiverr logo animation in the supplied screen recording (its clean half, from 4.20 s), beat for beat:
  the mark builds, a dot bounces along the baseline with a thin trail raising the letters, the dot lands, a hold,
  the dot hops off right and returns as a big circle that sweeps the wordmark away and becomes the icon.
- The G's own dot plays Fiverr's green dot. It bounces CHARLIE into being, drops into its slot in the G, and the
  landing cascades STUDIO in. At the end the returning disc shrinks into the dot of the big icon.
- Colours are exactly the supplied PNGs (#1C1C1C ground, white logo), set as variables (Background, Logo).
- Logo pieces are traced from the two PNGs: wordmark 17 pieces (mean error 0.23/255), icon 4 pieces (0.08/255).

## Sound
- The soundtrack is the reference's own audio, 4.20-8.90 s of the screen recording, in
  `assets/audio/reference-soundtrack.wav`, with a 0.5 s fade-out. Its effects are mixed into the music, so they
  could not be separated; instead every beat of this animation sits at the reference's time minus 4.20 s, so its
  hits land on the matching moments.
- Rights: the track comes from someone else's TikTok post and is likely a licensed or commercial song. Fine for a
  private draft; replace it before publishing or client use.

## Measured
- `hyperframes check`: ok, 0 errors. Lockup at 2.0 s vs the logo PNG: mean difference 0.41/255; icon at 4.0 s vs
  the icon PNG: 0.24/255 (remaining differences are edge pixels from the half-pixel placement and PNG softness).
- Render audio: -12.9 LUFS integrated, -1.2 dBTP, no clipping. Measured, not heard.

## Kept on purpose
- `first_frame_empty`: the film opens on the empty ground; the G starts building on the third frame.

## Weakest moment
- 2.88-2.95 s: the disc's sweep is so fast that motion blur turns it into a soft smear for about four frames, as in the
  reference. Slowing the sweep from 0.15 s to 0.25 s would show the disc more clearly at the cost of the snap.
