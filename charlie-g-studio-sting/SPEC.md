# Charlie G Studio logo animation

GOAL:    the dot is the character: it bounces the wordmark into being, lands in the G, then returns as a
         big disc that swallows the wordmark and becomes the icon. The viewer remembers the icon.
REFERENCE: a Fiverr logo animation (screen recording, clean half from 4.20 s); its music is no longer used. Its grammar and timing, not its
         content: first mark drawn, a dot bouncing along the baseline with a thin trail raising each letter, the dot
         landing as the full stop, a hold, the dot hopping off right, returning as a big circle that sweeps left over
         the wordmark and becomes the icon, which slides to centre and holds.
OUTPUT:  HyperFrames, 1920 x 1080, 60 fps, 11.81 s (709 frames).
TIME:    no music. The timing grid is kept from the reference soundtrack it was first cut to: beats every 0.26483 s
         from 5.199 s, the text loading one letter per beat. Every visible action has its own sound effect.
SOUND:   act 1: a whoosh as the dot drops in and as each block flies in, a low thump as each block locks, a full
         sub-bass hit when the G completes, thumps under the two punches, a riser through the pull-apart cut off by a
         bass hit on the snap. Keyboard clacks for every dot landing and every letter; a Star Trek hail as the dot lands
         in the G, a chirp as it flies off; a whoosh for the disc sweep and a bass hit as the disc becomes the icon.
         Each placed so its hit lands one frame after its picture.
LOOK:    ground #1C1C1C, ink #FFFFFF, exactly the supplied PNGs. Monochrome: no accent added.
         Logo pieces traced from the PNGs (wordmark: 17 pieces, mean error 0.23/255; icon: 4 pieces, 0.08/255).
         Lockup at 1:1 of the PNG: 1347 px wide (70% of the frame), cap height 92 px, centred.
         Final icon from the icon PNG at 2x: 344 x 330 px, centred.
OBJECTS: the G is three blocks and a dot; the dot is a white ball with weight (squash on every touchdown);
         the disc is the same dot grown to 340 px.
MOTION:  letters grow up from the baseline, back.out(2.2), 0.3 s. Dot: parabolic hops, linear in x, squash
         1.3 x 0.7 over +-0.04 s at each touchdown, a thin 3 px trail along its own path.
         Disc sweep: power2.in, 0.15 s. Icon slide: power3.out, 0.33 s.
SHOTS:
  ACT 1, over the build-up (big icon at frame centre, 344 x 330 px)
  0.30-0.95  the dot drops in alone and bounces.
  0.72-1.00  the left block slides in from the left; the dot hops.
  1.54-1.80  the top-right block drops in from the top; the dot hops.
  1.92-2.12  the lower-right block slides in from the right and closes the G.
  2.30, 2.60 the G punches (1.05x) on two hits.
  2.75-3.98  the four pieces pull apart as the music builds, then snap back together on the drop (power4.in).
  3.98-4.20  the G, dot included, shrinks (0.366x) into its place in the wordmark.
  ACT 2, from the drop (beats b0 = 5.199 s, then every 0.265 s)
  4.28-5.20  the dot pushes off from its slot and arcs high to the left, never leaving the frame.
  5.20-6.79  one hop per beat along the baseline; each letter of CHARLIE grows up as the dot lands beside it.
  6.79-7.32  a two-beat hop back into the G; STUDIO cascades in at half-beat steps (7.34-7.98).  hold to 8.52.
  8.52-8.87  the dot hops off the right edge.
  8.92-9.27  it returns as a 340 px disc and sweeps the wordmark away.
  9.27-9.65  the disc becomes the icon's dot as the blocks grow round it; the icon slides to centre.
  ENDING
  10.52, 11.04 the icon punches (1.05x, 1.03x) on the last two hits, rhyming with act 1.
  11.04-11.81 hold to the end.
BANNED:  glow, particles, gradients, any colour not in the logo, fades standing in for motion, drifting after landing.
QA:      4.6, 5.2, 6.1, 7.0, 7.6, 8.0, 8.6, 9.2, 9.5, 10.55, 11.5 s; the lockup at 8.3 s against the logo PNG and the
         icon at 11.2 s against the icon PNG.
