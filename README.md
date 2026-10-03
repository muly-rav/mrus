# MRUS Consulting website

Single-page static site (`index.html`) hosted free on GitHub Pages.

## Publish (GitHub Pages)
1. Repo **Settings → Pages**.
2. Source: **Deploy from a branch** → branch `main`, folder `/ (root)` → Save.
3. Site goes live at `https://muly-rav.github.io/mrus/` within a minute or two.
   Note: on a free GitHub plan, Pages only works if the repo is **public**.

## Custom domain (www.mrus.asia, DNS at GoDaddy)
1. Settings → Pages → Custom domain: `www.mrus.asia` (also set by the `CNAME` file) → Save, then tick **Enforce HTTPS**.
2. At GoDaddy → My Products → mrus.asia → DNS:
   - `CNAME` record: `www` → `muly-rav.github.io`
   - `A` records (name `@`) for the bare domain `mrus.asia`:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Delete GoDaddy's default `A @` ("Parked") record and any old `www` record first.
   - Leave the existing `MX` / email records alone.

## Contact form
The form posts to [FormSubmit](https://formsubmit.co) (free, no account) and emails
`muly@mrus.com`. **One-time activation:** after the site is live, submit the form
once; FormSubmit sends a confirmation email to muly@mrus.com — click the link in it.
Every submission after that is delivered to the inbox (check spam the first time).
