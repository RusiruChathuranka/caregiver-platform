# Kindred Care

A colorful, responsive caregiver coordination dashboard concept for Sri Lanka.

## What's included

- Responsive admin dashboard with summary cards, recent care requests, caregiver network, upcoming placements, and review reminders.
- Care request form with basic client-side validation and generated reference IDs.
- Care request management with search, status filters, and editable request statuses.
- Caregiver directory with search, availability filters, and a demo add-caregiver flow.
- Booking and shift overview.
- Blog/resource manager with draft/publish state and a simple editor flow.
- Family/patient list, illustrative reports, and workspace settings.
- Responsive navigation, modal interactions, toast feedback, and accessible form labels.

## Run locally

This is currently a **static frontend prototype** using illustrative data in browser memory. It does not yet connect to a database, authentication provider, email/WhatsApp messaging, or private document storage. Changes are not persisted after a page reload. Do not enter real patient details or sensitive personal information.

You can open `index.html` directly, or run a local static server:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy with GitHub Pages

1. Open this repository on GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch `main` and folder `/ (root)`, then save.
5. Wait for GitHub Pages to publish the site.

Alternatively, the included workflow deploys the static site through GitHub Actions after it is enabled in the repository's Pages settings.

## Before production

This prototype is not a production booking system. Before handling real requests, add:

- Authentication and role-based access controls.
- PostgreSQL-backed persistence and server-side validation.
- Private storage for identity and qualification documents.
- Carefully designed authorization policies and audit logs.
- Consent, privacy, retention, and incident-handling processes.
- Verified caregiver screening workflows.
- Secure notification integrations and tested backup/recovery.

Suggested next stack: React + TypeScript + Tailwind CSS, with Supabase/PostgreSQL or a dedicated API backend. Keep private patient/caregiver data off public pages and never put service secrets in browser code.
