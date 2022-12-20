# Newfoundland Turnip Strips Archive

Archive of The Newfoundland Turnip's strips of webcomics.

All archived strips are located in the `strips` folder.

## Generating

To generate information and generate a single strip from combining the images.

### Usage

1. Create a "slug" folder based on a title into the `strips` folder, example: `strips/slush-run`
2. Download all strips of the webcomic to the newly-created folder
3. Run `bin/strip [slug] "[title]" [date] [width]x`, example: `bin/strip slush-run "Slush run" 2022-11-23 1200x`

This will:

* Rename all strips to index-based, example: `FB_282898929882892892.jpeg` into `1.jpg`, `2.jpg`, etc
* Create a `info.json` file containing information about the webcomic: slug, title, date, and strip count
* Creates a combined strip image `combined.jpg` containing all images stacked into one, to the width provided

### Site

The `static` folder is a temporary static site which takes all strips and creates a website from them.

Running `bin/site` will generate the website, Github serves the website.

#### Viewing locally

`cd static/ && python3 -m http.server 8080`

Then, open `http://localhost:8080` to view.

## License

This project is released under the MIT [license](https://github.com/gnikyt/turnipstrips/blob/master/LICENSE).

Strips are owned and sourced from The Newfoundland Turnip's Facebook page.
