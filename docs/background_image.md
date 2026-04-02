
---


# Background Image

ReyPlot allows you to place an image behind your plot, adding visual context or artistic flair. The image is stretched to fill the entire canvas and is applied to **both the inner and outer layers** (with the outer layer automatically masking the inner area).

## Basic Usage

```python
import reyplot as rp

fig = rp.chart()
fig.background_image(path="image.jpg", blur=7)
fig.scatter(data=df,x="sepal_width", y="sepal_length" , color= "maroon")
rlt.chart(size=[600,480])

fig.show()


```
![Trigonometric functions plot](images/plot.jpg)

## blur
The blur parameter accepts float values.
The default value of ```blur``` is ```0```

The image is loaded using Pillow and scaled to match the chart’s dimensions. The ```blur``` parameter applies a Gaussian blur to the image, creating a soft background effect.

