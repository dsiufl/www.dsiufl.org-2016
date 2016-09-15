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

The timing duration is stored in the `_config.yaml` as the variable 
`carousel_interval`.

## Members on the About page

The members list on the About page is dynamically generated. The member 
information is kept in the `_members/` folder in Markdown files name in the 
`<lastname>_<firstname>.md` format. There is also a variable in the 
`_config.yml` that controls the semesters that are listed. Place the member's 
headshot in `img/members` folder in the `<lastname>_<firstname>.jpg` or 
`<lastname>_<firstname>.png` format, the suggested dimension is 432 x 432 px. 
Using photo of different dimensions would cause distortion in arrangement. 
To add a new member, copy an existing `member.md` file, rename it and fill 
corrseponding areas accordingly. Please pay special attention to `Major` category
because long name would cause distortion, too.

### At a new semester

1. Update the `semesters` variable in `_config.yaml` to add the new semester name
at the top. Use `<year> [Fall|Spring]` as the format of the semester name.
1. Add new Markdown files to `_members/` for new people. Copy an existing file
as a template.
1. For re-elected people, add a new position to their positions variable in
their existing file.

### Removing people

1. Delete their .md file from the `_members/` directory

## Workshops

### Adding a new workshop

Add a Markdown file to the _workshops directory. You can copy one of the 
existing files and edit it. Sort order is controlled by the sort variable, not
the file name. 

To make a line bold, use ** tag or <b>. 
To make a line in larger font, use "#" symbol before the line (without ""), "#" refers
to the largest font size while "####" refers the smallest but still larger than body font.
To add a link, use [`the notation of such link`] and put ('the link used') right after []
See `data_science_roadmap.md` for the link example. 

Here is a 
[cheetsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for emphasis, 
lists, links and so on.


## Gallery

Images should be placed in `img/gallery` and 1900x1263 px. For each image, a
Markdown file should be created in `_gallery/` with information about the
image. Copy and update one of the existing files. Keep the images and Markdown
files named the same to make it easier to match them up when maintaining the
site.

Images are sorted by the eventDate parameter with the newest first.

### Managing Google calendar 
dsiufl@gmail.com 
Any events with "Events" tag would be shown on the calendar section.

