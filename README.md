# Sajdah Guide — Quran data cache

Static, pre-generated per-Surah JSON: Arabic Uthmani text, Tajweed markup, Fateh Muhammad
Jalandhry's Urdu translation, and Tafsir al-Muyassar — the same default reading data the
[Sajdah Guide](https://github.com/redfleet/redfleet-sajdah) app fetches live from
[api.alquran.cloud](https://alquran.cloud), generated once and served from here via
[jsDelivr](https://www.jsdelivr.com/) (`cdn.jsdelivr.net/gh/redfleet/redfleet-sajdah-quran-data@main/...`)
for speed and reliability, with the live API kept as a fallback for anything not cached here
(other translation/Tafsir languages, word-by-word data, audio, etc.).

No reciter audio or other copyrighted recorded performance is mirrored in this repo —
intentionally out of scope. Just the same freely-redistributed Quran text/translation/Tafsir
every public Quran API already publishes.

- `manifest.json` — which editions and how many Surahs this snapshot covers
- `data/surah/{number}.json` — one file per Surah (1-114)

See `manifest.json`'s `generatedAt` for when this was last regenerated.
