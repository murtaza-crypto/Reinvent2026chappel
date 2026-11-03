# Little Chapel of Structured Data

Landing page for LlamaIndex at AWS re:Invent 2026. Preserves the supplied website, including inline styles, scripts, and embedded artwork.

## Run locally

From this directory, run `python3 -m http.server 3000` and open http://localhost:3000.

## Deploy on Vercel

Import this GitHub repository into a new Vercel project. Choose **Other** as the framework, use the repository root, leave the build and install commands empty, and set the output directory to `.`. No dependencies or environment variables are required. Pushes to `main` trigger production deployments once the repository is connected.

## Configure booking

All booking buttons open the Chili Piper URL configured in `BOOKING_LINK` inside an accessible modal. Visitors complete the booking in Chili Piper. The modal closes only when its frame sends `booking-confirmed` from the configured Chili Piper origin, not on the earlier `booked` or `timeslot-selected` actions. Close button, Escape, backdrop dismissal, focus restoration, scroll locking and a new-tab fallback are included.

Chili Piper references: https://help.chilipiper.com/hc/en-us/articles/1500011381522-Capturing-Javascript-Messaging-in-Browser and https://help.chilipiper.com/hc/en-us/articles/12601963874323-Embedding-A-Calendar-or-Booking-Link

## Assets and demo

Artwork is embedded in the HTML. Fonts load from Google Fonts with local fallbacks. The ceremony is a browser-side demonstration with sample data; it does not call a document-processing service.
