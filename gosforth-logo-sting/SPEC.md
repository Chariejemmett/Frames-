# Gosforth Roofing logo sting

GOAL:    the viewer meets the mark as a character and remembers the lockup it builds: "// GOSFORTH ROOFING".
REFERENCE: a LinkedIn logo reel (screen recording). Its grammar, not its content: a whip in with a heavy
         horizontal smear, the mark acting like a character, a loose dot knocked out of it, the wordmark
         popping out letter by letter beside the mark, the dot falling home last, a hold. Extended: a pattern built from the mark, ending on the icon alone.
OUTPUT:  HyperFrames, 1920 x 1080, 60 fps, 11 s (660 frames). Starts on the empty ground, ends on the icon alone.
LOOK:    ground #FFFFFF, ink #0E0E0E (wordmark), accent #F03535 (mark: two slashes and the dot).
         The logo is the brand's own artwork, traced from the supplied PNG to vectors (mean alpha error 0.4/255),
         one path per piece: 2 slashes, 1 dot, 15 letters. No added type, no effects, no grain.
         Final lockup 1307 px wide (68% of the width), centred; cap height 83 px (7.7% of the height).
OBJECTS: the "//" mark is one body (two slashes squash and rock together); the dot is a separate small body
         with its own weight; the letters are pieces that grow up from the baseline.
MOTION:  whip: expo.out arrival, power3/4.in exit, render-time motion blur (shutter 480).
         gravity: power2.out going up, power2.in coming down. Impacts: 3-frame squash, springback
         elastic.out(1, 0.45) (damping ~0.5, playful). Letters: scaleY 0 -> 1 from the baseline, back.out(2.4),
         0.34 s each, staggered unevenly 30-70 ms. Camera: one pull-back, power3.inOut.
SHOTS (one continuous shot, camera at 2.4x then pulling back to 1x):
  0.00-0.62  "//" whips in from the left, smeared; brakes, tips forward on its front corner, drops back. tap on landing.
  0.62-0.86  small rock back onto its rear corner; settles at frame centre.
  0.84-1.02  the dot pops into being at its home corner; the mark crouches.               pop
  1.02-1.56  the mark jumps and flips a half turn (lands looking identical); the dot is
             launched straight up out of frame.                                         whoosh, tap on landing
  1.70-2.30  the mark leans back, looking up after the dot.
  2.20-3.60  camera pulls back from 2.4x to 1x while the lockup slides left to centre; the 15
             letters grow up out of the baseline beside the mark, left to right.      soft ticks per letter
  3.55-3.85  the dot falls back in from the top and hits the right slash; the mark dips, a ripple runs
             through the letters.                                                      click
  3.85-4.38  the dot bounces once and lands on its home corner, squashes, settles.       pop (the payoff)
  4.40-5.60  hold, dead still.
  5.60-6.45  the letters sink back into the baseline, right to left; the mark slides back to centre.  woosh (supplied)
  6.35-7.00  copies of the "//" ripple out from the mark into a full-frame brick pattern: rows alternate
             red and ink like courses of roof tiles (190 x 150 px grid, 104 tiles).               cinematic whoosh
  7.05-7.65  every row but the mark's slides one tile, alternate rows in opposite directions.         whoosh
  7.70-8.50  a flip wave runs along the slant: each pair turns a half turn and lands identical.         woosh (supplied)
  8.55-9.60  the pattern collapses inward, farthest tiles first, while the camera pushes in 3x.
  9.60-11.0  the icon lands alone, settles, and holds to the end (1.4 s).                             bass hit
BANNED:  glow, particles (the pattern is the mark itself, never decoration), gradients, a dark void; fading anything in; the logo redrawn or re-typed;
         titles drifting after they land; a docked corner logo; bounce on the lockup during the hold.
QA:      frames at 0.30, 0.62, 1.30, 1.56, 2.00, 2.70, 3.20, 3.86, 4.40, 5.00, 6.00; the final lockup at 5.0 s
         must match the supplied PNG; every piece in frame after 3.6 s.
