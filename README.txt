StartcomAI website  (two verticals)

FILES
  index.html               Products: Voice, SMS, RCS, WhatsApp, AI Voice Bot
  digital-marketing.html   Digital Marketing: SEO, Website building, Ads and social, OBD/IVR
  favicon.svg, favicon.ico, apple-touch-icon.png   browser tab and home-screen icons

Each page is fully self-contained: all styling and scripts are inside the HTML file, so it
displays correctly even if opened on its own. Keep both pages in the same folder so the
Products | Digital Marketing switcher and cross-links work. The icon files are optional
(the tab icon is also embedded in each page).

PREVIEW   Double-click index.html, or run:  python -m http.server 8000
DEPLOY    Upload all 5 files to any static host (Netlify, Cloudflare Pages, GitHub Pages). No build step.

EDIT BEFORE LAUNCH  (search for "CONFIG" near the top of the <script> in BOTH pages)
  CONTACT_EMAIL   placeholder hello@startcom.ai - set your real inbox
  LEAD_ENDPOINT   URL that accepts a JSON POST (Formspree, Netlify Forms, your API). Empty = the
                  form opens the visitor's email app. Each lead includes "vertical" (products|marketing).
  CONSOLE_URL     your customer console URL. Empty = Login opens "request access".

BRAND
  Logo artwork is a vector redraw of the StartcomAI robot mascot (header, dashboard sidebar, footer).
  The browser-tab favicon uses a simplified head so it stays readable at 16px; apple-touch-icon.png
  uses the full mascot. If you have the official logo as an SVG with a transparent background,
  replace the <symbol id="mark"> block near the top of each page with it.
  Wordmark: heavy italic "Startcom" + cyan-to-purple gradient "AI". Tagline in the footer:
  "Powering Intelligent Communication".

STILL TO CREATE   privacy.html and terms.html (linked from the footer and the form consent line).

AI VOICE BOT  (new product, Products page: strip card, #voicebot section, nav, footer, developer sample,
              compliance checker group, three industry journeys, FAQ)
  - The section shows a live call you can play as the customer: 3 scenarios (admissions callback, EMI
    reminder, site-visit booking) x 3 languages (English, Hindi, Hinglish) x every reply path.
    Scenarios use fictional businesses and SAMPLE data; they are scripted, not a real speech engine.
  - Positioning is based on market research (Indian voice-AI vendors, buyer use cases, TRAI/RBI/DPDP rules)
    and on the capabilities VIH Metaverse describes for its Shruti voice bot (real-time speech AI, custom
    bots per business, inbound and outbound, scheduling/reminders/collections, live dashboards).
    The page does NOT use the VIH or Shruti name or copy. If you will resell or white-label Shruti
    (or any engine), confirm the commercial terms and branding rights first.
  - Claims to verify before launch: languages offered, real-time/low-latency behaviour, interruption handling,
    human handoff, CRM and dashboard features, mid-call WhatsApp/SMS, call recording and summaries, and
    "the bot says it is automated at the start of every call".
  - The AI Voice Bot API shown (/v1/voicebot/calls) is illustrative, like the other API samples.
  - Compliance copy (140 series, DND, 8 AM to 7 PM recovery window for lenders, DPDP) reflects Oct 2026
    guidance from public sources that differ in places. Have your compliance lead review it.

PRICING
  No prices, plans, rates, fee estimators or "free" offers are shown anywhere on the site. Pricing is
  agreed directly with each customer. "Get a quote" buttons and the contact form are the only pricing
  touchpoints. Example copy inside the demos (e.g. a fictional clinic's "free consultation") belongs to
  the fictional customer, not to StartcomAI.

VERIFY BEFORE LAUNCH
  - Every capability described is what you intend to deliver; remove anything you cannot.
  - "24/7 support" (hero) and "you own the domain, hosting and ad accounts" are commitments to confirm.
  - Dashboards, charts, feeds, simulators and planners use SAMPLE data and are labelled so.
  - The API shown in the Developers section is illustrative (api.startcom.ai does not exist yet).
  - Compliance copy reflects Oct 2026 (TRAI DLT, 140/1600 series, TCCCPR Feb 2025, DPDP Rules).
    Have your compliance lead review it. Add legal name, address and registrations to the footer.

NOT CONNECTED (needs real engineering)
  Accounts and login, carrier/provider APIs, dialer and campaign engine, billing, API keys,
  lead storage/CRM, consent logging, monitoring.
