# Assignment summary
#### R code for my meme

```R
library(magick)

derp_face <- image_read("https://www.kindpng.com/picc/m/691-6919280_derp-face-png-clipart-transparent-png.png")
blank <- image_blank(860, 100, color = "black") %>% 
    image_annotate("Me when I try to make memes:", size = 50, gravity = "south", color = "white")

final <- c(blank, derp_face)

final <- image_append(final, stack = TRUE)

image_write(final, "my_meme.png")
```

![This is my meme](https://raw.githubusercontent.com/Holy-mizu/stats220/main/my_meme.png)
--------------------------

#### Why this meme

The reason why I came up with this meme is becasue I don't spend time browsing through memes, and I am very ***bad*** at making memes.
This meme is **original** because the _fact_ I cannot make any memes inspired me to make the meme, and I've assembled everything thing using R code from above.
