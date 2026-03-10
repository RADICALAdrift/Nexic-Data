# Nexic-Data

This repository contains shared, community-maintained data used by the **Nexic Discord Bot** on the Nexus Assault Discord server.

The primary purpose of this repository is to define and organize **Twitch channel mappings** for Streamers, VTuber groups, and independent creators. These mappings are used by the bot to power features such as **auto-live notifications** and other automation systems.

---

## Current Structure

The repository currently includes categorized JSON files located in `channel_maps/`.

Examples include:

- `twitch_beastiez.json`
- `twitch_ex_vshojo_en.json`
- `twitch_ex_vshojo_jp.json`
- `twitch_fleshtuber.json`  
  *(Regular Twitch streamers — a joking term used in the VTuber community for non-VTuber creators)*
- `twitch_indie.json`
- `twitch_phase_connect.json`
- `twitch_sva.json`
- `twitch_vchiban.json`

Additional categories may be added over time as the dataset grows.

---

## File Format

Each JSON file maps a creator's **display name** to their Twitch login identifier.

Example:

```json
"Aethelstan": [{"type": "twitch", "identifier": "aethelstan"}],
"BananaJuju": [{"type": "twitch", "identifier": "bananajuju"}],
"Camila": [{"type": "twitch", "identifier": "camila"}]
```

This **single-line format is preferred** for readability and consistency.

---

## Optional Fields

Some entries may include optional metadata.

Example with nickname support:

```json
"ChonkyLotus": [{"type": "twitch", "identifier": "chonkylotus", "nickname": "Chonky"}]
```

If a nickname is present, the bot may use it when generating live notifications.

If no nickname is provided, the bot will fall back to the creator's display name.

---

## Contributing

Community contributions are welcome.

You can help by:

- Adding new creators
- Correcting Twitch identifiers
- Suggesting or correcting commonly used nicknames
- Fixing formatting issues

If you would like to contribute, feel free to open:

- a **Pull Request**
- an **Issue** for discussion

Please ensure that:

- Twitch identifiers are correct
- JSON formatting remains consistent
- entries follow the preferred single-line format where possible

---

## Notes

This repository is maintained for use with the **Nexic Discord Bot**, but the data may also be useful for other tools or projects that need categorized Twitch creator lists.
