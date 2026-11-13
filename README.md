# How transformers read

An interactive, 12-slide presentation about the transformer architecture, from attention intuition to the scaled dot-product computation, multi-head attention, the transformer block, model families, the cost of attention and sampling.

Everything runs in the browser from a single `index.html`: no build step, no server, no dependencies to install. The only external request is for Google Fonts, with system-font fallbacks.

## View locally

Open `index.html` in any modern browser.

## Navigate

- Arrow keys, Page Up / Page Down, or the Back and Next buttons
- Click a segment of the progress bar to jump to a slide
- Every slide has its own link, such as `#s6` for the attention walkthrough

## Deploy on Render

**Option A, with the included Blueprint:** in the Render dashboard choose **New → Blueprint**, select this repository and click **Apply**. Render reads `render.yaml` and creates the static site.

**Option B, by hand:** choose **New → Static Site**, select this repository, leave the build command empty and set the publish directory to `.`.

Either way the site goes live at `https://<name>.onrender.com`, and every push to `main` redeploys it automatically.

## Other hosts

Because it is a single static file, it also works on GitHub Pages, Netlify, Vercel and Cloudflare Pages without changes.

## Note on content

The attention patterns on slides 1 and 7 are hand-built illustrations, and the tokenizer and embedding values on slide 3 are toys. The matrix arithmetic on slide 6 and the cost figures on slide 10 are computed from real numbers.
