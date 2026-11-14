# Review: Charlie G Studio logo animation

**Output:** `renders/charlie-g-studio-logo.mp4`, 1920 x 1080, 60 fps, 11.81 s (709 frames), H.264 + AAC.

## Creative calls
- Modelled on the Fiverr logo animation in the supplied screen recording (its clean half, from 4.20 s), beat for beat:
  the mark builds, a dot bounces along the baseline with a thin trail raising the letters, the dot lands, a hold,
  the dot hops off right and returns as a big circle that sweeps the wordmark away and becomes the icon.
- The G's own dot plays Fiverr's green dot. It bounces CHARLIE into being, drops into its slot in the G, and the
  landing cascades STUDIO in. At the end the returning disc shrinks into the dot of the big icon.
- Colours are exactly the supplied PNGs (#1C1C1C ground, white logo), set as variables (Background, Logo).
- Logo pieces are traced from the two PNGs: wordmark 17 pieces (mean error 0.23/255), icon 4 pieces (0.08/255).

- Extended to the length of the supplied video. A new first act plays over the soundtrack's quiet build-up: the dot
  drops in alone, the G's three blocks arrive one by one, the big G punches on two hits, its pieces pull apart as the
  music builds and snap together on the drop, and the G shrinks into its place in the wordmark. The dot
  then hops out of the G in one long arc to where it starts bouncing the letters in; it never leaves the frame. The text then loads one letter per beat: CHARLIE one hop per beat (5.2-6.8 s), STUDIO at half-beat
  steps once the dot is back in the G. Everything after that plays as before, on the same hits. On the last two hits the icon punches again.

## Sound
- No music. 33 sound effects, one per visible action, each placed so its hit lands one frame after its picture
  (credits in `assets/sfx/CREDITS.md`):
  - keyboard clacks (five single keystrokes cut from github.com/6m1w/claude-sound-fx): the dot's landings in act 1,
    one clack per letter as CHARLIE and STUDIO load in, the punches and the snap;
  - Star Trek interface sounds from the same repository: a hail when the dot lands in the G, a chirp as it flies off;
  - from the HyperFrames bundle (Pixabay licence): in act 1, a whoosh as the dot drops in and as each block flies in,
    a low thump as each block locks, a full bass hit when the G completes and thumps under the two punches; a whoosh
    for the disc sweep, and a riser that climbs through the
    pull-apart (2.73-3.98 s, its steepest 1.25 s) and is cut off by a sub-bass hit as the pieces snap together; the same hit, quieter, as the disc turns into the icon.
- Rights: the repository is MIT for its code, but its audio has no stated source; the Trek sounds come from the Star
  Trek franchise. Replace them with cleared effects before publishing or client use.
- The rest of the repository is voice clips of film, game and anime characters (JARVIS, GLaDOS, Pikachu and others)
  and was not used.

## Measured
- `hyperframes check`: ok, 0 errors. Lockup at 2.0 s vs the logo PNG: mean difference 0.41/255; icon at 4.0 s vs
  the icon PNG: 0.24/255 (remaining differences are edge pixels from the half-pixel placement and PNG softness).
- Render audio: -19.1 LUFS integrated (sparse effects with silence between them), -1.0 dBTP, no clipping;
  onsets measured in the render match the picture times. Measured, not heard.

## Kept on purpose
- `first_frame_empty`: the film opens on the empty ground; the dot drops in at 0.3 s.

## Weakest moment
- 7.08-7.15 s: the disc's sweep is so fast that motion blur turns it into a soft smear for about four frames, as in the
  reference. Slowing the sweep from 0.15 s to 0.25 s would show the disc more clearly at the cost of the snap.
