# Mindathlon — website

Static site for the Mindathlon mobile app, served by GitHub Pages at
<https://nodabasi.github.io/mindathlon/>.

Plain HTML and one stylesheet — no build step, no dependencies. Edit a file, commit,
push; Pages redeploys in a minute or two.

## Pages

| URL | File | Used in the stores as |
|---|---|---|
| `/mindathlon/` | `index.html` | Marketing URL (English) |
| `/mindathlon/support/` | `support/index.html` | Support URL (English) |
| `/mindathlon/privacy/` | `privacy/index.html` | Privacy Policy URL (English) |
| `/mindathlon/tr/` | `tr/index.html` | Marketing URL (Turkish) |
| `/mindathlon/tr/support/` | `tr/support/index.html` | Support URL (Turkish) |
| `/mindathlon/tr/privacy/` | `tr/privacy/index.html` | Privacy Policy URL (Turkish) |

**Do not rename these directories.** The paths are registered in App Store Connect and
Google Play Console; changing one breaks a live store link.

## Editing

- Colours and layout live in `assets/style.css`; every page shares it.
- Links are relative, so the site also opens correctly straight from the filesystem.
- When the privacy policy changes in substance, update the effective date at the top of
  both `privacy/index.html` and `tr/privacy/index.html`.

## Local preview

```sh
python3 -m http.server 8000
# then open http://localhost:8000/
```
