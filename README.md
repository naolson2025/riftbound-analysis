# Riftbound Analysis

CSV dumps of all Riftbound TCG card sets from the official card gallery.

Source: https://playriftbound.com/en-us/card-gallery/
API: `https://content.publishing.riotgames.com/publishing-content/v2.0/public/channel/riftbound_website/list/riftbound_gallery_cards?locale=en_US&from=0&limit=2000`

Fetched 2026-08-30 via `curl` + `fetch` script. Total unique cards: **1189** (verified with `limit=2000&from=0` directly returns 1189; page `totalItems:1197` stale).

## Sets

| File | Set | Cards | Collector Numbers | Notes |
|------|-----|-------|-----------------|-------|
| `OGN-Origins.csv` | Origins (OGN) | 352 | 298 + 54 alt/showcase | Main set |
| `OGS-Proving-Grounds.csv` | Origins Proving Grounds (OGS) | 24 | 24 | Starter set |
| `SFD-Spiritforged.csv` | Spiritforged (SFD) | 288 | 221 + overnumbered | Set 2 (Feb 13 2026 ENG, Dec 12 2025 CN) |
| `UNL-Unleashed.csv` | Unleashed (UNL) | 288 | 219 + overnumbered | Set 3 (May 2026) |
| `VEN-Vendetta.csv` | Vendetta (VEN) | 237 | 166 + overnumbered | Set 4 (July 31 2026 unified) |
| `ALL-SETS.csv` | All | 1189 | — | Concatenated, sorted by set+collectorNumber |

Upcoming `Radiance` not yet in gallery.

## Columns

`id,publicCode,collectorNumber,name,set_id,set_label,rarity_id,rarity_label,cardType,superType,domain,energy,might,power,tags,ability_text,accessibilityText,illustrator,orientation,cardImage_url`

- `ability_text` cleaned from `text.richText.body` HTML (`<br />` → newline, tags stripped, `html.unescape`)
- `cardType`/`superType`/`domain` comma-joined labels
- `energy`/`might`/`power` from `energy.value.label` / `might.value.label` / `power.value.label` (fallback to raw value)
- Sorted by `collectorNumber`

## Usage

```bash
# example count rows per set
python3 -c "import csv; print(len(list(csv.DictReader(open('OGN-Origins.csv')))))"
```

## Re-fetch

See `/tmp/fetch_riftbound.py` (original script used `curl -sL` pagination `from 0 to 1200 step 200` + `limit 2000` verification + `csv.DictWriter` with UTF-8).

## License

Data © Riot Games / Riftbound. CSVs provided for analysis.
