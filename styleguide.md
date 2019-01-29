# LACMIP Documentation Style Guide

Please refer to and update this style guide to help maintain consistency in our internal documentation.
For more information about theme formatting options, see the Minimal Mistakes documentation on [utility classes](https://mmistakes.github.io/minimal-mistakes/docs/utility-classes/) and [helpers](https://mmistakes.github.io/minimal-mistakes/docs/helpers/).

## Including media in documentation pages

To include a basic image with a caption, do so e.g.:
```
{% include figure image_path="/assets/images/lacmip-logo.jpg" alt="alt text goes here" caption="Figure caption text goes here." %}
```

To include a basic image without a caption, do so e.g.:
```
<img src="{{ site.baseurl }}/assets/images/access_login.png" alt="" width="100"/>{: .align-right}
```

To include a video, do so e.g.:
```
{% include video id="XsxDH4HcOWA" provider="youtube" %}
```

## Formatting conventions

Top-level headings within documentation pages should use `##` and be sentence case.

Use *italics* for filenames and for names of columns/fields, e.g. *IPProject*.

`"..."` for values of columns/fields, e.g. "FIC".

Use *italics* and carrots for file paths as well as navigation paths, e.g. *Dropbox > EMu > Data Migration Archive* or *Tools > Reports > Report all*.

Use **bold** for emphasis, e.g. "After making an edit, **remember to commit**".

Format code snippets with \`...\`, e.g. `bundle exec jekyll serve`.

File extensions written as part of a filename are lowercase, e.g. *example.jpg*, but when written alone are uppercase, e.g. "the file should be a JPG."

Highlight important information using classes, e.g.
```
whatever text I want to write
{: .notice--warning}`.
```
Adding `{: .notice--warning}` on a new line after your text block will highlight it in a box with a light yellow background.

## Page-level options

There are several things you may wish to control at the page level by overwriting site defaults. These include...
- remove the right-hand table of contents by including `toc: false` to the yml header of the page

## Naming files

Markdown files being added to the *_documentation* collection should be named descriptively yet succinctly. Do not use any character other than a-z.

Image files should be named descriptively. Recommendation is to name them according to the page they are being linked to, e.g. *labels_designs.jpg* is linked to the labels page.
