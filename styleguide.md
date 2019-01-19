# LACMIP Documentation Style Guide

Please refer to and update this style guide to help maintain consistency in our internal documentation.
For more information about theme formatting options, see the Minimal Mistakes documentation on [utility classes](https://mmistakes.github.io/minimal-mistakes/docs/utility-classes/) and [helpers](https://mmistakes.github.io/minimal-mistakes/docs/helpers/).

## Page-level options

There are several things you may wish to control at the page level by overwriting site defaults. These include...
- remove the right-hand table of contents by including `toc: false` to the yml header of the page

## Including media in documentation pages

To include a basic image with a caption, do so e.g.:
```
{% include figure image_path="/assets/images/lacmip-logo.jpg" alt="alt text goes here" caption="Figure caption text goes here." %}
```

To include a basic image without a caption, do so e.g.:
```
![image-right]({{ site.baseurl }}/assets/images/tray1.jpg){: .align-right}
```

To include a video, do so e.g.:
```
{% include video id="XsxDH4HcOWA" provider="youtube" %}
```

## Formatting conventions

Top-level headings within documentation pages should use `##` and be sentence case.

Use *italics* for filenames and for names of columns/fields, e.g. *IPProject*.

`"..."` for values of columns/fields, e.g. "FIC".

Use **bold** for emphasis, e.g. "After making an edit, **remember to commit**".

Format code snippets with \`...\`, e.g. `bundle exec jekyll serve`.

File extensions written as part of a filename are lowercase, e.g. *example.jpg*, but when written alone are uppercase, e.g. "the file should be a JPG."
