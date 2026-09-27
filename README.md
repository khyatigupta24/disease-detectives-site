# Disease Detectives — website

A single-page site for Disease Detectives, a youth-led public health education
program founded by Khyati Gupta. Built as one self-contained `index.html` —
no build step, no dependencies.

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire site (all 8 pages, styles, and scripts) |
| `favicon.png` | Browser tab icon |
| `apple-touch-icon.png` | Icon used when saved to a phone home screen |
| `og-image.png` | Preview image shown when the site is shared on social media / iMessage / Slack |

## Publish it on GitHub Pages

1. Create a new **public** repository on GitHub (e.g. `disease-detectives-site`).
2. Upload all four files in this folder to the root of that repository.
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment**, set Source to **Deploy from a branch**,
   branch `main`, folder `/ (root)`, then Save.
5. Wait a minute or two, then refresh that Pages settings page — it will show
   your live URL, something like `https://yourusername.github.io/disease-detectives-site/`.
6. (Optional) Add a custom domain in that same Pages settings screen, and
   point a CNAME record at your domain registrar to `yourusername.github.io`.

## Two things to finish before it's fully live

1. **Connect the forms.** Open `index.html`, search for `YOUR_FORM_ID`
   (it appears twice — once for the Join Us form, once for Contact), and
   replace it with a real form ID from [formspree.io](https://formspree.io)
   (free — sign up, create a form, copy the ID it gives you). Until this is
   done, the forms still show a confirmation message but nothing is actually
   emailed anywhere.
2. **Update the share-link URL.** In the `<head>`, find the line
   `<meta property="og:url" content="...">` and replace it with your final
   GitHub Pages or custom domain URL, once you know it.

## Also worth updating once you have real numbers/details

- The **Impact stats** section on the Home page (workshops run, students
  reached, schools partnered) currently uses placeholder figures.
- The **workshop schedule** table and **social media links** in the footer
  and Contact page are placeholders.
