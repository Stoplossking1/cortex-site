# Deploying cortexsolution.ca

The public site is deployed from the `main` branch of `Stoplossking1/cortex-site` through GitHub Pages. The custom domain is defined in `CNAME` as `cortexsolution.ca`.

## Publish

1. Validate `index.html` locally, including desktop/mobile layout, dialogs, demo scenarios, and the pilot email action.
2. Commit only the intended site files.
3. Push `main` to `origin`.
4. Wait for GitHub Pages to publish the new commit.

## Verify

- `https://cortexsolution.ca` loads over HTTPS.
- The page title describes equipment rental services, not one rental segment.
- Construction/tools, party/event, AV/film/camera, landscaping/agriculture, and specialty rental are represented.
- Demo tabs open and switch among the construction, party/event, and AV/film scenarios.
- The mobile menu and all dialogs open, close, and return focus correctly.
- Pilot and contact actions address `jordan@apmode.co`.

## Product guardrail

The public demo is a transparent simulation. Do not embed a customer-specific Vapi assistant or publish a billable public call button until the category-level assistant, phone controls, spend cap, and failure behavior are tested.
