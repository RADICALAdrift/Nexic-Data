# Contributing

Thank you for your interest in contributing to **Nexic-Data**.

This repository maintains categorized creator data used by the Nexic Discord bot and other tools. Contributions that improve the accuracy or completeness of the dataset are always welcome.

---

## Ways to Contribute

You can help improve this dataset by:

- Adding new creators
- Correcting platform identifiers
- Suggesting commonly used nicknames
- Fixing formatting issues
- Reporting errors in existing entries

If you are unsure about a change, feel free to open an **Issue** first to discuss it.

---

## Dataset Format

Each entry follows this structure:

```json
"CreatorName": {
  "nickname": "OptionalNickname",
  "platforms": [
    {"identifier": "creatorname", "type": "twitch"},
    {"identifier": "creatorname", "type": "twitter"},
    {"identifier": "creatorname", "type": "youtube"}
  ]
}
```

### Field Description

| Field | Description |
|-----|-----|
| display name | The creator's public name used as the JSON key |
| nickname | Optional short name used by the bot |
| platforms | List of platform identifiers |

---

## Platform Identifier Rules

Identifiers should match the creator's **actual platform username**.

Examples:

| Platform | Example |
|--------|--------|
| Twitch | `lordaethelstan` |
| Twitter/X | `LordAethelstan` |
| YouTube | `lordaethelstan69` |

Do **not include full URLs**. Only include the username/identifier.

---

## Formatting Guidelines

Please follow these guidelines when editing JSON files:

- Maintain valid JSON formatting
- Keep indentation consistent
- Follow the existing structure
- Avoid duplicate entries
- Place creators in the correct category file

Example category files include:

- `twitch_indie.json`
- `twitch_sva.json`
- `twitch_phase_connect.json`
- `twitch_vchiban.json`

---

## Pull Requests

When submitting a pull request:

1. Clearly describe what you added or changed
2. Ensure the JSON file remains valid
3. Keep changes focused on a single improvement where possible

Pull requests may be reviewed and adjusted to maintain formatting consistency.

---

## Notes

This dataset is primarily maintained for the **Nexic Discord Bot**, but the data may be useful for other community tools and projects.

Thank you for helping improve the dataset!