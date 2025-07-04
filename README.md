# Sefaria Extension for Raycast

A Raycast extension that provides access to [Sefaria.org](https://www.sefaria.org/), the free digital library of Jewish texts.

## Features

### 🔍 Search Sefaria

- Search for texts, commentaries, and sources across the entire Sefaria library
- Returns top 20 results with Hebrew text and metadata
- Supports searching for:
  - Biblical texts
  - Talmudic sources
  - Commentaries (Rashi, Ramban, etc.)
  - Any text in the Sefaria library

### 📖 Get Source

- Retrieve specific sources by reference
- Shows both Hebrew and English text side by side
- Supports various reference formats:
  - `Exodus 17:15` or `Exod. 17:15`
  - `Shemot 17:15` (Hebrew book names)
  - `Berakhot 14b` (Talmudic references)
  - `Rashi on Genesis 1:1` (Commentary references)

## Usage

1. **Search Sefaria**: Use the search command to find texts by keyword or topic
2. **Get Source**: Use the get source command to retrieve specific text passages

## Installation

1. Install the extension from the Raycast Store
2. Use the commands `Search Sefaria` or `Get Source` from Raycast

## Development

```bash
# Install dependencies
pnpm install

# Start development server
pnpm run dev

# Build extension
pnpm run build

# Lint code
pnpm run lint

# Auto-fix linting issues
pnpm run fix-lint
```

## API

This extension uses the [Sefaria API](https://developers.sefaria.org/):

- Search: `POST /api/search-wrapper`
- Texts: `GET /api/v3/texts/{reference}`

## License

MIT
