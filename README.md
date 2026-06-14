# zmk-corne-config

Personal [ZMK](https://zmk.dev) firmware configuration for a [Corne](https://github.com/foostan/crkbd) (CRKBD) split keyboard.

- **Controller:** nice!nano v2 (`nice_nano_v2`)
- **Shield:** `corne_left` / `corne_right`

## Building

Firmware is built automatically by GitHub Actions on every push. Download the
`firmware` artifact from the latest run on the
[Actions tab](../../actions), unzip it, and you'll find:

- `corne_left-nice_nano_v2-zmk.uf2`
- `corne_right-nice_nano_v2-zmk.uf2`

## Flashing

1. Put a half into bootloader mode by double-tapping the reset button. It mounts
   as a USB drive named `NICENANO`.
2. Drag the matching `.uf2` file onto the drive. It will reboot automatically.
3. Repeat for the other half.

## Customizing

- `config/corne.keymap` — key bindings and layers
- `config/corne.conf` — feature flags (RGB underglow, OLED display, etc.)
- `build.yaml` — board/shield build matrix

See the [ZMK docs](https://zmk.dev/docs) for details.
