# Nexic-Data

This repository contains shared community-maintained data used by the Nexic Discord Bot on the Nexus Assault Discord. The primary purpose is to define and organize Twitch channel mappings for various Streamers & VTuber groups and independents, used by the bot to manage autolive notifications and more.

---

## 📂 Current Structure

The main content includes categorized JSON files, such as the ones in channel_maps/

- `CHANNEL_MAP_TWITCH.json`
- `CHANNEL_MAP_TWITCH_EX_VSHOJO_EN.json`
- `CHANNEL_MAP_TWITCH_EX_VSHOJO_JP.json`
- `CHANNEL_MAP_TWITCH_EX_VSHOJO_JP_NOVA.json`
- `CHANNEL_MAP_TWITCH_INDIE.json`
- `CHANNEL_MAP_TWITCH_VCHIBAN.json`
- More categories may be added over time...

Each JSON file defines a mapping of VTuber display names to their Twitch identifiers and may include optional metadata (like tags or maturity rating) for future functionality.

Examples:
```json
"Kson": [{"type": "twitch", "identifier": "ksonsouchou", "tags": ["mature", "variety"], "mature": true}]
```
```json
"Kson": [
  {
    "type": "twitch",
    "identifier": "ksonsouchou",
    "tags": ["mature", "variety"],
    "mature": true
  }
]
```

The top example is preferred Thank you
