# Charlie G Studio logo animation

GOAL:    the dot is the character: it bounces the wordmark into being, lands in the G, then returns as a
         big disc that swallows the wordmark and becomes the icon. The viewer remembers the icon.
REFERENCE: a Fiverr logo animation (screen recording, clean half from 4.20 s). Its grammar and timing, not its
         content: first mark drawn, a dot bouncing along the baseline with a thin trail raising each letter, the dot
         landing as the full stop, a hold, the dot hopping off right, returning as a big circle that sweeps left over
         the wordmark and becomes the icon, which slides to centre and holds.
OUTPUT:  HyperFrames, 1920 x 1080, 60 fps, 4.7 s (282 frames).
TIME:    the soundtrack is the reference's own audio (4.20-8.90 s of the recording), so every beat below sits at
         the reference's time minus 4.20 s and its hits land where the reference's did.
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
  0.05-0.55  the G's three blocks grow out of their outer corners at centre of the lockup.
  0.60-1.50  the dot falls in from the upper left and bounces along the baseline: C H, A R, L I E grow up as it
             lands beside them; a last high hop drops it into its slot in the G (1.50).
  1.52-1.75  the landing sends a cascade through S T U D I O, left to right.
  1.75-2.20  hold.
  2.20-2.55  the dot hops out of the G and off the right edge.
  2.60-2.80  it re-enters from the right, grown to a 340 px disc.
  2.80-2.95  the disc sweeps left across the wordmark; every letter is gone once the disc has passed it.
  2.95-3.10  the disc becomes the icon: the three blocks grow around it as it shrinks into the icon's dot.
  3.00-3.33  the icon slides to the centre.
  3.33-4.70  hold on the icon.
BANNED:  glow, particles, gradients, any colour not in the logo, fades standing in for motion, drifting after landing.
QA:      0.3, 0.9, 1.25, 1.5, 1.7, 2.0, 2.4, 2.7, 2.88, 3.0, 3.2, 4.0 s; the lockup at 2.0 s against the logo PNG and the
         icon at 4.0 s against the icon PNG.
