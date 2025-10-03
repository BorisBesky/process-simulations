# Process Simulations

Interactive visualizations of distributed algorithms and process synchronization. This repository contains small HTML apps that demonstrate core concepts like distributed snapshots (Chandy–Lamport) and consensus (Raft).

## What you'll find here

- `index.html` — Landing page and index linking to the simulations. A responsive, modern UI to pick a simulation.
- `Chandy-Lambert-Simulation.html` — Interactive Chandy–Lamport global snapshot visualization.
- `Raft-Protocol-Simulation.html` — Interactive Raft consensus protocol visualization.

## How to preview

There are two simple ways to preview the simulations locally on macOS:

1) Open directly (quick):

- Double-click any `*.html` file in Finder to open in your default browser.
- Or from the terminal:

```bash
open index.html
```

This method opens files via the `file://` protocol. Some advanced features that use fetch/XHR or modules may be blocked by the browser when loaded this way.

2) Serve with a lightweight HTTP server (recommended):

This avoids file:// restrictions and is the recommended way to preview the simulations.

Python 3 (no install required on most macOS machines):

```bash
# run from repository root
python3 -m http.server 8000 --directory $(pwd)
# then open http://localhost:8000/index.html
```

Node (if you prefer npm):

```bash
# If you have npm, you can install a static server once:
npm install -g serve
# run it from the repo root
serve -l 8000 .
# then open http://localhost:8000/index.html
```

## Notes

- The HTML files are self-contained and meant for learning and demos.

## License

This project is licensed under the MIT License — see the [LICENSE](./LICENSE) file for details.
