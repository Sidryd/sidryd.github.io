# Adjust a ggplot theme

The library `ggplot2` in `R` is such a good package. However, creating a nicely formatted graph with the right title adjustment and so on often results in many rows of code. Especially code that is repeated through out a project. Luckliy the there is a solution which helps you tidy up your code, make it more consistent, and easily adjust the properties for all graphs. The package comes with a function for setting a default theme, `theme_set()`, and a function for updating the associated elements, `theme_update()`. 

```r
library(ggplot2)
theme_set(theme_bw())
theme_update(plot.title = element_text(hjust = 0.5, size = 14, face = "bold"),
             plot.subtitle = element_text(hjust = 0.5, size = 12),
             legend.title = element_text(face = "bold"))
```
