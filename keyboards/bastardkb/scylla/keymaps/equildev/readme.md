# equildev keymap for Bastard Keyboards Scylla (mk2)

Decoded 1:1 from an Argos configuration export (`argos_config.json`, keycodes 8 layers x 60 matrix entries, 10 rows x 6 cols, right half mirrored), mapped through the board's `info.json` (`LAYOUT_split_4x6_5`, 58 keys, thumbs in matrix rows 4/9).

Requires the **Argos community module** (declared in `keymap.json`), which provides at runtime from EEPROM:

- combo 0: `Space` + `Backspace` → `Tab`, enabled (no `TD()` keycodes are referenced; all 50 Argos tap-dance slots are empty in this export)
- macros 0-4 (`QK_MACRO_0..4` referenced on layers 1-2)
- per-layer RGB colors (see the table in `keymap.c`)
- tapping term / combo settings

Layers 3-7 exist in the export and are all-transparent; they are included so flash matches what Argos reports.

The vendor keymap (`../vendor/`) is left untouched.
