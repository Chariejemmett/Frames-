# KSL Commercial Cleaning logo animation

GOAL:    the letters K, S and L arrive one by one like parts clicking together, the logo gets wiped clean with a
         shine, and "COMMERCIAL CLEANING" types itself in. The viewer remembers a crisp, clean lockup.
REFERENCE: the person's earlier logo animations in this repository (the Charlie G Studio build in particular):
         pieces flying in on whooshes and thumps, a punch, a pull-apart over a riser that snaps back on a bass hit,
         text typed in letter by letter, then a hold.
OUTPUT:  HyperFrames, 1920 x 1080, 60 fps, 7.5 s (450 frames).
LOOK:    ground #FFFFFF, light blue #6FBFE5 (K, S, L), navy #0D1D27 (the K's leg and the tagline): the supplied SVG's
         own colours, set as variables. The SVG's own vector paths, one element per piece (S, K stem and arm, K leg,
         L, 18 tagline letters). Scale 8x: logo 1100 px wide, KSL 388 px tall, tagline cap height 65 px, centred.
         The one effect is a white shine band (0 -> 90% -> 0 white, 128 px wide, slanted) that sweeps across the
         blue and navy letters once: the cleaning medium, clipped to the letter shapes.
MOTION:  arrivals: power2.in for falls, power3.out for slides, back.out(1.3) for the L; impacts squash on the base,
         springback elastic.out(1, 0.45). Pull-apart power2.inOut over 1.05 s, snap power4.in 0.12 s.
         Tagline letters grow up from the baseline, back.out(2.2), 0.28 s, 50 ms apart, 130 ms between the words.
SOUND:   all from the HyperFrames bundle (Pixabay licence): a whoosh as each piece flies in, a click and a low thump
         as each lands, a full bass hit when the L completes the logo, a thump under the punch, a riser through the
         pull-apart cut off by a bass hit on the snap, a sparkle with the shine, a key press per tagline letter.
         Each placed so its hit lands one frame after its picture.
SHOTS:
  0.20-0.50  the K's blue stem and arm drop in from the top and land with a squash.
  0.72-0.98  the navy leg kicks in along its own diagonal from the lower right and locks into the K.
  1.12-1.52  the S rolls in from the right, a full turn, and lands.
  1.68-1.95  the L slides in from the right and completes KSL: bass hit.
  2.12       the logo punches (1.05x).
  2.35-3.52  K, S and L pull apart and tilt as the riser climbs, then snap back together on a bass hit.
  3.62-4.22  a shine sweeps across the letters, left to right.
  4.35-5.30  COMMERCIAL CLEANING types in, letter by letter.
  5.30-7.50  hold.
BANNED:  glow outside the letters, particles, gradients on the ground, lens flares, anything fading in.
QA:      0.5, 0.9, 1.3, 1.9, 2.8, 3.4, 3.8, 4.0, 4.6, 5.1, 6.5 s; the final frame against the supplied SVG.
