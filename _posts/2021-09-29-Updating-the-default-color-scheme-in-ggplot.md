
# Updating the default color scheme in ggplot

Viridis

```r
library(ggplot2)
options(ggplot2.continuous.colour = scale_color_viridis_c, 
            ggplot2.continuous.fill = scale_fill_viridis_c,
            ggplot2.discrete.colour = scale_color_viridis_d,
            ggplot2.discrete.fill = scale_fill_viridis_d)
```

Do you miss the default settings? 

```r
options(ggplot2.continuous.colour = scale_colour_gradient, 
            ggplot2.continuous.fill = scale_fill_gradient,
            ggplot2.discrete.colour = scale_color_hue,
            ggplot2.discrete.fill = scale_fill_hue)
```
