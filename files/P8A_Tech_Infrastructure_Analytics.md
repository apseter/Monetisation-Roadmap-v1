# P8A: TECH INFRASTRUCTURE & ANALYTICS
## Shopify Store, Tracking Pixels, Analytics & Tool Stack Configuration
### Modular-Liner Trail Shorts D2C Brand | March 2026 | Confidential

---

> **P8A Subproject Summary:** This document covers the complete technical infrastructure for the DTC store: Shopify configuration, Google Analytics 4 setup, Meta Pixel + Conversions API, TikTok Pixel, Microsoft Clarity, UTM architecture, Shopify app stack, email/SMS tech, site speed optimization, mobile experience, security, and a backup/disaster recovery plan. Everything a solo founder needs to build a technically sound Shopify store.

> **P8A Core Principle:** Install tracking BEFORE your first visitor. Every session without analytics is lost data. Get GA4, Meta Pixel (with CAPI), and Microsoft Clarity live on the password page during pre-launch — not on launch day.

---

## P8A TABLE OF CONTENTS

1. P8A.1: Shopify Store Configuration
2. P8A.2: Theme Selection & Customization
3. P8A.3: Shopify App Stack (Complete)
4. P8A.4: Google Analytics 4 (GA4) Setup
5. P8A.5: Meta Pixel + Conversions API (CAPI)
6. P8A.6: TikTok Pixel
7. P8A.7: Microsoft Clarity (Free Heatmaps)
8. P8A.8: Google Search Console
9. P8A.9: UTM Architecture & Link Tracking
10. P8A.10: Shopify Product Data Structure
11. P8A.11: Site Speed Optimization
12. P8A.12: Mobile Experience Checklist
13. P8A.13: Email/SMS Technical Setup (Klaviyo)
14. P8A.14: Domain, DNS & SSL
15. P8A.15: Security & Fraud Prevention
16. P8A.16: Backup & Disaster Recovery
17. P8A.17: Technical Launch Checklist
18. P8A.18: P8A Action Items

---

## P8A.1: SHOPIFY STORE CONFIGURATION

### P8A.1.1: Plan Selection

**Shopify Basic at £25/month** (or £19/month on annual billing). Upgrade to Grow (£65/month) only when monthly revenue consistently exceeds £5,000-10,000 — the 0.3% processing fee difference saves ~£15-30/month at that volume.

### P8A.1.2: Store Settings Checklist

| Setting | Location | Value |
|---|---|---|
| Store name | Settings → General | [Brand Name] |
| Store currency | Settings → General | GBP |
| Store address | Settings → General | UK registered office address |
| Unit system | Settings → General | Metric |
| Time zone | Settings → General | (GMT) London |
| Order ID format | Settings → General | #1001 (default) |
| Customer accounts | Settings → Customer accounts | Optional (don't force registration) |
| Checkout | Settings → Checkout | Guest checkout enabled, email as primary contact |
| Tipping | Settings → Checkout | Disabled (not appropriate for apparel) |
| Order processing | Settings → Checkout | Don't auto-fulfil, don't auto-archive |

### P8A.1.3: Checkout Optimization

| Setting | Recommendation | Why |
|---|---|---|
| Express checkout | Enable Shop Pay + Apple Pay + Google Pay | 1-click checkout increases conversion 10-18% |
| Customer contact | Email (not phone) | Lower friction, GDPR-simpler |
| Name fields | First + Last (required) | Needed for shipping labels |
| Company field | Optional (hidden by default) | Most B2C customers don't need it |
| Address autocomplete | Enable (Shopify default) | Reduces address errors |
| Post-purchase page | Enable (for upsell) | Cross-sell liner/outer after purchase |

---

## P8A.2: THEME SELECTION & CUSTOMIZATION

### P8A.2.1: Theme Comparison

| Theme | Cost | Best For | Limitations |
|---|---|---|---|
| **Dawn** (free) | £0 | Clean, fast, minimal. Default Shopify theme. | Basic design, limited sections |
| **Refresh** (free) | £0 | Modern, editorial feel | Newer, less documentation |
| **Impulse** | £380 | Rich media, promotional features | Cost |
| **Prestige** | £350 | Premium brand feel, storytelling | Cost |

**Recommendation: Dawn (free) for launch.** It's the fastest Shopify theme (97+ Lighthouse score), fully OS 2.0 compatible, and adequate for a 2-4 product store. Upgrade to a paid theme (Impulse or Prestige) at 1,000+ monthly sessions when design becomes a conversion bottleneck.

### P8A.2.2: Essential Theme Customizations

| Element | Configuration | Where |
|---|---|---|
| Logo | Upload SVG or PNG (max height 60px header) | Theme → Header |
| Favicon | 32×32 PNG | Settings → Brand |
| Colors | Set brand palette (primary, secondary, accent) | Theme → Colors |
| Typography | Set heading + body fonts (Google Fonts) | Theme → Typography |
| Announcement bar | "Free UK Shipping Over £40 🇬🇧" | Theme → Header → Announcement |
| Homepage sections | Hero banner → Featured collection → Value props → Blog posts → Email signup | Theme → Home page |
| Product page | Image gallery left + details right + size guide tab + FAQ accordion + reviews | Theme → Product pages |
| Footer | 4 columns: Shop / Help / Legal / Newsletter | Theme → Footer |

### P8A.2.3: Critical Product Page Elements

Every product page MUST include (in order of importance):

1. **Product images** — 6-8 images: front, back, detail (snaps, pocket, DWR), on-model (trail), flat lay, modular demo
2. **Price** with bundle savings shown (~~£43~~ £39)
3. **Size selector** with "Size Guide" link that opens modal/tab
4. **Colour selector** with swatches
5. **Add to Cart** button (prominent, above fold on mobile)
6. **"Complete Your System"** cross-sell (if viewing outer → show liner, and vice versa)
7. **Key features** — 4-5 bullet points with icons: DWR, modular, phone pocket, inclusive sizing, flatlock seams
8. **Size guide** — full measurement table (cm + inches) in a tab or accordion
9. **FAQ accordion** — 5-6 product-specific questions
10. **Reviews** (Judge.me widget)
11. **"You may also like"** — related products

---

## P8A.3: SHOPIFY APP STACK (COMPLETE)

### P8A.3.1: Essential Apps (Install Before Launch)

| App | Cost | Purpose | Priority |
|---|---|---|---|
| **Simple Bundles** | $15/mo | Bundle inventory sync (outer + liner = system) | CRITICAL |
| **Judge.me** (Free) | £0 | Product reviews + star ratings + Schema markup | CRITICAL |
| **Kiwi Sizing** (Free) | £0 | Interactive size guide / fit quiz | HIGH |
| **Klaviyo** | £0 (free to 250 contacts) | Email marketing + flows | CRITICAL |
| **Sendcloud** | £0 (free to 100 labels/mo) | Multi-carrier shipping labels + tracking | CRITICAL |
| **Google & YouTube** channel | £0 | GA4 integration + Google Shopping feed | HIGH |
| **Facebook & Instagram** channel | £0 | Meta Pixel + Conversions API + Instagram Shopping | HIGH |
| **TikTok** channel | £0 | TikTok Pixel + catalog sync | MEDIUM |
| **Translate & Adapt** | £0 | French translation (2 languages free) | HIGH |
| **CookieYes** | £0 (free to 100 pages) | Cookie consent banner (GDPR/PECR) | CRITICAL |
| **Back in Stock: Restock Alerts** (Swym) | £0 | Email notification when sold-out items return | HIGH |
| **JSON-LD for SEO** | £0 | Enhanced Schema markup (Product, FAQ, Breadcrumb) | MEDIUM |

### P8A.3.2: Post-Launch Apps (Add When Needed)

| App | Cost | Trigger to Install | Purpose |
|---|---|---|---|
| **AfterShip Returns** | $23/mo | Returns >5/month | Self-serve returns portal |
| **Tidio** | £0→$29/mo | CS tickets >20/month | Live chat + AI chatbot |
| **UpPromote** | £0→$29.99/mo | Ambassador codes active | Referral + affiliate tracking |
| **Shopify Email** | £0 (2,500 emails free/mo) | Backup to Klaviyo | Simple campaigns |

### P8A.3.3: Apps to AVOID

| App | Why Not |
|---|---|
| Oberlo / DSers | Dropshipping — you're manufacturing |
| Bold Bundles | More expensive than Simple Bundles, no advantage at your scale |
| Privy | Inferior to Klaviyo for email capture |
| Yotpo (paid) | $79/mo minimum — Judge.me Free does 95% of the same |
| PageFly / Shogun | Page builders — unnecessary with Dawn theme, add bloat |

---

## P8A.4: GOOGLE ANALYTICS 4 (GA4) SETUP

### P8A.4.1: Setup via Google & YouTube Channel

1. Install "Google & YouTube" Shopify app (free)
2. Connect your Google account
3. App auto-creates GA4 property and installs gtag.js
4. Auto-tracks: page_view, view_item, add_to_cart, begin_checkout, purchase, search
5. Verify events firing via GA4 → Admin → DebugView

### P8A.4.2: Enhanced Ecommerce Events (Auto-Tracked)

| Event | When | Data |
|---|---|---|
| page_view | Every page load | Page title, URL, referrer |
| view_item | Product page viewed | Product name, ID, price, category |
| add_to_cart | Add to Cart clicked | Product, quantity, value |
| remove_from_cart | Item removed from cart | Product, quantity |
| begin_checkout | Checkout started | Cart contents, total value |
| add_shipping_info | Shipping selected | Shipping method |
| add_payment_info | Payment entered | Payment method |
| purchase | Order confirmed | Order ID, revenue, tax, shipping, items |

### P8A.4.3: Custom Events to Add

| Event | How | Purpose |
|---|---|---|
| size_guide_click | GA4 event via theme customization | Measure size guide engagement (reduces returns) |
| email_signup | Klaviyo → GA4 integration | Track email capture conversion rate |
| bundle_upsell_click | Custom event on "Complete Your System" click | Measure cross-sell effectiveness |

### P8A.4.4: GA4 Audiences to Create (For Future Retargeting)

| Audience | Definition | Use |
|---|---|---|
| All visitors (30 days) | page_view in last 30 days | Broad retargeting |
| Product viewers (non-purchasers) | view_item but NOT purchase in 14 days | High-intent retargeting |
| Cart abandoners | add_to_cart but NOT purchase in 7 days | Highest-value retargeting |
| Purchasers | purchase event | Lookalike seed, exclude from prospecting |
| Bundle page viewers | view_item on bundle product | Bundle-specific retargeting |

### P8A.4.5: Key GA4 Reports for DTC

| Report | Path | Check Frequency |
|---|---|---|
| Traffic acquisition | Reports → Acquisition → Traffic acquisition | Weekly |
| Landing pages | Reports → Engagement → Landing pages | Weekly |
| Ecommerce purchases | Reports → Monetization → Ecommerce purchases | Daily |
| Funnel exploration | Explore → Funnel exploration (custom) | Monthly |
| Conversion paths | Advertising → Conversion paths | Monthly |

### P8A.4.6: Ecommerce Funnel to Build

Create a custom funnel exploration: view_item → add_to_cart → begin_checkout → purchase. Benchmark conversion rate at each step. Industry averages for apparel: view→cart 8-12%, cart→checkout 40-55%, checkout→purchase 55-70%. If any step drops below these benchmarks, that's your optimization priority.

---

## P8A.5: META PIXEL + CONVERSIONS API (CAPI)

### P8A.5.1: Why CAPI Is Critical

Browser-only pixel tracking loses 15-30% of conversions due to iOS privacy changes, ad blockers, and cookie restrictions. Conversions API sends event data server-to-server, bypassing all browser limitations. **Always set CAPI to "Maximum" mode.**

### P8A.5.2: Setup via Facebook & Instagram Channel

1. Install "Facebook & Instagram" Shopify app
2. Connect Meta Business Suite account
3. Connect or create Meta Pixel
4. **Set data sharing to "Maximum"** (Settings → Data sharing → Maximum)
5. Verify domain in Meta Business Suite → Brand Safety → Domains
6. Configure 8 priority events: Purchase, AddToCart, InitiateCheckout, ViewContent, Lead, CompleteRegistration, Search, AddPaymentInfo

### P8A.5.3: Verify Pixel Is Firing

- Install **Meta Pixel Helper** Chrome extension
- Visit your store → extension should show pixel ID and events
- Check Events Manager → Test Events → enter your store URL
- Verify: PageView fires on every page, ViewContent on product pages, AddToCart on button click, Purchase on thank-you page

### P8A.5.4: Meta Custom Audiences to Create

| Audience | Definition | Min Size for Ads |
|---|---|---|
| Website visitors (180 days) | All pixel traffic | 1,000 people |
| Product page visitors (30 days) | ViewContent event | 1,000 people |
| Add to Cart (30 days) | AddToCart event | 100 people (for retargeting) |
| Purchasers (180 days) | Purchase event | 100 people |
| Email list (Klaviyo sync) | Customer list upload | 500 emails |
| 1% Lookalike of purchasers | Based on purchaser seed | Requires 100+ seed |

**Reality check:** Most of these audiences won't reach minimum size (1,000) until Month 3-4. Use **broad targeting** for prospecting ads initially, and rely on Klaviyo email for retargeting (free, no minimum audience size).

---

## P8A.6: TIKTOK PIXEL

### P8A.6.1: Setup

1. Install "TikTok" Shopify sales channel
2. Connect TikTok for Business account
3. Pixel auto-installs with standard events: PageView, ViewContent, AddToCart, CompletePayment
4. Enable "Advanced Matching" for better attribution
5. Verify via TikTok Events Manager → Test Events

### P8A.6.2: When TikTok Pixel Matters

The pixel is collecting data from Day 1 even if you're not running TikTok ads. When you eventually start TikTok Promote or TikTok Ads (Month 4+), you'll have months of pixel data for audience building. Install now, activate ads later.

---

## P8A.7: MICROSOFT CLARITY (FREE HEATMAPS)

### P8A.7.1: Why This Is the Most Underused Free Tool

Microsoft Clarity provides session recordings, heatmaps, and scroll maps — completely free, no limits. For a solo founder who can't afford Hotjar ($39/mo), Clarity is invaluable for understanding why visitors aren't converting.

### P8A.7.2: Setup

1. Create account at clarity.microsoft.com
2. Add your domain
3. Install tracking code via Shopify: Online Store → Themes → Edit code → theme.liquid → paste code before `</head>`
4. Or install the "Microsoft Clarity" Shopify app

### P8A.7.3: What to Watch For

| Insight | What to Look At | Action If Found |
|---|---|---|
| **Rage clicks** | Users clicking repeatedly on non-clickable elements | Make the element clickable or restyle |
| **Dead clicks** | Clicks on elements that do nothing | Fix broken links or confusing UI |
| **Quick backs** | Users immediately returning from a page | Page content doesn't match expectation |
| **Scroll depth** | How far users scroll on product pages | If <60% reach size guide, move it higher |
| **Form abandonment** | Where users drop off in checkout | Identify friction points |

### P8A.7.4: Weekly Clarity Review (15 Minutes)

Watch 5-10 session recordings per week, specifically: sessions where user viewed product but didn't add to cart, mobile sessions (75% of your traffic), and sessions from paid traffic sources. This reveals UX issues that analytics alone cannot detect.

---

## P8A.8: GOOGLE SEARCH CONSOLE

### P8A.8.1: Setup

1. Go to search.google.com/search-console
2. Add property → URL prefix → enter https://yourdomain.com
3. Verify via DNS record (add TXT record at your domain registrar) or via the Google & YouTube Shopify app (auto-verifies)
4. Submit sitemap: yourdomain.com/sitemap.xml (Shopify auto-generates)

### P8A.8.2: Monthly SEO Check (10 Minutes)

| Report | What to Check | Action |
|---|---|---|
| Performance | Which queries bring impressions/clicks | Create content targeting high-impression/low-click queries |
| Coverage/Indexing | Pages indexed vs submitted | Fix any "Not indexed" errors |
| Core Web Vitals | LCP, CLS, INP scores | Optimise if any "Poor" ratings |
| Links | Top linking sites | Identify PR/backlink opportunities |

---

## P8A.9: UTM ARCHITECTURE & LINK TRACKING

### P8A.9.1: UTM Naming Convention

Establish from Day 1 and NEVER deviate:

| Parameter | Convention | Example |
|---|---|---|
| utm_source | Platform (lowercase) | instagram, facebook, klaviyo, google, tiktok, reddit |
| utm_medium | Channel type | paid-social, email, organic-social, influencer, qr-code, podcast |
| utm_campaign | Campaign descriptor | launch-apr26, summer-bundle, bfcm-2026 |
| utm_content | Creative variant | video-trail-muddy, carousel-product, ambassador-sarah |

### P8A.9.2: UTM Rules

- Always lowercase, hyphens not spaces or underscores
- Never use UTMs on internal links (breaks attribution)
- Create a Google Sheet as your UTM registry (every unique URL documented)
- Use a UTM builder tool: Google's Campaign URL Builder or utm.io (free)

### P8A.9.3: Where to Apply UTMs

| Link | UTM |
|---|---|
| Instagram bio link | ?utm_source=instagram&utm_medium=organic-social&utm_campaign=bio-link |
| Klaviyo email CTA | Auto-tagged by Klaviyo (utm_source=klaviyo) |
| Ambassador discount link | ?utm_source=instagram&utm_medium=influencer&utm_content=ambassador-[name] |
| Reddit post link | ?utm_source=reddit&utm_medium=organic-social&utm_campaign=trailrunning-sub |
| Podcast mention link | ?utm_source=podcast&utm_medium=podcast&utm_campaign=[show-name] |
| QR code on event flyer | ?utm_source=qr-code&utm_medium=event&utm_campaign=lakeland-trails-may |

---

## P8A.10: SHOPIFY PRODUCT DATA STRUCTURE

### P8A.10.1: Product Setup for SEO + Shopping Feeds

Every product must have these fields populated:

| Field | Example | Why |
|---|---|---|
| Title | "Modular Trail Running Shorts – Outer Shell" | SEO title tag source |
| Description | 300-500 words, keyword-rich, formatted HTML | SEO + conversion |
| Product type | "Trail Running Shorts" | Google Shopping category |
| Vendor | "[Brand Name]" | Brand filter |
| Tags | trail-running, shorts, outer, dwr, modular, mens, womens | Internal search + collections |
| SEO title | "Modular Trail Running Shorts – DWR Outer Shell | [Brand]" | <60 chars, keyword-first |
| SEO description | "Trail running shorts with C0 DWR, 170mm phone pocket, modular liner attachment. £28. Free UK shipping over £40." | 150-160 chars |
| HS code | 6203.43.00 | Customs/duties (international shipping) |
| Country of origin | Pakistan | Customs declaration |
| Weight | 180g (outer), 120g (liner), 300g (bundle) | Shipping rate calculation |
| Barcode/SKU | OS-BLK-M | Inventory tracking |

### P8A.10.2: Variant Structure

| Product | Option 1 | Option 2 | Option 3 |
|---|---|---|---|
| Outer Short | Size (S/M/L/XL/2XL) | Colour (Slate Black/Dark Forest) | Gender (Men's/Women's) |
| Liner | Size (S/M/L/XL/2XL) | — | Gender (Men's/Women's) |
| System Bundle | Size (S/M/L/XL/2XL) | Colour (Slate Black/Dark Forest) | Gender (Men's/Women's) |

**Important:** Shopify limits products to 3 options and 100 variants. With 5 sizes × 2 colours × 2 genders = 20 variants for the outer, you're well within limits.

### P8A.10.3: Product Images

| Image | Type | Requirements |
|---|---|---|
| 1 | Hero (front view, white background) | 2048×2048px, WebP or PNG |
| 2 | Back view | Same dimensions |
| 3 | Detail — snap mechanism | Close-up, lifestyle |
| 4 | Detail — phone pocket | Phone visible in pocket |
| 5 | On-model (trail setting) | Lifestyle, action shot |
| 6 | Modular demo (outer + liner together) | Shows the system |
| 7 | On-model (women's) | Essential — women's from day one |
| 8 | Flat lay with accessories | Context/lifestyle |

All images: consistent lighting, optimised file size (<500KB), descriptive alt text for SEO.

---

## P8A.11: SITE SPEED OPTIMIZATION

### P8A.11.1: Why Speed Matters

Every 1-second delay in page load reduces conversion by **7%**. Google uses Core Web Vitals as a ranking factor. Target: Lighthouse Performance score **>80** on mobile.

### P8A.11.2: Speed Checklist

| Action | Impact | How |
|---|---|---|
| Use Dawn theme (fastest free theme) | High | Already recommended |
| Compress all images to WebP | High | Use Shopify's auto-compression or TinyIMG app |
| Limit apps to essentials only | High | Each app adds JavaScript. Remove unused apps. |
| Lazy-load images below the fold | Medium | Dawn theme does this by default |
| Minimise custom code in theme.liquid | Medium | Only add essential tracking pixels |
| Avoid page builder apps (PageFly, Shogun) | High | These add significant JavaScript bloat |
| Use system fonts or limit Google Fonts to 2 | Medium | Each font file = 20-50KB |
| Remove unused Shopify features | Low | Disable features you don't use |

### P8A.11.3: Speed Testing

| Tool | URL | Frequency |
|---|---|---|
| Google PageSpeed Insights | pagespeed.web.dev | Monthly |
| Shopify Speed Score | Online Store → Themes → Speed | Monthly |
| GTmetrix | gtmetrix.com | After any major change |

---

## P8A.12: MOBILE EXPERIENCE CHECKLIST

### P8A.12.1: Mobile Will Be 70-80% of Your Traffic

Test every page on your actual phone (not just Shopify preview). Check:

| Element | Mobile Requirement |
|---|---|
| **Add to Cart button** | Visible without scrolling on product page. Full-width, thumb-friendly (min 48px height). |
| **Product images** | Swipeable gallery with zoom. First image loads in <2 seconds. |
| **Size selector** | Large touch targets. Not tiny dropdown — use visible buttons. |
| **Price** | Clearly visible, not buried below fold |
| **Navigation** | Hamburger menu works smoothly. Search icon visible. |
| **Checkout** | Express checkout buttons (Shop Pay, Apple Pay) above standard checkout |
| **Footer** | Collapsible sections, not massive text blocks |
| **Announcement bar** | Readable on small screens, doesn't cover content |
| **Pop-ups** | Email capture pop-up must be easily dismissible. Don't trigger on page load — trigger on scroll 50% or exit intent. Google penalises intrusive mobile pop-ups. |
| **Size guide** | Opens as overlay/modal, not a new page. Pinch-to-zoom on measurement table. |

---

## P8A.13: EMAIL/SMS TECHNICAL SETUP (KLAVIYO)

### P8A.13.1: Klaviyo Configuration Checklist

| Setting | Value | Location |
|---|---|---|
| Sending domain | mail.[yourdomain].com | Klaviyo → Settings → Email → Domains |
| SPF record | Add to DNS | Provided by Klaviyo |
| DKIM record | Add to DNS | Provided by Klaviyo |
| DMARC record | v=DMARC1; p=none | Add TXT record at DNS |
| From name | "[Brand Name]" or "[Founder Name] from [Brand]" | Account settings |
| From email | hello@[brand].com | Account settings |
| Reply-to | Same as from email | Account settings |
| Shopify integration | Connected + syncing | Integrations → Shopify |
| Consent settings | Single opt-in for UK, double opt-in for EU | Lists → Settings |

### P8A.13.2: DNS Records to Add

| Record Type | Host | Value | Purpose |
|---|---|---|---|
| TXT | @ | v=spf1 include:_spf.klaviyo.com ~all | SPF — email authentication |
| CNAME | k1._domainkey | Provided by Klaviyo | DKIM — email signing |
| TXT | _dmarc | v=DMARC1; p=none; rua=mailto:dmarc@[brand].com | DMARC — deliverability |
| CNAME | mail | Provided by Klaviyo | Custom sending domain |

**Without these records, your emails will land in spam.** Set up BEFORE sending any emails.

### P8A.13.3: Klaviyo Lists vs Segments

| Type | Name | Purpose |
|---|---|---|
| **List** | Newsletter Subscribers | All email signups |
| **List** | Pre-Launch Waitlist | Founding 300 signups (archive post-launch) |
| **Segment** | Engaged 30 Days | Opened/clicked in last 30 days |
| **Segment** | Customers | 1+ purchases |
| **Segment** | Non-Purchasers | On list but never bought |
| **Segment** | Bought Outer Only | Cross-sell liner target |
| **Segment** | Bought Liner Only | Cross-sell outer target |
| **Segment** | Bundle Buyers | Referral programme target |
| **Segment** | Lapsed (90+ days) | Win-back flow target |

---

## P8A.14: DOMAIN, DNS & SSL

### P8A.14.1: Domain Setup

1. Purchase domain from Namecheap, Google Domains, or Cloudflare Registrar (~£10-15/year)
2. In Shopify: Settings → Domains → Connect existing domain
3. Add DNS records at your registrar:
   - A record: @ → 23.227.38.65
   - CNAME record: www → shops.myshopify.com
4. Wait 24-48 hours for propagation
5. Verify SSL auto-provisioned (padlock icon in browser)
6. Set primary domain to [brand].com (not [brand].myshopify.com)
7. Enable auto-redirect from www to non-www (or vice versa — pick one and be consistent)

### P8A.14.2: Email Setup

Options for hello@[brand].com:
- **Google Workspace** (£5.52/user/month) — professional, reliable, calendar included
- **Zoho Mail** (free for 1 user, 5GB) — budget option
- **Shopify Email Forwarding** — forwarding only, no sending

**Recommended: Google Workspace** for professionalism and reliability. One user is sufficient.

---

## P8A.15: SECURITY & FRAUD PREVENTION

### P8A.15.1: Shopify Built-In Security

Shopify handles: SSL/TLS encryption, PCI DSS compliance (Level 1), DDoS protection, server security, and automatic security updates. You don't need to manage any of this.

### P8A.15.2: Fraud Prevention

| Measure | Implementation | Cost |
|---|---|---|
| **Shopify Fraud Analysis** | Built into every order — shows risk indicators | Free (included) |
| **Shopify Flow fraud tag** | Auto-tag orders with different billing/shipping address | Free |
| **Address Verification (AVS)** | Enabled by default in Shopify Payments | Free |
| **3D Secure** | Enabled by default for UK/EU cards (Strong Customer Authentication) | Free |
| **Manual review** | Review any order flagged "High risk" before fulfilling | Your time |

### P8A.15.3: Fraud Decision Rule

For orders flagged "High risk" by Shopify:
1. Check if billing and shipping address match
2. Check if email looks legitimate (not random string @gmail.com)
3. Check if IP location roughly matches shipping address
4. For orders >£80: email customer to verify before shipping
5. When in doubt: cancel and refund. A £39 chargeback costs £39 + £15 Shopify dispute fee = £54 loss

### P8A.15.4: Account Security

- Enable 2FA on Shopify admin, Google account, Meta Business Suite, Klaviyo, and Wise
- Use a password manager (Bitwarden — free, or 1Password)
- Never share Shopify admin password — create staff accounts with limited permissions if needed

---

## P8A.16: BACKUP & DISASTER RECOVERY

### P8A.16.1: What Shopify Backs Up (And What It Doesn't)

Shopify automatically maintains: orders, customers, products, and financial data on their servers with redundancy. Shopify does NOT provide downloadable backups of your theme, pages, or blog content.

### P8A.16.2: What You Should Back Up

| Data | Frequency | How | Where |
|---|---|---|---|
| Theme code | Before any edit | Online Store → Themes → Duplicate | Shopify (duplicate theme) |
| Product data | Monthly | Settings → Export (CSV) | Google Drive |
| Customer data | Monthly | Customers → Export | Google Drive (encrypted) |
| Order data | Monthly | Orders → Export | Google Drive |
| Blog posts | After each post | Copy text to Google Docs | Google Drive |
| Images (originals) | Once | Keep originals on your computer/cloud | Google Drive |
| Klaviyo flows | After setup | Screenshot/document flow structure | Google Drive |
| Email templates | After creation | Export from Klaviyo | Google Drive |

### P8A.16.3: Disaster Scenarios

| Scenario | Impact | Recovery |
|---|---|---|
| Theme accidentally broken | Store looks wrong / crashes | Revert to duplicate theme (1 minute) |
| Product accidentally deleted | Lost listing | Re-import from CSV backup |
| Shopify account suspended | Store offline | Contact Shopify support (usually resolved in 24-48 hrs) |
| Domain expires | Store unreachable | Renew immediately + enable auto-renew |
| Email deliverability crash | Emails going to spam | Check DNS records, warm up sending domain |

---

## P8A.17: TECHNICAL LAUNCH CHECKLIST

### P8A.17.1: Complete Before Removing Password Page

- [ ] **Tracking:** GA4 firing on all pages (verify via DebugView)
- [ ] **Tracking:** Meta Pixel + CAPI on Maximum (verify via Pixel Helper)
- [ ] **Tracking:** TikTok Pixel installed and verified
- [ ] **Tracking:** Microsoft Clarity recording sessions
- [ ] **Tracking:** Google Search Console verified + sitemap submitted
- [ ] **Products:** All products have images, descriptions, prices, HS codes, weights
- [ ] **Products:** Bundle inventory sync tested (order a bundle → component inventory decreases)
- [ ] **Checkout:** Place test order using Shopify Bogus Gateway or real small order
- [ ] **Checkout:** Verify confirmation email sends correctly
- [ ] **Checkout:** Express checkout (Shop Pay, Apple Pay) working
- [ ] **Payments:** Shopify Payments activated with Wise bank details
- [ ] **Shipping:** UK and EU shipping zones configured with correct rates
- [ ] **Shipping:** Free shipping threshold (£40 UK) working at checkout
- [ ] **Tax:** VAT-inclusive pricing displaying correctly
- [ ] **Tax:** EU VAT rates correct in Shopify Markets (France 20%, Germany 19%)
- [ ] **Email:** Klaviyo connected, all pre-launch + post-launch flows active
- [ ] **Email:** SPF/DKIM/DMARC records verified (use mail-tester.com to check)
- [ ] **Legal:** Privacy policy, T&Cs, returns policy pages published
- [ ] **Legal:** Cookie consent banner active and functional
- [ ] **SEO:** All product pages have SEO titles and meta descriptions
- [ ] **SEO:** JSON-LD Schema markup verified (use Google Rich Results Test)
- [ ] **Mobile:** Tested on actual phone — all pages load correctly, Add to Cart works
- [ ] **Speed:** Lighthouse mobile score >80
- [ ] **Domain:** SSL certificate active (padlock icon)
- [ ] **Domain:** Redirect from www to non-www (or vice versa) working
- [ ] **Reviews:** Judge.me widget visible on product pages
- [ ] **Size guide:** Kiwi Sizing quiz working on product pages
- [ ] **Cross-sell:** "Complete Your System" recommendation showing on product pages
- [ ] **Announcement bar:** "Free UK Shipping Over £40" displaying

---

## P8A.18: P8A ACTION ITEMS

### P8A.18.1: Week 1 (Technical Foundation)

| # | Action | Cost | Priority |
|---|---|---|---|
| 1 | Configure Shopify store settings (P8A.1.2) | £0 | CRITICAL |
| 2 | Install Dawn theme + customise (P8A.2.2) | £0 | CRITICAL |
| 3 | Install all essential apps (P8A.3.1 — 12 apps) | £15/mo (Simple Bundles only) | CRITICAL |
| 4 | Set up GA4 via Google & YouTube channel | £0 | CRITICAL |
| 5 | Set up Meta Pixel + CAPI via Facebook & Instagram channel (Maximum mode) | £0 | CRITICAL |
| 6 | Install Microsoft Clarity | £0 | HIGH |
| 7 | Set up Google Search Console + submit sitemap | £0 | HIGH |
| 8 | Install TikTok Pixel via TikTok channel | £0 | MEDIUM |

### P8A.18.2: Week 2 (Content & Configuration)

| # | Action | Cost | Priority |
|---|---|---|---|
| 9 | Create all products with full data (P8A.10.1) | £0 | CRITICAL |
| 10 | Configure domain DNS (A record + CNAME) | £0 | CRITICAL |
| 11 | Set up Klaviyo DNS records (SPF/DKIM/DMARC) | £0 | CRITICAL |
| 12 | Create Klaviyo lists and segments (P8A.13.3) | £0 | HIGH |
| 13 | Set up CookieYes consent banner | £0 | CRITICAL |
| 14 | Configure shipping zones + rates | £0 | CRITICAL |
| 15 | Configure Shopify Markets (UK/EU/USD) | £0 | HIGH |
| 16 | Document UTM naming convention (P8A.9.1) | £0 | MEDIUM |

### P8A.18.3: Week 3 (Testing & Polish)

| # | Action | Cost | Priority |
|---|---|---|---|
| 17 | Run full technical launch checklist (P8A.17.1) | £0 | CRITICAL |
| 18 | Place test order → verify full flow (confirmation email, tracking, inventory) | ~£1 test order | CRITICAL |
| 19 | Test on mobile device (real phone, not emulator) | £0 | CRITICAL |
| 20 | Run PageSpeed Insights → fix any score <80 | £0 | HIGH |
| 21 | Verify all Klaviyo flows trigger correctly | £0 | HIGH |
| 22 | Back up theme (duplicate) before launch | £0 | HIGH |
| 23 | Set up Google Workspace email (hello@brand.com) | £5.52/mo | HIGH |

---

## P8A KEY INSIGHT

> **Install every tracking pixel BEFORE your first visitor arrives.** The pre-launch password page should already be collecting GA4 and Meta Pixel data from the moment you share the waitlist link. Every session without analytics is permanently lost intelligence — you can never retroactively track a visitor who came and left without being counted. The technical setup in this document takes 2-3 focused days to complete. Do it once, do it right, and never think about it again.

---

*P8A: Tech Infrastructure & Analytics — Complete Technical Setup Guide*
*Prepared March 2026 | Confidential*
