# **API Reference**

A complete reference for all public classes, functions, and methods in ReyPlot.

---

## `chart` Class

The `chart` class is the main figure object. You instantiate it with `rp.chart()` (object‑oriented style) or use the global interface `reyplot.plot` (functional style). All methods described below work identically in both styles.

### Methods

| Method | Description | 
|--------|-------------|
| `chart(size=[600,480], scale=1)` | Create a new figure. |
| `scatter(...)` | Add a scatter plot. See [Scatter](scatter.md) for parameters. |
| `inner_layer(color="#EEEEEE", gradient=False, gradient_color="#000000", alpha=1)` | Set inner background. |
| `outer_layer(color="#EEEEEE", gradient=False, gradient_color="#000000", alpha=1)` | Set outer background. |
| `background_image(path=None, blur=0)` | Set background image. |
| `block_grid(color="#D1D1D1", gradient=True, gradient_color="#000000", alpha=0.4, radius=1, display=True)` | Add block grid. |
| `axes(color="black", style="two_lines", alpha=1, x_tic=4, y_tic=4, sig_digits=3)` | Configure axes. |
| `title(title, color="black", alpha=1, font="Sans")` | Set main title. |
| `x_title(x_title=None, color="black", alpha=1, font="Sans")` | Set x‑axis label. |
| `y_title(y_title=None, color="black", alpha=1, font="Sans")` | Set y‑axis label. |
| `x_lim(limits)` | Set x‑axis limits. |
| `y_lim(limits)` | Set y‑axis limits. |
| `legend(display=True, location="top_right", text_color="black", stroke=True, stroke_color=None, shadow=False)` | Configure legend. |
| `auto_legend(style="formal")` | Enable auto‑legend for color/size mappings. |
| `save(name="reyplot", filetype="png")` | Save to file. |
| `show()` | Display in a window. |

## `load_dataset`

```python
load_dataset(name, engine="polars")
```
