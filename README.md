# Golden Gate Design Story Page

A static, mobile-first landing page intended for the QR code on the 4 × 4 information card.

## What is included

- `index.html` — page structure and copy
- `styles.css` — responsive design
- `script.js` — mobile navigation and automatic copyright year
- `assets/` — current product and information-card images

## Edit before publishing

Search `index.html` for these links and replace them when your final URLs are ready:

- `https://goldengatefurniture.com` — currently used for all Shop buttons
- Google Maps directions link for Made in San Francisco Gallery

The visible brand is Golden Gate Design, while sales currently route to the existing Golden Gate Furniture store.

## Publish with GitHub and Cloudflare Pages

### 1. Create a GitHub repository

1. Sign in to GitHub.
2. Click **New repository**.
3. Name it something like `golden-gate-design-story`.
4. Keep it Public or Private; either works with Cloudflare Pages.
5. Do not add a README because one is already included here.

### 2. Upload the files

Unzip this package. In the new GitHub repository:

1. Click **Add file → Upload files**.
2. Drag in `index.html`, `styles.css`, `script.js`, `README.md`, and the `assets` folder.
3. Commit the files to the `main` branch.

You can also use GitHub Desktop if you prefer.

### 3. Connect Cloudflare Pages

1. Sign in to Cloudflare.
2. Go to **Workers & Pages → Create → Pages → Connect to Git**.
3. Select the GitHub repository.
4. Use these build settings:
   - Framework preset: **None**
   - Build command: leave blank
   - Build output directory: `/`
5. Click **Save and Deploy**.

Cloudflare will provide a temporary `pages.dev` address.

### 4. Connect the custom domain

In the Cloudflare Pages project:

1. Open **Custom domains**.
2. Add `goldengatedesign.com` or a subdomain such as `story.goldengatedesign.com`.
3. If the domain is already on Cloudflare DNS, Cloudflare will add the required record.

If this page should live at `goldengatedesign.com/story`, use one of these approaches:

- Make this page the main homepage and use `goldengatedesign.com` on the card, or
- Put the project on `story.goldengatedesign.com`, or
- Add it to a larger Golden Gate Design site later as the `/story` route.

For a first launch, using the main domain or `story.goldengatedesign.com` is simplest.

## QR-code tracking

Create the QR code using a trackable URL such as:

`https://goldengatedesign.com/?utm_source=info_card&utm_medium=qr&utm_campaign=bridge_story`

If you use different print runs or distribution channels, change `utm_source`:

- `amazon_insert`
- `etsy_insert`
- `street_fair`
- `gallery_handout`
- `open_studios`

All can open the same page while analytics shows where scans came from.

To track visits, add Google Analytics, Cloudflare Web Analytics, or another analytics script to the `<head>` of `index.html`.

## Image notes

The current files use photos supplied during development. Replace them at any time by keeping the same filenames, or update the `src` paths in `index.html`.
