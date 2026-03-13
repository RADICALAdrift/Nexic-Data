# Nexic-Data

This repository contains shared, community-maintained data used by the **Nexic Discord Bot** on the Nexus Assault Discord server.

The primary purpose of this repository is to define and organize creator mappings for streamers, VTubers, and other creators. These mappings are used by the bot to power features such as **auto-live notifications** and other automation systems.

---

## Repository Structure

Creator data is organized into categorized JSON files located in:

`channel_maps/`

Examples include:

- `twitch_beastiez.json`
- `twitch_ex_vshojo_en.json`
- `twitch_ex_vshojo_jp.json`
- `twitch_fleshtuber.json` *(regular Twitch streamers — a joking term used in the VTuber community for non-VTuber creators)*
- `twitch_indie.json`
- `twitch_nexusandfriends.json` *(Nexus Assault specific streamers and community friends)*
- `twitch_phase_connect.json`
- `twitch_sva.json`
- `twitch_vchiban.json`

Additional categories may be added over time as the dataset grows.

---

## File Format

Each JSON file maps a creator's **display name** to platform identifiers.

Example:

```json
"LordAethelstan": {
  "nickname": "Aethel",
  "platforms": [
    {"identifier": "lordaethelstan", "type": "twitch"},
    {"identifier": "LordAethelstan", "type": "twitter"},
    {"identifier": "lordaethelstan69", "type": "youtube"}
  ]
}
```

Field descriptions:

- **display name** – the creator's public name used as the JSON key  
- **nickname** – optional short name used by the bot for notifications  
- **platforms** – list of platform identifiers for the creator  

Currently supported platform types include:

- `twitch`
- `twitter`
- `youtube`

Additional platforms may be added in the future.

---

## Optional Fields

Some entries may include optional metadata.

Example without nickname support:

```json
"LordAethelstan": {
  "platforms": [
    {"identifier": "lordaethelstan", "type": "twitch"},
    {"identifier": "LordAethelstan", "type": "twitter"},
    {"identifier": "lordaethelstan69", "type": "youtube"}
  ]
}
```

If a **nickname** is present, the bot may use it when generating live notifications.

If no nickname is provided, the bot will fall back to the creator's display name.

Future metadata fields may include information such as agency affiliations or former identities.

---

## Contributing

Community contributions are welcome.

If you would like to contribute to this dataset, please see **CONTRIBUTING.md** for contribution guidelines.

You can contribute by opening:

- a **Pull Request**
- an **Issue** for discussion

---

## Notes

This repository is maintained primarily for use with the **Nexic Discord Bot**, but the dataset may also be useful for other tools or projects that need categorized creator lists.

---

## Future Expansion

The dataset structure is designed to be flexible and may support additional metadata over time, such as:

- creator friendships
- agency affiliations
- additional platforms
- tags or categories

---

## Example Use Cases

The dataset may be useful for:

- Discord bots
- creator discovery tools
- streaming dashboards
- community projects