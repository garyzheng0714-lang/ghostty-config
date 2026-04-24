# Ghostty Configuration

## Overview

Personal [Ghostty](https://ghostty.org/) terminal configuration files. The repository currently contains one Gruvbox Dark Hard based profile with a MonoLisa font setup, subtle transparency, blur, padded windows, and selection/cursor preferences.

## Available Configurations

| Config | Description |
|--------|-------------|
| [gruvbox-dark-hard](./configs/gruvbox-dark-hard/config) | Gruvbox Dark Hard theme with subtle transparency and blur |

## Project Structure

```text
.
├── README.md
└── configs/
    └── gruvbox-dark-hard/
        ├── README.md
        └── config
```

## Usage

Copy the desired profile to Ghostty's config path:

```bash
cp configs/<config-name>/config ~/.config/ghostty/config
```

For the current profile:

```bash
mkdir -p ~/.config/ghostty
cp configs/gruvbox-dark-hard/config ~/.config/ghostty/config
```

Restart Ghostty or reload the configuration after copying.

## Gruvbox Dark Hard Settings

| Setting | Value |
| --- | --- |
| Theme | `Gruvbox Dark Hard` |
| Font | `MonoLisa Variable` |
| Font size | `12` |
| Window size | `110` columns by `30` rows |
| Background opacity | `0.95` |
| Background blur radius | `20` |
| Cursor style | Block, blinking, `0.8` opacity |
| macOS titlebar style | `tabs` |
| Window padding | `15` x, `10` y |
| Selection behavior | `copy-on-select = clipboard` |

## Notes

- The config assumes `MonoLisa Variable` is installed locally. Change `font-family` and `window-title-font-family` if you use another font.
- The profile disables common ligature features with `font-feature` settings.
- `shell-integration-features = no-cursor` leaves cursor behavior to the explicit cursor settings in this config.
