# Nexic-Data

This repository contains shared community-maintained data used by the Nexic Discord Bot on the Nexus Assault Discord. The primary purpose is to define and organize Twitch channel mappings for various Streamers & VTuber groups and independents, used by the bot to manage autolive notifications and more.

---

## 📂 Current Structure

The main content includes categorized JSON files, such as the ones in channel_maps/

- `twitch_beastiez.json`
- `twitch_ex_vshojo_en.json`
- `twitch_ex_vshojo_jp.json`
- `twitch_fleshtuber.json` - Regular Twitch streamers (a joking term used in the VTuber community for non-VTuber creators)
- `twitch_indie.json`
- `twitch_phase_connect.json`
- `twitch_sva.json`
- `twitch_vchiban.json`
- More categories may be added over time...

Each JSON file defines a mapping of VTuber display names to their Twitch identifiers and may include optional metadata (like tags or maturity rating) for future functionality.

Examples:
```json
  "Aethelstan": [{"type": "twitch", "identifier": "aethelstan", "nickname": "Aethel"}],
  "BananaJuju": [{"type": "twitch", "identifier": "bananajuju", "nickname": "Juju"}],
  "Camila": [{"type": "twitch", "identifier": "camila"}],
```
```json
"Aethelstan": [
  {
    "type": "twitch",
    "identifier": "aethelstan",
    "nickname": "Aethel"
  }
]
```

The top example is preferred Thank you
