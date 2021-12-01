# usafhforum

```R
class %>%
  mutate(class = factor(class, levels=c("Freshman","Sophomore","Junior","Senior"))) %>%
  ggplot(aes(x = save_percent, y = class, fill = class)) + 
  stat_density_ridges(quantile_lines = TRUE, quantiles = 2, rel_min_height = 0.01) + 
  theme(legend.position = "none") + xlab("Save %") + 
  theme(panel.background = element_rect(fill = "#F7F7F7", colour = "#F7F7F7"), panel.border = element_blank(), panel.grid.major = element_line(colour = "#DEDEDE"), panel.grid.minor = element_blank()) + 
  theme(plot.background = element_rect(fill = "#F7F7F7")) + theme(text = element_text(family = ".SF Compact Rounded")) + 
  ylab("") + theme(axis.text=element_text(size=12), axis.title=element_text(size=14))
```
