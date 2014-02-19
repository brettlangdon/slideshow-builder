Slideshow Builder
=================

Nothing crazy, just a Makefile which compiles a [remark.js](http://remarkjs.com/)
presentation from a template html file and a directory of markdown slides.

## Usage

### Clone from github
```bash
git clone git://github.com/brettlangdon/slideshow-builder
cd ./slideshow-builder
```

### Write your slides
Create a new file for each individual slide in the `slides`
directory. Make sure they are in the order you wish them to
be in the slideshow. E.g. `1_title.md`, `2_about_me.md`, etc.

Please refer to Remark's [documentation](https://github.com/gnab/remark/wiki)
for information on formatting slides.


### Edit Template, Optional
Edit the `template.html` file to suit your needs.

The slides contents will be replaced with `{{slides}}` in
the template file.

### Build Slideshow
Just run `make` from the root directory

Everything will get put into the `build` directory.

### Viewing slideshow
Either copy `./build/index.html` to a web server or open in a browser,
or you can run `make run` to run `python -m SimpleHTTPServer` from
within the `./build` directory.

## License

Do whatever you want. This is just a Makefile
