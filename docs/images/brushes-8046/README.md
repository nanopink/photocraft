# Brushes panel evidence for #8046

These images support the pull request; this evidence branch is not intended for merging.

- `before.png`: base commit `98de85c64`, which already includes #8162's preview-size slider.
- `after-menu.png`: the new gear menu with only Brush Stroke enabled.
- `after-grid.png`: grid view with only Brush Tip enabled and preview scale 0.75.

The after images were captured from `cb9cf898a`. Its Brushes changes match
`6c4f56276`, the implementation commit in the focused pull request.

Captures use the existing `snapshot` example, Vulkan with `--safe-gpu`, a blank
600x400 document, a 1100x800 viewport at scale 1, the `proMedium` theme, and a
350-point right dock. No personal artwork is included.

Original captures by @nanopink, MIT OR Apache-2.0. Embedded PhotoCraft assets and
branding retain their existing licenses; see the repository attribution and
`docs/brand/LICENSE-brand.txt`.

## Narrow panel follow-up

- `narrow-before.png`: before the width bound, at `3cb042237`.
- `narrow-after.png`: the width bound in `7cf0fbf8e`, keeping the full card within the panel.

These use the same blank document, viewport and theme as above, with `dockWidth`
requested at 180, `brushesView` set to `grid`, and `brushesScale` set to 2. The app
retains its normal dock minimum width. All three preview parts are enabled.
