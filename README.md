# Bat

A [bat](https://github.com/sharkdp/bat) theme for the ambitious.

## Installation

1. Clone repository
2. Create bat theme folder
   ```bash
   mkdir -p "$(bat --config-dir)/themes"
   ```
3. Copy `Embark.tmTheme` from repository into theme folder
   ```bash
   cp Embark.tmTheme "$(bat --config-dir)/themes"
   ```
4. Rebuild `bat` cache so it can find theme
   ```bash
   bat cache --build
   ```
5. Run `bat --list-themes | grep Embark` and ensure that it is found. If it isn't one of the previous steps wasn't done
   properly.

## Usage

You can either set the theme by passing the the `--theme="Embark"` flag to any bat invocation.

```bash
Cat --theme="Embark" README.md
```

Or, set it as the default theme in configuration.

```bash
echo "--theme=Embark" > $(bat --config-dir)/config
```

## Thanks to

* [Catppuccin Bat Theme](https://github.com/catppuccin/bat)
