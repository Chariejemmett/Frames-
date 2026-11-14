# Charlie G Studio logo animation

GOAL:    the dot is the character: it bounces the wordmark into being, lands in the G, then returns as a
         big disc that swallows the wordmark and becomes the icon. The viewer remembers the icon.
REFERENCE: a Fiverr logo animation (screen recording, clean half from 4.20 s). Its grammar and timing, not its
         content: first mark drawn, a dot bouncing along the baseline with a thin trail raising each letter, the dot
         landing as the full stop, a hold, the dot hopping off right, returning as a big circle that sweeps left over
         the wordmark and becomes the icon, which slides to centre and holds.
OUTPUT:  HyperFrames, 1920 x 1080, 60 fps, 9.7 s (582 frames).
TIME:    the soundtrack is the reference's whole audio (0-9.70 s of the recording). Its first 4 s are a quiet build-up
         (act 1); the beat drops at ~4.1 s and hits land every ~0.27 s. Act 2 starts at 4.20 s, exactly where the
         reference's clean pass starts, so its beats keep the reference's timing.
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
  3.98-4.20  the snap flings the dot off the top left; the G shrinks (0.366x) into its place in the wordmark.
  ACT 2, from the drop: the previous film, every time + 4.20 s
  4.80-5.70  the dot falls back in from the upper left and bounces CHARLIE up; drops into the G.
  5.72-5.92  the landing cascades STUDIO in.        hold to 6.40.
  6.40-6.75  the dot hops off the right edge.
  6.80-7.15  it returns as a 340 px disc and sweeps the wordmark away.
  7.15-7.53  the disc becomes the icon's dot as the blocks grow round it; the icon slides to centre.
  ENDING
  8.40, 8.92 the icon punches (1.05x, 1.03x) on the last two hits, rhyming with act 1.
  8.92-9.70  hold; the music fades out over the last 0.45 s.
BANNED:  glow, particles, gradients, any colour not in the logo, fades standing in for motion, drifting after landing.
QA:      0.62, 0.85, 1.9, 2.2, 3.85, 4.05, 4.3, 5.1, 6.2, 7.0, 7.3, 8.43, 9.6 s; the lockup at 6.2 s against the logo PNG and the
         icon at 9.0 s against the icon PNG.
