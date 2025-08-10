## 📁 Structure

- `channel_maps/` — JSON files containing channel maps for Twitch Streamers & VTubers.

## 🛠️ Usage

These files are read by Nexic's Autolive system to determine which channels to announce when Streamers & VTuber go live in the Nexus Assault Discord.

Each JSON file contains a dictionary of VTuber names and their Twitch identifiers, e.g.:

```json
{
  "Ironmouse": [{ "type": "twitch", "identifier": "ironmouse"}]
}
