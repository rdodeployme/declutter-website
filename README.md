# Declutter.com.au — website

Static site: `index.html` contains every page (Home, Services, How it works, About, FAQ, Contact) with hash routing, so it runs from GitHub Pages with no build step.

**Publish:** Settings → Pages → Source: *Deploy from a branch* → Branch: `main` / root → Save.

**Before go-live, replace the placeholders:**
- `1300 XXX XXX` → the allocated 1300 number (search-and-replace, and change `href="#contact"` on the phone links to `href="tel:1300XXXXXX"`).
- `NDIS provider details: to be confirmed` → registration number + entity, once confirmed.
- Photos live in `images/` (AI-generated in Higgsfield as stand-ins; the file names describe each shot). Swap for real team/job photos when you have them — keep the same file names and nothing else needs to change.
- "Part of the Recycle Group" footer line → the actual mark (small).

The contact form has Netlify attributes on it; on GitHub Pages it needs a form handler (e.g. Formspree, or a `mailto:`) — the `<form>` tag's `action` is the only thing to change.
