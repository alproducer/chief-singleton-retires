# ChiefSingletonRetires.com

Netlify-ready static wrapper for the Icarus Invites event page.

## What this does
- Keeps `ChiefSingletonRetires.com` as the page people share.
- Supplies custom Open Graph / social preview metadata.
- Embeds the live Icarus invitation so updates there can appear here automatically, if Icarus allows iframe embedding.
- Includes a visible **Open RSVP** button that opens the Icarus page directly.

## Deploy on Netlify
1. Unzip this folder.
2. In Netlify, choose **Add new project > Deploy manually** (or drag-and-drop the folder).
3. After Netlify gives you a temporary `*.netlify.app` address, add `ChiefSingletonRetires.com` under **Domain management**.
4. Follow Netlify's DNS instructions at the registrar where you bought the domain.
5. Netlify should issue HTTPS automatically after DNS resolves.

## Social sharing image
`og-image.png` is the image shown when the URL is texted/shared by services that honor Open Graph metadata.

The included version is a temporary text-only card. Replace it with the preferred portrait/invitation graphic, but KEEP THE SAME FILE NAME: `og-image.png`.

Recommended dimensions: 1200 x 630 px.

## Important iframe note
Icarus may block embedding using `X-Frame-Options` or a Content-Security-Policy `frame-ancestors` rule. If that happens, the browser will refuse to display the invitation inside this page. The **Open RSVP** button will still work.

If Icarus blocks the iframe, the next-best approach is to recreate the visible invitation as native HTML/CSS on this site and keep the RSVP button linked to Icarus.
