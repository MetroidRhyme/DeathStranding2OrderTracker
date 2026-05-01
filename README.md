# Death Stranding 2 Order Tracker

A single-file browser app for tracking delivery orders in *Death Stranding 2: On the Beach*. No installation, no server — just open the HTML file.

## Features

- **Locations & Nodes** — Organize deliveries by major region and individual node. Drag to reorder.
- **Order tracking** — Log orders with cargo type, source/destination, package count, weight, and modifiers (Fragile, Explosive, Rush, etc.).
- **Delivery runs** — Record each run's grade (D–S) and completion time. Best run is highlighted automatically.
- **Node ratings** — Rate each node with a half-star system (0–5 stars).
- **Grade summaries** — At-a-glance S/A/B/C/D counts per node and per major location.
- **Persistent storage** — All data is saved to `localStorage`; nothing leaves your browser.

## Usage

1. Download `DS2OrderTracker.html`.
2. Open it in any modern browser — no internet connection required after the initial load.
3. Use **+ LOCATION** to add major regions, then **+ NODE** inside each location to add individual nodes.
4. Use **+ ADD ORDER** to create orders between nodes.
5. Use **LOG RUN** to record a delivery result for any order.

## Data

All data is stored in your browser's `localStorage` under the key `ds2ot_v3`. To back up or transfer your data, open the browser console and run:

```js
copy(localStorage.getItem('ds2ot_v3'))
```

Then paste the result into a text file. To restore, paste it back:

```js
localStorage.setItem('ds2ot_v3', '<paste here>')
```
