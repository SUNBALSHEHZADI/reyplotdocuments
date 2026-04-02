# **Axes**

ReyPlot provides automatic axis limits and ticks using the Wilkinson algorithm. You can customize appearance and style.

## Basic Axes

By default, axes are drawn as a two‑line L‑shape. To change style, use `fig.axes()`:

```python
fig.axes(color="black", style="boxed", alpha=1, x_tic=4, y_tic=4, sig_digits=3)
```
