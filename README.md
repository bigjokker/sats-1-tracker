# Bitcoin Stats Widget

A sleek, real-time Bitcoin statistics widget built with HTML, CSS, and JavaScript. Displays key BTC metrics like price, sats per USD, market cap, dominance, and more, with interactive features and a responsive design. Updated every 60 seconds using CoinGecko and Mempool APIs.

## Features

- **Real-Time Stats**:
  - Sats per $1 (current and all-time low, pulsing animation).
  - BTC Price (current and all-time high, pulsing animation).
  - Price Changes (24h, 6m, 1y percentages, color-coded green/red).
  - Block Info (current block, hash rate, halving estimate).
  - BTC Dominance & Fear/Greed Index (with spinning ₿ logos).
  - Market Cap, 24h Volume, and Circulating Supply.

- **Interactive Elements**:
  - Clickable stat boxes: Link to converters, external sites (e.g., CoinMarketCap, Mempool, Wikipedia), or internal pages (e.g., detailed price changes, Bitcoin White Paper).
  - Theme Toggle: Dark/light mode switch (bottom-left Moon/Sun icon), saved in local storage.
  - Help Button: Bottom-right question mark opens help page with explanations.

- **Animations & Effects**:
  - Pulsing on key values (Sats per $1, BTC Price).
  - Fade-in on data updates.
  - Spinning ₿ logos in Dominance box.
  - Hover lift and glow on the widget.

- **Connected Pages**:
  - Sats Converter: USD/Sats/BTC calculator.
  - Price Change: Detailed % changes over multiple timeframes (24h to all-time, with Future Change as ∞%).
  - Help Page: Feature summaries and explanations.

- **Responsive Design**: Optimized for mobile and desktop; adjusts layout on smaller screens.
- **Data Sources**: CoinGecko (prices/market data), Mempool (blocks/hash rate), Alternative.me (Fear & Greed).
- **No External Dependencies**: Pure vanilla JS/CSS; fonts from Google Fonts.

## Setup and Installation

1. **Clone the Repository**:
   ```
   git clone https://github.com/bigjokker/sats-1-tracker.git
   cd sats-1-tracker
   ```

2. **API Key (Optional)**:
   - The code uses a CoinGecko API key (set to empty by default). For higher rate limits, get a free key from [CoinGecko API](https://www.coingecko.com/en/api) and replace `const apiKey = '';` in the script.

3. **Assets**:
   - Ensure images like `Moon.png`, `Sun.png`, `help.png`, and `Sats-tracker.png` are in the root directory.
   - Add `apple-touch-icon.png` for iOS home screen icon.

4. **Local Viewing**:
   - Open `index.html` in a browser.

## Usage

- Open the widget in a browser (or via GitHub Pages: [https://bigjokker.github.io/sats-1-tracker/](https://bigjokker.github.io/sats-1-tracker/)).
- Stats auto-update every 60 seconds.
- Click stats for more details/links.
- Toggle theme with the bottom-left icon.
- Access help via bottom-right icon.

For mobile: Add to home screen for app-like experience (uses `apple-touch-icon.png`).

## Data and APIs

- **CoinGecko**: Prices, market cap, dominance, historical data.
- **Mempool**: Block height, hash rate.
- **Alternative.me**: Fear & Greed Index.
- Updates handle errors gracefully (shows "Error" if fetch fails).

Note: All-time low Sats per $1 is calculated from CoinGecko's ATH price for global consistency.

## Contributing

Contributions welcome! Fork the repo, make changes, and submit a pull request. Focus areas:
- Bug fixes (e.g., API handling).
- New stats or animations.
- Improved mobile responsiveness.

## License

MIT License. See [LICENSE](LICENSE) for details.

---

Built by bigjokker. #Bitcoin #StackingSats
