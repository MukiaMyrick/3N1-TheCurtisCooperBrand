# 3N1 Business Hub — Implementation Guide

**Contact:** Teamcurtis31@gmail.com

## What this package actually provides
- `index.html`: interactive LOCAL demo dashboard with lead stages, booking requests, draft estimates/invoices, contract starter templates, social draft planner, and Chris/Chloe scripts.
- `website.html`: existing public-facing 3N1 website prototype with Curtis's photo and four service photos.
- `assets/logo.png`: 3N1 logo.
- `IMPLEMENTATION_GUIDE.md`: production setup roadmap.

**Important:** The dashboard uses browser localStorage, not a secure CRM database. It is not suitable for real customer data, shared access, or regulated information. No live booking, shared inbox, sending, payment processing, e-signature, AI chat, voice calling, social publishing or mobile app store deployment is active. Do not use the demo to store sensitive data.

## Recommended production stack
1. **Website and bookings:** Wix + Wix Bookings (or Square Appointments for salon staff), with separate service pages and a master Google Calendar. Avoid double-booking by verifying synchronization and staff calendars.
2. **CRM:** Wix Contacts/Automations for simplest setup; or HubSpot CRM if more robust pipelines are needed. Use divisions: Barber; Real Estate & Investing; DJ/Entertainment; Consultation Services.
3. **Inbox:** Google Workspace shared inbox / delegated mailbox or a CRM-connected team inbox, with Teamcurtis31@gmail.com as the contact. Confirm ownership and authorization before connecting.
4. **Payments:** Wix Payments or Stripe/Square through a compliant integration. Never store credit card details in the demo.
5. **Contracts:** Lawyer-reviewed templates + DocuSign or Dropbox Sign, using access controls and signed audit trails. Real estate paperwork must use broker-approved forms and required disclosures.
6. **Reminders and lead follow-up:** Booking platform confirmation/reminder tools and CRM workflows, with consent and opt-out controls for marketing texts/emails.
7. **Chris Chat AI:** Website chat vendor or CRM AI assistant connected to approved FAQs and booking flows. Require human escalation, privacy disclosures and testing.
8. **Chloe Voice AI:** Select a phone/voice AI vendor, verify number ownership, disclosure, call transfer, recording/consent rules and fallback routing. Test before turning on 24/7.
9. **Social:** Meta Business Suite for Facebook/Instagram; connect TikTok or LinkedIn separately if needed. Draft approval workflow before publishing.
10. **Apple/Android app:** Start with mobile-first website/PWA; native apps require separate builds or app-builder, store accounts, privacy policy, secure login and store approval.

## Lead stages by service
- Barber: New inquiry → Appointment requested → Staff assigned → Confirmed → Completed → Follow-up.
- Real estate: New inquiry → Buyer/Seller/Investor identified → Qualified → Consultation scheduled → Broker handoff → Active client → Closed / Nurture.
- DJ/Events: New inquiry → Event details collected → Availability checked → Quote sent → Agreement/deposit → Confirmed → Completed.
- Consultation: New inquiry → Scope confirmed → Scheduled → Paid (if applicable) → Completed → Follow-up.

## Example follow-up workflows
- **Immediate:** acknowledge the inquiry, identify the service, notify the assigned person.
- **After 24–48h:** one helpful follow-up if unbooked and not replied; do not send if opted out.
- **After confirmed booking:** send date/time/location or meeting link and cancellation policy.
- **24h before:** appointment reminder if customer opted into that channel.
- **After appointment:** request feedback, with appropriate consent.

## Required decisions before live activation
- Curtis's business phone, physical service locations, hours and staff schedules.
- Confirmed booking platform, live URLs, durations, cancellation and deposit policies.
- Service menus and prices; DJ package/quote rules; consultation scope and price.
- Brokerage name, license and legal disclosures for real estate.
- Authorized team members, roles and permissions; privacy policy and terms.
- Contract review and e-signature provider; payment processor and banking ownership.
- AI FAQ approvals, prohibited claims, transfer rules, and consent to messaging/recording.
- Whether app means installable website or native App Store / Play Store apps.

## How to preview
Unzip the package and open `index.html` in Chrome. Use the navigation tabs. Open `website.html` for the public site. Data in the dashboard remains local to the browser, so clearing browser storage removes it.


## Testimonials
The testimonials.html page is linked in the main site navigation. The submission form creates a draft email to Teamcurtis31@gmail.com; it is not a hosted form or a public review database. Only publish real reviews with consent.
