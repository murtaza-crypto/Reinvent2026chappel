# Little Chapel of Structured Data

Landing page for LlamaIndex at AWS re:Invent 2026. Preserves the supplied website, including inline styles, scripts, and embedded artwork.

## Run locally

From this directory, run `python3 -m http.server 3000` and open http://localhost:3000.

## Deploy on Vercel

Import this GitHub repository into a new Vercel project. Choose **Other** as the framework, use the repository root, leave the build and install commands empty, and set the output directory to `.`. No dependencies or environment variables are required. Pushes to `main` trigger production deployments once the repository is connected.

## Configure booking

In `index.html`, replace the `BOOKING_LINK` placeholder with the HTTPS scheduler URL. Until configured, booking buttons display the original calendar-coming-soon message.

## Assets and demo

Artwork is embedded in the HTML. Fonts load from Google Fonts with local fallbacks. The ceremony is a browser-side demonstration with sample data; it does not call a document-processing service.
