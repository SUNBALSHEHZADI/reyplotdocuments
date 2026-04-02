# **Introduction**

ReyPlot is designed for scientists, data analysts, and developers who need quick, attractive plots without heavy boilerplate.

## **Key Concepts**

### **Chart Object**
Everything starts with `rp.chart()`, which creates the figure canvas. You configure its size and scale.

### **Layers**
ReyPlot uses a **layer‑based rendering** system. Layers are drawn in a fixed order:
1. Inner Layer (background)
2. Background Image (if any)
3. Block Grid
4. Outer Layer (background with cutout)
5. Scatter Points
6. Axes
7. Titles
8. Legend

You can customize each layer with colors, gradients, and transparency.

### **Data Handling**
ReyPlot automatically converts many common data types to Polars DataFrames:
- Polars DataFrame
- Pandas DataFrame
- NumPy arrays
- PyArrow Table
- List of dicts
- Dict of lists
- List of lists

If you provide raw lists for `x` and `y`, you can omit the `data` argument.

### **Styling**
- **Color** – accepts hex codes or color names (e.g., `"teal"`, `"#800000"`). 
A built‑in color cycler rotates through: maroon → teal → blue → black → gray → green → cyan → orange → yellow → purple.
- **Gradients** – available for layers and block grid.
- **Glow & Shadow** – add visual depth to scatter points.
- **Dot Shapes** – circle, square, triangle, hexagon, diamond (and variants `c`, `t`, `c1`).
- **Size & Color Mapping** – encode additional dimensions by mapping data columns to point size or color.

## **Rendering**
Plots can be saved as PNG, JPG, or SVG, and displayed in a Tkinter window with `fig.show()`.

## Next Steps
- [Quick Start](quick_start.md) to get started.
- [Scatter](scatter.md) for detailed scatter plot options.
