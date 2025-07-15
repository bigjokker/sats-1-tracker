Satoshi’s per $1 - Live Tracker

A sleek, real-time Bitcoin stats widget built with HTML, CSS, and JavaScript. Displays Sats per $1, BTC price, market data, and more, updating live via APIs. Designed for mobile-first viewing and easy embedding or hosting on GitHub Pages.
Features

    Live Updates: Fetches data every 60 seconds (configurable) from CoinGecko, Mempool.space, and Alternative.me APIs.
    Key Stats:
        Sats per $1 (with all-time low).
        BTC Price (with all-time high).
        Price Changes (24h, 6m, 1y).
        Current Block, Hash Rate, and Halving Estimate.
        BTC Dominance and Fear & Greed Index.
        Market Cap, 24h Volume, and Circulating Supply.
    Visuals: Dark mode theme with Bitcoin orange accents, pulsing animations, and a subtle glow effect on hover.
    Responsive: Optimized for mobile (max-width 400px) but scales well on desktop.
    Custom Elements: Spinning Bitcoin logos in the Dominance box for flair.
    No Dependencies: Pure vanilla JS; no frameworks needed.

Demo

View a live demo here https://bigjokker.github.io/sats-1-tracker/

Installation & Usage

    Clone the Repo
    
    git clone https://github.com/bigjokker/sats-1-tracker.git
    cd sats-1-tracker
    Customize:
        Open index.html in a text editor (e.g., Notepad++).
        Add your CoinGecko API key (free tier available) to const apiKey = ''; in the <script> section to avoid rate limits.
        Update meta tags (e.g., og:image, og:url) with your repo details.
    Test Locally:
        Open index.html in a browser.
        Data should load automatically (internet required).
    Deploy to GitHub Pages:
        Push to your repo's main branch.
        Go to repo Settings > Pages > Set source to main branch and root folder.
        Access at https://yourusername.github.io/sats-1-tracker/.
    Embed Elsewhere:
        Copy the HTML code and paste into your site, or use an iframe: <iframe src="https://yourusername.github.io/sats-1-tracker/" width="400" height="600"></iframe>.

APIs Used

    CoinGecko: For BTC price, market data, dominance.
    Mempool.space: For block height and hash rate.
    Alternative.me: For Fear & Greed Index.

Note: Free APIs may have rate limits. Sign up for a CoinGecko API key for better reliability.
Configuration

    Update Interval: Change setInterval(updateSats, 30000); to a higher value (e.g., 60000 for 1 minute) to reduce API calls.
    Styles: Tweak CSS in the <style> block (e.g., colors, fonts, grid columns).
    All-Time Low Persistence: Uses localStorage to track the lowest Sats per $1 seen.

Contributing

Fork the repo, make changes, and submit a pull request. Suggestions for new stats or improvements welcome!
License

MIT License - Feel free to use, modify, and distribute. See LICENSE for details.
