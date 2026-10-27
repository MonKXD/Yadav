# Sunchem: SEO and SEM plan

Everything marked **Done** is already in the site files. Everything else needs an account or a decision from you.

## 1. SEO: done on the site

| Item | What was done |
|---|---|
| Title tag | "Sunchem – Paint Raw Materials Manufacturer & Importer, India" (60 characters) |
| Meta description | 160 characters, with the main product terms and a call to action |
| Canonical URL | Set to `https://monkxd.github.io/Yadav/`. **Change it if you use your own domain.** |
| Social sharing | Open Graph and Twitter card tags, with title, description, image and `en_IN` locale |
| Structured data | JSON-LD for Organization and LocalBusiness: name, legal name, address, both phone numbers, email, opening hours, founding year 2013 |
| Page structure | One `h1`, `h2` per section, a `<main>` landmark, labelled navigation |
| Images | Descriptive alt text on the hero image and logos. The hero image is preloaded, the footer logo loads lazily. |
| Click-to-call and click-to-email | Phone numbers and the email address are real `tel:` and `mailto:` links |
| Crawling | `robots.txt` and `sitemap.xml` added |
| 404 page | Marked `noindex` |
| Speed | Inter font reduced to the 5 weights the site uses |
| Tracking hook | A successful enquiry pushes an `enquiry_submit` event to `dataLayer` (for Google Tag Manager or GA4) |

## 2. SEO: steps only you can do

1. **Decide the final web address.** If you buy a domain, send it to me and I will update the canonical URL, sitemap, robots.txt and structured data.
2. **Google Search Console:** add the site, verify it, and submit `sitemap.xml`. Then use URL Inspection and click "Request indexing".
3. **Google Business Profile:** create or claim a profile with the same name, address and phone numbers as the website, category "Chemical manufacturer" or "Chemical wholesaler", and Mon–Sat 9 AM–6 PM hours. Keep the details identical everywhere.
4. **Directories:** list Sunchem on IndiaMART, TradeIndia and similar B2B directories, using the same name, address and phone (NAP) as the site.
5. **Backlinks:** ask suppliers and principals (Pidilite, Soham Polymers, Meghmani, Nigtas and others) whether they will link to you.
6. **Bundle the images** with `download-assets.sh` so the site loads fast and does not depend on Base44's servers.

## 3. SEO: content gaps (needs your decision)

The page is one long scroll. Search engines rank pages for specific topics, so separate pages help. I did not add them because you asked to keep the site as it is.

- Product pages, one each for pigment pastes, carbon black paste (gelling and non-gelling), acrylic emulsions, calcium carbonate and Blanc Fixe, each with specifications and an enquiry button.
- A short blog or guide section, for example "Gelling vs non-gelling carbon black paste".
- The main headline ("Raw Materials. Refined Excellence.") has no search terms. The subline under it ("Manufacturer · Distributor · Importer of Premium Paint Raw Materials") carries them.

## 4. SEM (Google Ads): starter plan

I can't create or run ads from here (no Ads account access). Search volumes and costs below are not known to me. **Validate every keyword in Google Keyword Planner before spending.**

**Settings**
- Campaign type: Search. Network: Search only (turn off the Display network).
- Locations: Maharashtra first, then India. Add Mumbai and Thane as bid boosts. Use "Presence" targeting, not "Presence or interest".
- Language: English. Add Hindi later if enquiries come in Hindi.
- Schedule: show ads Mon–Sat, 9 AM–6 PM IST, when the sales team can answer calls.
- Extensions: call (+91 22 48016417), sitelinks (Products, Clients, Request a Quote), structured snippets (Binders, Pigments, Additives).
- Conversions: count the `enquiry_submit` event and phone calls from the ad.

**Campaigns and ad groups (suggested keywords)**

| Campaign | Ad group | Example keywords |
|---|---|---|
| Pigment pastes | Pigment paste | pigment paste manufacturer, water based pigment paste, solvent based pigment paste |
| Pigment pastes | Carbon black | carbon black pigment paste, carbon black paste supplier, non gelling carbon black paste |
| Binders | Acrylic | acrylic emulsion for paint, pure acrylic emulsion supplier, paint binder supplier India |
| Extenders | Calcium carbonate | calcium carbonate for paints, coated calcium carbonate supplier, paint filler supplier |
| Extenders | Blanc fixe | blanc fixe supplier India, precipitated barium sulphate for paint |
| Pigments | Pigments | organic pigment supplier India, azo pigments for paint, titanium dioxide distributor |
| Additives | Additives | defoamer for paint, wetting and dispersing agents, paint additive supplier |

Use phrase and exact match. Start with a daily budget you are comfortable testing for 4 to 6 weeks, then move budget to the ad groups that bring enquiries.

**Negative keywords to add on day one:** free, diy, job, jobs, career, course, training, pdf, wikipedia, home use, retail, buy online, small pack, paint colour, paint price list.

**Responsive search ad text (within Google's limits)**

Headlines (30 characters or fewer):
1. Paint Raw Materials India
2. Pigment Paste Manufacturer
3. Acrylic Emulsion Supplier
4. Carbon Black Paste Supplier
5. Calcium Carbonate for Paints
6. Manufacturer & Importer
7. Get a Quote in 24 Hours
8. Sunchem – Mumbai Region
9. Authorised Distributor
10. Titanium Dioxide Supplier

Descriptions (90 characters or fewer):
1. Manufacturer, distributor and importer of paint raw materials. Request a quote today.
2. Binders, pigments, pigment pastes, calcium carbonate and additives for paint makers.
3. Technical sales team replies within 24 hours with pricing and availability.

Only claim what is true. "Authorised Distributor" and "24 hours" come from the site text. Remove a line if it is not accurate for a specific product.

**Landing pages:** send each ad group to the matching product section (`#products`), or better, to its own product page once those exist. Sending all traffic to the home page lowers conversion.

## 5. Tracking checklist

1. Create a GA4 property and a Google Tag Manager container (you create them, then send me the IDs and I will add the snippets).
2. In Tag Manager, create a trigger on the custom event `enquiry_submit` and send it to GA4 as a conversion.
3. Import that conversion into Google Ads.
4. Link Search Console, GA4 and Google Ads.
5. Check the contact form really saves to Base44 (not yet tested), since every conversion depends on it.
