# Crypto Pulse

Crypto Pulse is a responsive, single-page cryptocurrency price dashboard built with HTML, CSS, and vanilla JavaScript. It displays live BTC-USD and ETH-USD spot prices from the Coinbase API, refreshes them every five seconds, and indicates whether each price moved up or down since the previous update. Each card also draws a canvas line chart of up to the latest 20 successful price readings.

## Run it

Open `index.html` in a modern browser. The app needs an internet connection to retrieve prices from Coinbase. If your browser blocks requests from local files, serve the folder with any static HTTP server and open the resulting local URL.

## Data and behavior

- Prices are fetched from `https://api.coinbase.com/v2/prices/{SYMBOL}-USD/spot`.
- The dashboard polls BTC and ETH independently every five seconds.
- Each chart stores the latest 20 successful readings for that asset.
- A failed request leaves the last good price visible and displays an error message.
- No dependencies, build step, API key, or backend are required.

## Built for

Built with GitHub Copilot for **MLH Global Hack Week: Hacktoberfest**.
