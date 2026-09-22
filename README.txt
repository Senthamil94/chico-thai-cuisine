CHICO THAI CUISINE — redesigned website
=======================================

WHAT'S HERE
  index.html    Home — hero slider, highlights, story, market teaser, reviews, map, FAQ
  menu.html     Full menu (107 dishes) with live search, filters and sticky category nav
  market.html   Thai Market / supermarket page (8 aisles)
  gallery.html  All 21 photos with a keyboard-accessible lightbox
  about.html    Story + why-choose-us + FAQ
  contact.html  Contact details, message form, full-width map
  accessibility.css / accessibility.js
                Accessibility tools widget (same tools as Delhi to Kathmandu)
  img/          Logo, slider, gallery, market photos, and the boons logo
  robots.txt / sitemap.xml

HOW TO PUT IT LIVE
  Upload the HTML files, accessibility.css, accessibility.js, and the whole /img
  folder to the root of chicothaicuisine.com. Nothing else to install — no build
  step, no framework. Keep the /img folder with the pages so photos and the
  boons logo load locally.


TWO THINGS TO SWAP BEFORE YOU GO LIVE
-------------------------------------
1. ORDERING LINK
   Every "Order Online" button points to:
       https://order.boons.io/site/chico-thai-cuisine
   Replace it with your real boons store URL. Find and replace that exact string
   across all 6 HTML files — it appears in the header, drawer, hero slider,
   mobile dock, every menu category, the CTA bands, the footer and the schema.

2. MENU PRICES
   Prices came from your current live listings. Check them against your POS
   before publishing — they're in menu.html, one <div class="mi"> per dish.


ACCESSIBILITY
  The wheelchair button bottom-left opens the same accessibility tools used on
  Delhi to Kathmandu: text size, high contrast, grayscale, dark mode, underline
  links, readable font, highlight links/headings, stop animations, reading
  guide, saturation and brightness. Settings reset on refresh.
  Plus skip-to-content, visible focus rings, full ARIA on the slider, lightbox
  and menu filters, and prefers-reduced-motion support.
  The footer copyright includes Terms, Privacy policy, Accessibility, and the
  boons logo ("Powered by boons").


SEO
  Every slide carries its own SEO heading (one H1 on the homepage, the rest H2):
    1. Authentic Thai Restaurant in Chico, CA
    2. Best Pad Thai & Curry Near Downtown Chico
    3. Fresh Thai Seafood, Noodles & Chef's Specials
    4. Thai Market & Grocery Supermarket in Chico
  Each page has its own title, meta description, canonical, Open Graph tags.
  Restaurant schema.org JSON-LD (address, hours, phone, menu, order action)
  is embedded on every page.


EDITING LATER
  Hours              search for "11:00 AM – 8:30 PM" (and OPEN_FROM / OPEN_TO
                     near the bottom of each file — these drive the live
                     "Open now / Closed" badge)
  Phone / address    search for "530) 717-9108" and "407 Walnut"
  Market aisles      market.html, the <article class="aisle"> blocks
  Colours            the :root block at the top of each <style> tag
