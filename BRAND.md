# OrynDesign brand tokens

The single reference for the colours, type and logo used on the organisation profile (`profile/`).
If a value here changes, the SVG images in `profile/assets/` must be regenerated: their text is converted to outlines, so they do not pick up changes by themselves.

## Accent palette: Ocean

Adopted on 2026-11-17. A cyan that flows into a blue.

| Role | Name | Hex | Where it is used |
|---|---|---|---|
| Primary accent | Ocean Cyan | `#1ABFFF` | halo behind the logo, "open" in the tagline, icons, bars, number badges, the highlighter behind "open" / "Open" |
| Secondary accent | Ocean Blue | `#3A63FF` | far end of the flow lines, glow and bottom bars (cyan to blue gradient) |
| Highlight (dark theme) | Ocean Mist | `#98E2FF` | top of the accent text gradient. Derived: Ocean Cyan mixed 55% with white |
| Line on light | Deep Cyan | `#1495C7` | thin lines and borders on white. Derived: Ocean Cyan darkened to 3.4:1 contrast on white |
| Accent text on light | Ocean Ink | `#117EA8` | small labels such as "01" and "NEXT RELEASE" on white. 4.6:1 contrast |
| Text on accent fills | Ink | `#0A0A09` | text on Ocean Cyan surfaces (pills, highlighter). 9.4:1 contrast |

On light backgrounds never use Ocean Cyan for thin lines or small text: it has only 2.1:1 contrast on white. Use the deep values above, or a solid cyan surface with Ink text.

## Neutrals

| Token | Dark theme | Light theme |
|---|---|---|
| Card / page top | `#0E1315` | `#FFFFFF` |
| Card / page bottom | `#030506` | `#E1F7FF` (Ocean Cyan at 13% on white) |
| Heading, top of gradient | `#FFFFFF` | `#0A0A09` |
| Heading, bottom of gradient | `#B0B8BC` | `#34373D` |
| Body text | `#869196` | `#565B63` |
| Border | `#FFFFFF` at 10% | `#19BBFA` at 22% |
| Footer text (both themes) | `#888D95` | `#888D95` |

The dark neutrals are greys mixed with a small share of Ocean Cyan (1% to 7% depending on the token) so that the page does not look flat against the accent.

## Logo

White interlocking knot on a black rounded square. It is never recoloured.

| Part | Colour |
|---|---|
| Tile | radial sheen from `#5E5F61` through `#2A2B2D` and `#0A0A0A` to `#050505` |
| Knot | `#FFFFFF` to `#D9DCD6` |
| Tile border | `#5E6066`, one flat grey all the way round: no gradient and no accent colour, so every edge looks the same |

## Product marks

### Solidify

Files in `brand/solidify/`: `solidify-mark.svg` (the app icon) and `solidify-lockup-dark.svg` / `solidify-lockup-light.svg` (icon, wordmark and "BY ORYNDESIGN").

An S made of straight bars and two semicircles, with a uniform stroke and flat ends. A solid S sits in front of its own triangle mesh, offset down and to the right: what it was, behind what it is now. It uses the same black tile and the same tile border as OrynDesign; the Ocean colours appear only inside the S.

| Part | Colour |
|---|---|
| Solid S | gradient `#98E2FF` to `#1ABFFF` to `#3A63FF` |
| Mesh behind | Ocean Cyan at 20% fill with Ocean Mist `#98E2FF` lines |
| Wordmark | Inter 600, tracking -0.03 em, the two i-dots replaced by Ocean diamonds |

## Type

[Inter](https://rsms.me/inter/) (SIL Open Font License): 600 for the wordmark and headings (wordmark tracking -0.028 em), 400 for body text, 500 for small captions.

## CSS variables

```css
:root {
  --oryn-cyan: #1ABFFF;
  --oryn-blue: #3A63FF;
  --oryn-mist: #98E2FF;
  --oryn-deep-cyan: #1495C7;
  --oryn-ocean-ink: #117EA8;
  --oryn-ink: #0A0A09;
  --oryn-tile-border: #5E6066;
  --oryn-dark-top: #0E1315;
  --oryn-dark-bottom: #030506;
  --oryn-light-bottom: #E1F7FF;
}
```

## Palette history

| Date | Accent | Note |
|---|---|---|
| 2026-11-16 | Acid green `#BEF73A` | first banner |
| 2026-11-17 | Amber `#FFAA00` | chosen from a sweep of "acid orange" tones (hue 32 to 68 degrees) |
| 2026-11-17 | **Ocean `#1ABFFF` to `#3A63FF`** | current |

<details>
<summary>Other palettes considered for the final round</summary>

| Name | Hex |
|---|---|
| Ultraviolet | `#8F6BFF` to `#D94BFF` |
| Coral | `#FF5A7A` to `#FF9F6B` |
| Emerald | `#2BE39A` to `#00AFA0` |
| Signal Red | `#FF3B30` to `#C9183A` |
| Magenta | `#FF2E93` to `#FF6FB5` |
| Ice | `#BFE3FF` to `#7FB8FF` |
| Indigo | `#6A5CFF` to `#22D3EE` |
| Graphite | `#FFFFFF` to `#A9AEB5` |
| Lilac | `#B9A2FF` to `#7C9CFF` |

</details>
