# Liquid Glass for Zed

A native dark liquid glass theme for [Zed](https://zed.dev) inspired by Apple design.

Frosted translucent chrome surrounds a solid, readable editor. System blue accents. Built for macOS.

---

## Features

- **Native macOS blur** — Uses Zed's `"blurred"` window background for genuine liquid glass
- **Solid editor** — The code area stays opaque and readable (`#0a0a0a`)
- **Translucent chrome** — Sidebar, panels, title bar, and status bar float with frosted glass
- **Apple palette** — System blue (`#0A84FF`) accents, off-white text, and clean semantic colors
- **Apple-inspired syntax** — Soft peach strings, lavender keywords, cyan functions, mint types

---

## Preview

*(Add a screenshot here once you've tested it!)*

---

## Local Installation

1. Copy this repo's `themes/liquid-glass.json` into your Zed themes directory:
   ```bash
   mkdir -p ~/.config/zed/themes
   cp themes/liquid-glass.json ~/.config/zed/themes/
   ```

2. Open Zed and select **Liquid Glass** from the theme picker (`Cmd + K, Cmd + T`).

3. Restart Zed if the theme does not appear immediately.

---

## Live Tweaking

To iterate quickly on colors without restarting Zed, add overrides to your `~/.config/zed/settings.json`:

```json
{
  "theme": "Liquid Glass",
  "theme_overrides": {
    "Liquid Glass": {
      "editor.background": "#0d0d0d",
      "accent": "#007AFF"
    }
  }
}
```

Zed will hot-reload the changes.

---

## Publishing to the Zed Extension Store

To make this theme available to everyone:

1. **Fork** the [Zed extensions repository](https://github.com/zed-industries/extensions)
2. **Add this repo as a submodule** under the `extensions/` directory:
   ```bash
   cd extensions
   git submodule add https://github.com/yourusername/liquid-glass-zed.git liquid-glass
   ```
3. **Update `extensions.toml`** in the extensions repo to include your theme
4. **Open a Pull Request**

See the [official docs](https://zed.dev/docs/extensions/themes) for full details.

---

## Credits

- Apple design language and system colors
- Inspired by [Ayu Glass](https://github.com/jansol/zed-ayu-glass) for Zed

---

## License

MIT
