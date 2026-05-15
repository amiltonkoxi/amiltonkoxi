# Setup Guide · Dynamic Profile README

## Repository structure

Your repository `amiltonkoxi/amiltonkoxi` should look like this:

```
amiltonkoxi/
├── README.md
├── assets/
│   ├── banner.svg                 # animated header
│   ├── fmead-architecture.svg     # animated FMEAD diagram
│   ├── tech-stack.svg             # technical stack cards
│   └── divider.svg                # animated section divider
└── .github/
    └── workflows/
        └── snake.yml              # snake animation workflow
```

## Step by step

### 1. Place the files

```bash
# in your repo root
mkdir -p assets .github/workflows

# copy the assets you downloaded
mv banner.svg fmead-architecture.svg tech-stack.svg divider.svg assets/

# copy the workflow
mv snake.yml .github/workflows/

# place the README
mv README.md .
```

### 2. Push everything

```bash
git add .
git commit -m "feat: dynamic profile README with Tokyo Night design system"
git push origin main
```

### 3. Enable the snake animation workflow

1. Go to your repository on GitHub.
2. Click on the **Actions** tab.
3. You should see "Generate Snake Animation" listed.
4. Click on it and press **Run workflow** once manually.
5. After the first successful run, an `output` branch will be created automatically.
6. The snake SVG will be served from `https://raw.githubusercontent.com/amiltonkoxi/amiltonkoxi/output/github-contribution-grid-snake-dark.svg`.

From then on, it runs every 12 hours and updates the snake to reflect your latest contributions.

## What animates in your profile

| Element | What moves |
|---|---|
| Banner | Cursor blink after `$ whoami --verbose`, FPGA chip activity LED, pulsing dots, drifting glow, data packets flowing on circuit traces, inner chip outline pulse |
| FMEAD architecture | "LIVE" indicator pulse, sensor activity dots, AXI bus packet, sensor-to-FPGA data packets, FPGA-to-output data packets, ESP32 Wi-Fi ripple, MicroBlaze and Custom Logic stroke pulse, Anomaly Engine stroke pulse, FPGA-to-Browser packet |
| Divider | Center dot grows and shrinks, traveling pulse moves across |
| Typing tagline | Three rotating phrases below the banner |
| GitHub stats | Auto-update with your real commits, language usage, streaks |
| Activity graph | Continuous contribution timeline |
| Snake | Eats your contribution squares, regenerated every 12h |

## Things you may want to tweak

| What | Where |
|---|---|
| Portfolio URL | Replace `href="#"` in two places |
| Repository names | If you rename `FMEAD-FPGA`, search and replace |
| Stats card commit count | `count_private=true` is enabled; remove if you prefer only public |
| Typing tagline phrases | Edit `lines=` parameter in the typing SVG URL after the banner |

## Note on SVG animations

The banner, FMEAD architecture, and divider use SVG SMIL animations (`<animate>`, `<animateMotion>`). These are supported by GitHub's rendering. Some markdown previewers in local editors do not animate, which is normal. They animate live on github.com.
