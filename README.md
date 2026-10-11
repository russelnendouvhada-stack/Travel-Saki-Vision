# Travel Saki

A responsive, destination-led travel website created by RNX Technology for Travel Saki. The site uses the logo supplied by Russel Nendou and travel photography from Travel Saki’s websites.

## Run locally

No installation or build step is needed. With Python installed, run:

```bash
python -m http.server 8080 --directory dist
```

Open `http://localhost:8080`. The source consists of `dist/index.html`, `dist/styles.css`, `dist/app.js` and `dist/assets/`.

## Features

- Home, destinations, tours, transport, company story and trip planning views.
- Destination search, experience filters and price/name sorting.
- A device-local shortlist and detailed package dialogs.
- A trip enquiry builder with review, WhatsApp, email and copy actions.
- Responsive layouts, keyboard navigation, accessible form labels and reduced-motion support.
- Privacy and booking information views.

The form prepares a message in the visitor’s browser. It does not store submissions or confirm bookings. Visitors must send their message in WhatsApp or their email app. Payment processing and live inventory are not integrated.

## Research and content

Reviewed on 12 October 2026 (South Africa time):

- Original website: https://www.travelsaki.co.za/
- Original company story: https://www.travelsaki.co.za/about.html
- Original contact and official social links: https://www.travelsaki.co.za/contact.html
- Newer site: https://travelsakisa.co.za/
- Published tour catalogue: https://travelsakisa.co.za/shop/
- Current about/contact/transport/activities pages on the newer site.
- Instagram: https://www.instagram.com/travelsaki_sa/
- Facebook: https://www.facebook.com/Travelsakisa/

Both social profiles’ public metadata were retrieved and their identities verified against the original site’s contact links. Individual posts and full feeds were not accessible. The gallery therefore uses operator website photography and does not pretend to be a live social feed.

Package prices come from the operator’s published catalogue. Cape Town, Mozambique, Namibia, Mauritius, Zanzibar and Sun City detail highlights were checked against product pages. Where departures have passed or wording is unclear, the site asks visitors to confirm new dates. Seasonal offers and a past Mother’s Day offer are not presented as current departures. There are no invented ratings, traveller counts or testimonials. The Dudu Mabaso quote is the brief testimonial published on the newer About page.

## Content updates

Edit the `tours` array in `dist/app.js` to update package prices, images, details or dates. Verify changes with Travel Saki before public launch. All prices are marked as published reference prices; final dates, availability, terms and quotes are confirmed directly with the operator.

The supplied PNG is retained unmodified as `dist/assets/logo.png`; `logo-trim.png` removes only transparent outer margins for layout. Images were converted to WebP for performance. Brand colours are gold, warm ivory and deep green.

## Deployment

Deploy the `dist` directory as static assets. Hash routes do not require server rewrite rules. `vercel.json` configures this repository for Vercel static deployment. Sites identity and static directory are declared in `.openai/hosting.json`.

## Ownership

Travel Saki’s logo, photography and business content belong to their respective rights holders. This project is prepared for client review. It does not transfer brand or image rights.
