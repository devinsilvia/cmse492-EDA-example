# DC Comics — Exploratory Data Analysis

A minimal data science project that explores the
[DC Comics Wikia character dataset](https://github.com/ghoshpoulami1293/ComicBookUniverse)
as an example of an AI-assisted EDA workflow.

The analysis covers:
* Data loading and cleaning
* Summary statistics and value-count breakdowns
* Visualisations: alignment, gender, debut decade, appearance distributions, and more

---

## Project structure

```
.
├── data/               # Raw CSV goes here (see data/README.md)
├── notebooks/
│   └── dc_comics_eda.ipynb   # Main exploratory notebook
├── pyproject.toml      # Python environment (managed with uv)
└── README.md
```

---

## Quick-start

### 1 — Install [uv](https://docs.astral.sh/uv/)

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

### 2 — Create the virtual environment and install dependencies

```bash
uv sync
```

### 3 — Download the dataset

```bash
curl -L "https://raw.githubusercontent.com/ghoshpoulami1293/ComicBookUniverse/main/data/dc-wikia-data.csv" \
     -o data/dc-wikia-data.csv
```

### 4 — Launch Jupyter and open the notebook

```bash
uv run jupyter notebook notebooks/dc_comics_eda.ipynb
```

---

## Dependencies

| Package | Purpose |
|---|---|
| `pandas` | Data loading, cleaning, and aggregation |
| `numpy` | Numerical helpers |
| `matplotlib` | Low-level plotting |
| `seaborn` | Statistical visualisations |
| `jupyter` / `notebook` | Interactive notebook environment |

All dependencies are declared in `pyproject.toml` and pinned via `uv.lock`
(generated on first `uv sync`).

---

## Dataset

**Source**: FiveThirtyEight Comic Characters Dataset, republished in  
<https://github.com/ghoshpoulami1293/ComicBookUniverse>

**File used**: `dc-wikia-data.csv` (~6 700 DC Comics characters)

Key columns: `name`, `ALIGN`, `EYE`, `HAIR`, `SEX`, `GSM`, `ALIVE`,
`APPEARANCES`, `YEAR`
