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

The timing duration is stored in the `_config.yml` as the variable 
`carousel_interval`.

## Members on the About page

The members list on the About page is dynamically generated. The member 
information is kept in the `_members/` folder in Markdown files name in the 
`<lastname>_<firstname>.md` format. There is also a variable in the 
`_config.yaml` that controls the semesters that are listed.

### At a new semester

1. Update the `semesters` variable in `_config.yaml` to add the new semester name
at the top. Use `<year> [Fall|Spring]` as the format of the semester name.
1. Add new Markdown files to `_members/` for new people. Copy an existing file
as a template.
1. For re-elected people, add a new position to their positions variable in
their existing file.

### Removing people

1. Delete their .md file from the `_mmebers/` directory

