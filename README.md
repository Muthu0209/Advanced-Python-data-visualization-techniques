# Advanced-Python-data-visualization-techniques
Advanced data visualization techniques in Python using Seaborn and Plotly — including lmplots, joint plots, violin/strip/swarm plots, catplots, interactive Plotly charts (histogram, bar, scatter, 3D scatter), and plot customization — applied to an automobile dataset to explore relationships and distributions across variables. Practiced as part of the **Data Analytics Essentials** program (Great Learning / UT Austin McCombs).


## Dataset

**File:** `Automobile.csv`: 201 rows × 26 columns

| Type | Example columns |
|---|---|
| Categorical | `make`, `fuel_type`, `aspiration`, `number_of_doors`, `body_style`, `drive_wheels`, `engine_location`, `engine_type`, `fuel_system` |
| Numerical | `wheel_base`, `length`, `width`, `height`, `curb_weight`, `engine_size`, `bore`, `stroke`, `compression_ratio`, `horsepower`, `peak_rpm`, `city_mpg`, `highway_mpg`, `price` |

**Quick facts from the data overview**

- Car prices range from 5,118 to 45,400
- Curb weight ranges from 1,488 to 4,066
- Toyota is the most common make

## Techniques Covered

### Seaborn

| Plot | What it shows | Example in notebook |
|---|---|---|
| `lmplot` | Scatterplot with a fitted regression line; split by `hue` or `col` | curb weight vs. horsepower by fuel type |
| `jointplot` | Bivariate plot with marginal distributions (`scatter`, `hex`, `kde`, `reg`) | engine size vs. horsepower |
| `violinplot` | Distribution + density of a numeric variable across groups | horsepower by fuel type |
| `stripplot` | Categorical scatter with jitter, best for small datasets | engine size by body style |
| `swarmplot` | Non-overlapping points, so width shows the distribution | price by number of doors |
| `catplot` | Figure-level interface (point, bar, box, swarm) with faceting | horsepower by fuel type across drive wheels |

### Plotly (interactive)

- Histogram
- Bar plot
- Scatter plot
- Box plot with underlying data points
- 3D scatter plot (exportable to HTML)

### Plot Customization

- Axis limits (`plt.xlim`, `plt.ylim`)
- Titles and labels
- Grid styles (`darkgrid`, `whitegrid`, `white`)
- Color palettes (`deep`, `muted`, `pastel`, `bright`, `dark`, `colorblind`)
- Legend labels and position

## Tech Stack

- Python 3
- pandas, NumPy
- Matplotlib, Seaborn
- Plotly Express

## Getting Started

1. Clone the repo

```bash
git clone https://github.com/Muthu0209/Advanced-Python-data-visualization-techniques.git
cd Advanced-Python-data-visualization-techniques
```

2. Install the dependencies

```bash
pip install pandas numpy matplotlib seaborn plotly
```

3. Open the notebook in Jupyter or Google Colab

```bash
jupyter notebook
```

4. Make sure `Automobile.csv` is in the same folder as the notebook, and load it with:

```python
df = pd.read_csv('Automobile.csv')
```

## Repository Structure

```
├── Advanced Python data visualization techniques.ipynb
├── Automobile.csv
└── README.md
```

## Key Takeaways

- Choosing the right plot depends on the data: scatter-style plots for relationships, violin/strip/swarm for distributions across categories
- Hexbin and KDE jointplots handle overplotting better than plain scatterplots
- Swarm plots reveal distribution shape that strip plots can hide
- Plotly adds interactivity (hover, zoom, 3D rotation) that static plots lack

## Author

**Muthu**: Data Analyst | [GitHub](https://github.com/Muthu0209)
