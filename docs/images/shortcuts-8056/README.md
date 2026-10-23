# Shared tool key evidence for #8056

Both captures explicitly save `B` as the Brush shortcut, select Pencil and press
plain B once. The Shift-switch preference is enabled, its current default.

- `before.png`: the tool changes to Brush. The options bar shows Flow.
- `after.png`: Pencil remains selected. The options bar shows Auto Erase.

The before renderer has no shortcut changes; the after renderer is from
`cb9cf898a`, whose shortcut changes match the focused PR's `d1c60828c`.
Both use the existing `snapshot` example, Vulkan with `--safe-gpu`, a blank
600x400 document and a 1100x800 viewport at scale 1 with the `proMedium` theme.

The control script sets `shortcuts.tools.select.brush` to `B` through `prefs.set`,
then runs `ui.set {"tool":"pencil"}` and `ui.key {"key":"B"}`.

Original captures by @nanopink, MIT OR Apache-2.0. Embedded PhotoCraft assets and
branding retain their existing licenses; see the repository attribution and
`docs/brand/LICENSE-brand.txt`. This evidence branch is not intended for merging.
