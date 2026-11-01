# Maryam Saberi: personal research site

A single-page site (plain HTML and CSS, no build step) hosted free on GitHub Pages.

## What's here

| File | What it is |
| --- | --- |
| `index.html` | The whole site: text, styles and scripts (the dark "Point Cloud" design) |
| `media/` | The three research-card images (abstract illustrations, tinted teal by the page; swap in your own figures) |
| `photo.jpg` | Your headshot (square, 640×640). Replace it with a file of the same name to change it |
| `Maryam_Saberi_CV.pdf` | Your CV. The "download_cv.pdf" and "cv.pdf" buttons link to this exact filename, so keep the name when you replace it |

## Put it online (first time)

1. Sign in to [github.com](https://github.com) (or create a free account).
2. Click **+** (top right) → **New repository**.
   - Name it exactly **`mrymsaberi.github.io`** (your username plus `.github.io`).
   - Set it to **Public** and click **Create repository**.
3. On the new repository page, click **uploading an existing file**.
4. Drag in `index.html`, the `media` folder, `photo.jpg` and `Maryam_Saberi_CV.pdf`, then click **Commit changes**.
5. Go to **Settings → Pages** and check that **Source** is "Deploy from a branch" with branch **main** and folder **/ (root)**.
6. After a minute or two, the site is live at **https://mrymsaberi.github.io**.

## Update it later

- **On github.com:** open `index.html` in the repository, click the pencil icon, edit, then **Commit changes**. The site updates within a minute or two.
- **To replace a file** (new CV, new photo): use **Add file → Upload files** with the same filename.

## Common edits in `index.html`

- **New paper:** copy one `<article class="pub" ...>` block in the Publications section. `data-kind` is `J` (journal), `C` (conference) or `R` (under review). Update the counts on the filter buttons and the "7 papers" number at the top.
- **Paper accepted:** change its `data-kind` from `R` to `J` or `C`, change `[R]<small>in review</small>` to `[J]<small>2027</small>` (or `[C]`, with the real year), and replace the empty `<span></span>` at the end with a DOI link: `<a class="go" href="https://doi.org/...">doi ↗</a>`.
- **Add Google Scholar or GitHub:** copy the LinkedIn button in the top section and change the link and label.
- **Use your own research figures:** put the image in `media/`, then change the matching `src="media/..."` in the Research section and delete `class="tint"` from that `<img>` (the tint recolors the placeholder illustrations and would recolor your figure too).

The `designs/` folder holds the other design options for comparison. It isn't part of the site, so you don't need to upload it.
