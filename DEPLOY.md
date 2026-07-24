# Go-live — cortexsolution.ca
*DFY path, ~10 minutes, no CLI.*

## Before deploying (2 required edits in index.html)

1. Replace `REPLACE_WITH_VAPI_PUBLIC_KEY` with the **public** key (Vapi dashboard → Settings → API Keys → Public). Never the private key — anyone can read frontend code.
2. In Vapi → Billing, **set a spend limit** — a public call button on a public URL is billable by strangers.
3. (When the 514 number exists: swap the "Numéro démo — bientôt" strings in the `STR` object for the real number.)

## Deploy (Netlify Drop — free, includes TLS)

1. Go to https://app.netlify.com/drop (create free account if needed).
2. Drag the `site/` folder onto the page → site is live at `something.netlify.app` in seconds.
3. Site settings → Domain management → Add custom domain → `cortexsolution.ca` (+ `www.cortexsolution.ca`).

## DNS (at the registrar where the domain was bought)

Add these records:

| Type | Name | Value |
|---|---|---|
| A | @ | 75.2.60.5 |
| CNAME | www | `<your-site>.netlify.app` |

Propagation: minutes to a few hours. Netlify auto-issues the HTTPS certificate once DNS resolves. Alternative: transfer nameservers to Netlify DNS (their UI offers it) — even simpler long-term.

## Verify

- https://cortexsolution.ca loads with the padlock, FR by default, EN toggle works.
- The call button starts a browser call to the assistant (after the public key is in).
- Check on a phone — the whole page must be readable one-handed.
