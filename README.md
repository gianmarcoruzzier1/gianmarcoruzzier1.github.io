# Personal Website Notes

## Structure

```
webpage_gian/
├── index.html        -- entire site (single page)
├── css/
│   └── style.css     -- all styles
├── assets/
│   ├── img/
│   │   └── photo.jpg -- your profile photo
│   └── pdf/
│       └── cv.pdf    -- your CV
└── README.md         -- this file
```

## How to update

### Change text content
Edit `index.html` directly. Each section is wrapped in a `<section id="...">` tag.

### Update the CV
Replace `assets/pdf/cv.pdf` with a new file of the same name.

### Add a profile photo
Drop `photo.jpg` into `assets/img/`. Then add an `<img>` tag in `index.html`:
```html
<img src="assets/img/photo.jpg" alt="Gianmarco Ruzzier" width="200" />
```

### Change styling
Edit `css/style.css`. The stylesheet is plain CSS — no build step needed.

### Add a research paper link
In the `#research` section of `index.html`, add a list item:
```html
<li><a href="assets/pdf/paper.pdf">Paper Title (Year)</a></li>
```

## Deployment
Upload the entire `webpage_gian/` folder to your web host, or push to GitHub Pages.
For GitHub Pages: repository must be named `<username>.github.io` and `index.html` must be in the root.
