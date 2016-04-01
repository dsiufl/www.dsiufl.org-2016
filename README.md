# How to manage content

## Updating front page carousel

### Images

The images used on the front page are dynamically sized and windowed to the 
aspect ratio on the front page. Using images that are at around 1200px wide
and 600px high probably will work well.

Place the images in `img/carousel/header[1|2|3].jpg to have them served. You
can safely rename existing files if you want to keep them around; only those
three file names will be used in that order.

### Duration

The timing duration is stored in the _config.yml as the variable 
`carousel_interval`.
