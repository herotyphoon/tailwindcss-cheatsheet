# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

- Placeholder for upcoming changes

---

## [1.0.0] — 2026-03-15

### Added

- Initial release of the Tailwind CSS Cheatsheet
- **Layout** — Display, Position, Z-Index, Overflow, Float, Aspect Ratio, Columns, Break
- **Flexbox** — Direction, Wrap, Justify Content, Align Items/Content/Self, Justify Self, Place utilities, Flex Grow/Shrink/Basis, Order, Gap
- **Grid** — Template Columns/Rows, Column/Row Span, Start/End, Auto Flow, Auto Cols/Rows, Subgrid support
- **Spacing** — Full padding and margin scale (0 → 96) including half-steps, negative margins, space-between utilities
- **Sizing** — Width, Height, Min/Max Width/Height with all fractions, keywords, and viewport units (svh, dvh, lvh, svw, dvw)
- **Typography** — Font Size (xs → 9xl), Font Weight (thin → black), Font Family, Font Style, Text Alignment, Text Transform, Text Decoration, Underline Offset, Line Height, Letter Spacing, Whitespace, Word Break, Truncate, Hyphens, Vertical Align
- **Colors** — All 22 color palettes (slate, gray, zinc, neutral, stone, red, orange, amber, yellow, lime, green, emerald, teal, cyan, sky, blue, indigo, violet, purple, fuchsia, pink, rose) × 11 shades (50 → 950) rendered as visual swatches
- **Opacity** — 0 → 100 scale
- **Backgrounds** — Attachment, Clip, Origin, Repeat, Size, Position, Image, Gradients (all 8 directions, from/via/to stops, positional stops, opacity modifiers)
- **Borders** — Width (all sides), Color, Style, Radius (all directions and corners), Divide utilities, Outline, Ring (with offset and color)
- **Effects** — Box Shadow (sm → 2xl, inner, none, color modifiers), Mix Blend Mode (17 values), Background Blend Mode
- **Filters** — Blur, Brightness, Contrast, Grayscale, Hue Rotate, Invert, Saturate, Sepia, Drop Shadow; all repeated for Backdrop Filter
- **Transforms** — Scale (x/y), Rotate, Translate (x/y, fractions), Skew (x/y), Transform Origin (9 positions), transform-gpu, transform-none
- **Transitions** — Property, Duration (0 → 1000ms), Timing Function, Delay
- **Animation** — spin, ping, pulse, bounce; custom animation config example
- **Interactivity** — Cursor (15 values), Pointer Events, User Select, Resize, Scroll Behavior, Scroll Margin/Padding, Scroll Snap (align, type, stop), Touch Action, Will Change, Appearance, Caret Color, Accent Color
- **Responsive Breakpoints** — Visual bar chart for sm/md/lg/xl/2xl, max-* variants, 50+ pseudo-class and state variants
- **Dark Mode** — class and media strategy, toggle example
- **Group & Peer** — hover/focus/checked/disabled variants, named groups and peers
- **Arbitrary Values** — Full syntax examples including arbitrary properties and variants
- **Configuration** — Complete `tailwind.config.js` template with theme extension, custom colors, fonts, spacing, animations, keyframes, plugins
- **Directives** — @tailwind, @layer (base/components/utilities), @apply, theme(), screen()
- **Common Patterns** — Center a div, absolute center, gradient text, frosted glass, responsive sidebar, card hover lift, CSS grid auto-fill
- **Tables** — table-auto/fixed, border-collapse/separate, border-spacing, caption-side
- **Lists** — list-style-type/position/image
- **SVG** — fill, stroke, stroke-width
- **Accessibility** — sr-only, not-sr-only with CSS definition

### Design

- Dark theme with CSS variables for easy customization
- Sticky navigation bar with section jump links
- Color-coded sections (sky, violet, emerald, pink, orange)
- JetBrains Mono for code, Syne for headings
- Visual breakpoint bar chart
- Responsive 2-column grid layout
- Print-friendly styles (nav hidden)
- Scroll-to-top button
- Zero dependencies (single HTML file, one Google Fonts import)

---

[Unreleased]: https://github.com/YOUR_USERNAME/tailwind-cheatsheet/compare/v1.0.0...HEAD
[1.0.0]: https://github.com/YOUR_USERNAME/tailwind-cheatsheet/releases/tag/v1.0.0
