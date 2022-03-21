My code for the meme:
"""library(magick)
redpanda <- image_read("https://cdn.pastemagazine.com/www/articles/2021/07/13/turning-red-pixar-main.jpg") %>% 
  image_crop(geometry = "578x381+150")
blank <- image_annotate(image_blank(528, 50, color = "Black"), text = "WAKING UP ON MONDAY BE LIKE:", color ="#FFFFFF", size = 25, font = "Impact", gravity = "south")
final <- image_append(c(blank, redpanda), stack = TRUE)
image_write(final,"my_meme.png")"""
