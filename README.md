# Shiva Super Mart — React website

16 pages built with React 19, Vite and Lucide icons. Run `npm install`, `npm run dev`, or `npm run build`.

## Pages
Home, About, All Categories, Agricultural Machinery, Hardware & Tools, Pipes & Fittings, Spare Parts, Oils & Lubricants, Pumps & Water Tanks, Paint & Building Essentials, Machinery Services, Bulk Enquiries, Gallery, Buying Guide, FAQs, Contact.

Home has nine main sections; all other content pages have at least seven, including their hero. Category content is defined in `src/data.js`. Branding colours and responsive layouts are in `src/style.css`.

## Lead generation
The guided popup opens from enquiry buttons or once per browser session after 35 seconds. It asks for category, requirement, timing, location, name and phone, then explicit consent. The final action prepares a WhatsApp message to +91 6394906263. The visitor must review and send it in WhatsApp. Forms do not submit to a database or CRM and the site does not store visitor contact information. Only a session flag suppresses repeated automatic popups. Contact-page form uses the same flow.

Contact details come from the supplied poster. Availability, prices, hours, delivery, installation, warranties and service appointments require confirmation from the store. No invented product prices or customer reviews are used. Images are supplied store photographs and artwork; they are not an inventory feed.

The site uses path-based navigation and requires SPA fallback to `index.html` on static hosting. Build emits static route entrypoints for all 16 pages as an additional compatibility measure. Google Maps opens an address search, not a verified map pin.

## Vercel deployment
Import this repository in Vercel. Framework: Vite. Build command: `npm run build`. Output directory: `dist`. No environment variables or API credentials are required. `vercel.json` provides these settings; the postbuild script writes entrypoints for all 16 routes.
