---
title: A blog, I guess
---

# Updating the default color scheme in ggplot2

When building a project, it is a nice feature to display standardized graphs as well as intriguing graphs. Working with the default palette solves the first issue, but seldom the second issue. By defining a palette for each graph, a lot of repetitive code is introduced as well as the factor of not being consistent, for the gain of more intriguing graphs. A trade-off situation as often within the field. Another approach is to override the default palettes within the `ggplot2` package using the, in my opinion, more intriguing [Viridis](https://github.com/sjmgarnier/viridis) palette. 

```r
library(ggplot2)
options(ggplot2.continuous.colour = scale_color_viridis_c, 
            ggplot2.continuous.fill = scale_fill_viridis_c,
            ggplot2.discrete.colour = scale_color_viridis_d,
            ggplot2.discrete.fill = scale_fill_viridis_d)
```

Do you miss the default settings? I got you covered. 

```r
options(ggplot2.continuous.colour = scale_colour_gradient, 
            ggplot2.continuous.fill = scale_fill_gradient,
            ggplot2.discrete.colour = scale_color_hue,
            ggplot2.discrete.fill = scale_fill_hue)
```
