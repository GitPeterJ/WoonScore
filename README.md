# WoonScore

A geospatial livability scoring system for the Netherlands using H3 hexagons. Calculates location quality scores based on mobility, amenities, and air quality to optimize house hunting decisions.

## Project Structure

```
WoonScore/
├── notebooks/          # Jupyter notebooks for analysis and exploration
│   └── 01_setup.ipynb  # Setup verification notebook
├── src/                # Python source code modules
│   └── __init__.py     # Package initialization
├── data/               # Data files (gitignored)
├── pyproject.toml      # Project configuration and dependencies
├── uv.lock             # Locked dependency versions
└── README.md           # This file
```

## Prerequisites

- Python 3.12 or higher
- [uv](https://github.com/astral-sh/uv) - Fast Python package installer and resolver

## Installation

1. Install uv if you haven't already:
   ```bash
   pip install uv
   ```

2. Clone the repository:
   ```bash
   git clone https://github.com/GitPeterJ/WoonScore.git
   cd WoonScore
   ```

3. Install dependencies:
   ```bash
   uv sync
   ```

## Usage

### Running Python Scripts

Use `uv run` to execute Python scripts with the project dependencies:

```bash
uv run python your_script.py
```

### Running Jupyter Notebooks

Start Jupyter Lab:

```bash
uv run jupyter lab
```

Or Jupyter Notebook:

```bash
uv run jupyter notebook
```

Then open `notebooks/01_setup.ipynb` to verify the installation.

### Activating the Virtual Environment

To activate the virtual environment manually:

```bash
source .venv/bin/activate  # On Linux/Mac
# or
.venv\Scripts\activate     # On Windows
```

## Core Dependencies

- **h3** (>=4.0.0) - Hexagonal hierarchical geospatial indexing system
- **geopandas** (>=1.0.0) - Geospatial data manipulation and analysis
- **osmnx** (>=2.0.0) - OpenStreetMap network analysis
- **pyrosm** (>=0.6.0) - Fast OSM data parser
- **shapely** (>=2.0.0) - Geometric operations
- **jupyter** (>=1.0.0) - Interactive notebooks

## Development

The project uses modern Python practices with uv for dependency management. All dependencies are locked in `uv.lock` for reproducibility.

## License

To be determined
