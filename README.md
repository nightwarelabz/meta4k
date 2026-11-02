# meta4k

A ten-second seamless loop of the Meta ribbon and wordmark, computed
entirely in [Krell](https://github.com/nightwarelabz/krell) — every pixel
of every frame is accumulated from mathematical samples; nothing is drawn,
textured, or composited from image assets beyond the reference lockup the
letterforms and ribbon silhouette were measured from.

## Specification

- 3840 × 2160, 30 fps, 300 frames, exactly 10.000 s
- 11,200,000 samples per frame: an 8.8M-sample woven thread for the ribbon
  and 2.4M white-light motes over a living multi-shade white field
- Frame 300 is byte-identical to frame 0 — the loop closes exactly

## Construction

- The ribbon's centreline is a Fourier series through the seventh harmonic,
  fitted by least squares to the medial axis of the reference ribbon.
- The band is a Möbius weave: a triangular stitch at 880 crossings per
  circuit, two interlaced families, with the fold placed at the crossing
  and a blue gradient running from (0, 96, 219) to (0, 200, 255).
- Mid-film, the ribbon phi-warps through a Poincaré-disk Möbius
  automorphism whose centre path is zero at both ends, so the film starts
  and ends on the perfect still.
- The background is a domain-warped multi-sine white field with a soft
  blue aura — two drifting low-frequency fields and a breathing halo —
  morphing continuously through the loop.
- The wordmark is sampled from a native-resolution mask of the reference
  letterforms with smoothstepped coverage.

## Files

- `meta4k.png` — the frame-0 still at full 3840 × 2160
- The films are attached to this repository's
  [Releases](https://github.com/nightwarelabz/meta4k/releases): the 4K
  master and a 1080p view copy
