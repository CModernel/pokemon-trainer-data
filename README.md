# Pokémon Trainer Academy — Data Repository

Public data repository for the **Pokémon Trainer Academy** app.
Contains Pokémon data, generation info, and curated competitive
game data (abilities, moves, items).

---

## 📁 Structure

\`\`\`
pokemon-trainer-data/
  data/
    v1/
      pokemon-data.json     ← 1025 Pokémon with stats, types, generation
      generations.json      ← Generation & region metadata
      abilities.json        ← Curated competitive abilities (coming soon)
      moves.json            ← Curated competitive moves (coming soon)
      items.json            ← Curated competitive items (coming soon)
    latest.json             ← Version manifest for app update checks
\`\`\`

---

## 🔄 Data Updates

Data is automatically updated daily via GitHub Actions.
The script fetches from [PokéAPI](https://pokeapi.co) and commits
any changes automatically.

### latest.json format
\`\`\`json
{
  "latestDataVersion": 1,
  "minAppVersion": "1.0.0",
  "changelog": "Initial release"
}
\`\`\`

---

## 🌐 CDN Access via jsDelivr

All files are accessible via jsDelivr CDN:

\`\`\`
https://cdn.jsdelivr.net/gh/USERNAME/pokemon-trainer-data@main/data/v1/pokemon-data.json
https://cdn.jsdelivr.net/gh/USERNAME/pokemon-trainer-data@main/data/v1/generations.json
\`\`\`

---

## 📜 License

### Code & JSON structure
MIT License — see [LICENSE](LICENSE)

### Pokémon data
Pokémon data is sourced from [PokéAPI](https://pokeapi.co), which is
licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

Pokémon and all related names, characters, and media are trademarks
of Nintendo, Game Freak, and The Pokémon Company.
This project is not affiliated with or endorsed by any of these companies.

---

## ⚠️ Disclaimer

This is a fan-made project and is not affiliated with, endorsed by,
or connected to Nintendo, Game Freak, or The Pokémon Company.

Pokémon, the Pokémon character names, and all related media are
trademarks of Nintendo / Creatures Inc. / GAME FREAK inc.

Region map images are used under fair use for educational and
fan appreciation purposes. No copyright infringement is intended.
If you are a rights holder and have concerns, please open an issue
and content will be removed promptly.

---

## 🤝 Contributing

This repo is auto-maintained via GitHub Actions.
Manual additions (abilities, moves, items JSONs) follow the same
versioned structure under \`data/v{N}/\`.
```

Y el `LICENSE` file (MIT):
```
MIT License

Copyright (c) 2025 [Tu nombre]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
