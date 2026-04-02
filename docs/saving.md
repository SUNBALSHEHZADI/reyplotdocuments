
# **Saving Plots**

ReyPlot can export plots to PNG, JPG, or SVG.The filetype parameter accepts a string and specifies the output image format.
ReyPlot supports the following formats:

```
"svg"
"png"
"jpg"
``` 

Default value: `"png"`

## Save to File

```python
fig.save("filename", filetype="png")
```

