# Quick Start

Get started with ReyPlot in just a few lines of code. This guide shows you how to create basic scatter plots using both raw numerical data and built‑in datasets. The examples demonstrate that ReyPlot supports both raw numerical data and structured datasets, combining the flexibility of Matplotlib with the simplicity of Seaborn.

---

## 1. Create a Simple Scatter Plot with NumPy

This example loads the Iris dataset and creates a scatter plot of sepal width vs. sepal length. The points are colored according to the sepal length value, creating a gradient from blue to red. 

```python
import reyplot.plot as rlt 

df = rlt.load_dataset("iris")

rlt.chart(size=[600,480])

rlt.scatter(data = df,
           x = "sepal_width",
           y = "sepal_length",
           color_by = "sepal_length",
           color_range = ("blue","red")
           )
rlt.title("Iris Data")
rlt.show()



``` 
![Trigonometric functions plot](images/blue and red plot.png)



!!! tip
To save the figure instead of displaying it, replace ```rlt.show()``` with:

```rlt.save("iris_scatter_plot.png")```
You can also specify ```filetype="jpg" ```.