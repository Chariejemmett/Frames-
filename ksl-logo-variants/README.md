# KSL logo: softer variations

Three calmer takes on the KSL Commercial Cleaning logo animation (`../ksl-logo-sting` is the original, bouncier
version). Each is its own HyperFrames project: 1920 x 1080, 60 fps, 6.5 s, built from the supplied SVG, with no
squash, overshoot, punches or snaps. Sounds are soft swells, whooshes and a sparkle from the HyperFrames bundle
(Pixabay licence).

| Project | What happens | Sound |
| --- | --- | --- |
| `ksl-focus` | K, the navy leg, S and L each fade up out of a soft blur, 0.25 s apart; a slow shine; the tagline fades in letter by letter out of a light blur. | a cinematic swell peaking as the L sharpens, a sparkle on the shine, a soft whoosh under the tagline |
| `ksl-wipe` | a soft-edged wipe passes left to right and leaves KSL behind it; the navy leg fades in last, easing down its diagonal; a shine; the tagline gets its own quicker wipe. | a slow whoosh for each wipe, a soft one for the leg, a sparkle on the shine |
| `ksl-settle` | each letter fades in slightly large and blurred and settles to size; the tagline fades in as its wide letter spacing closes up; a shine to finish. | a cinematic swell under the letters, a soft whoosh as the tagline closes, a sparkle on the shine |

Render one with `npx hyperframes render --fps 60 --quality delivery -o renders/<name>.mp4` from its folder.
Colours (background, light blue, navy) are composition variables in each `index.html`.
