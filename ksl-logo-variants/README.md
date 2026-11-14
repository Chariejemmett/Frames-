# KSL logo: softer variations

Three calmer takes on the KSL Commercial Cleaning logo animation (`../ksl-logo-sting` is the original, bouncier
version). Each is its own HyperFrames project: 1920 x 1080, 60 fps, 6.5 s, built from the supplied SVG, with no
squash, overshoot, punches or snaps. In all three the K's navy leg comes last: it streaks in along its own diagonal
from off the lower right with three fading after-images and glides to a stop. Sounds are soft swells and whooshes
from the HyperFrames bundle (Pixabay licence).

| Project | What happens | Sound |
| --- | --- | --- |
| `ksl-focus` | K, S and L each fade up out of a soft blur, 0.25 s apart; the leg streaks in; the tagline fades in letter by letter out of a light blur. | a cinematic swell, a swish on the leg, a soft whoosh under the tagline |
| `ksl-wipe` | a soft-edged wipe passes left to right and leaves K, S and L behind it; the leg streaks in; the tagline gets its own quicker wipe. | a slow whoosh for each wipe, a swish on the leg |
| `ksl-settle` | K, S and L fade in slightly large and blurred and settle to size; the leg streaks in; the tagline fades in as its wide letter spacing closes up. | a cinematic swell under the letters, a swish on the leg, a soft whoosh as the tagline closes |

Render one with `npx hyperframes render --fps 60 --quality delivery -o renders/<name>.mp4` from its folder.
Colours (background, light blue, navy) are composition variables in each `index.html`.
