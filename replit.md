# AB Paving Glasgow — Replit Project

## Overview
A React + Vite + TypeScript frontend website for AB Paving Glasgow, a block paving driveways and landscaping company serving Glasgow and surrounding areas. Built as a local SEO lead-generation site.

## Tech Stack
- **Frontend**: React 18, TypeScript, Vite
- **Styling**: Tailwind CSS, shadcn/ui components
- **Routing**: React Router v6
- **Forms**: React Hook Form + Zod
- **Email**: @emailjs/browser (Service ID: `service_abpaving`, Template ID: `template_quote`)
- **State/Data**: TanStack React Query
- **Icons**: lucide-react

## Contact Details
- **Phone**: 07432 421 978 (tel: 07432421978)
- **Public email**: akerr.pog@gmail.com
- **Customer email** (form recipient): abpavingltd@gmail.com
- **EmailJS public key**: set as Replit secret `VITE_EMAILJS_PUBLIC_KEY`

## Design System
- **Brand colours**: Navy (primary), Orange (accent) — do NOT change
- **Display font**: Montserrat
- **Body font**: Open Sans
- **Logo**: `src/assets/logo.png`
- **Favicon**: `public/favicon.png`

## Project Structure
```
src/
  pages/
    Index.tsx           — Homepage (hero, services, areas grid, blog/guide cards, reviews, CTA)
    About.tsx
    BlockPavingDriveways.tsx
    ResinDriveways.tsx          — /resin-driveways-glasgow
    PatiosSlabbing.tsx
    LandscapingPage.tsx
    GardenTransformations.tsx
    Gallery.tsx
    Reviews.tsx
    Contact.tsx                 — /contact (quote form, contact info, Google Maps embed)
    PrivacyPolicy.tsx           — /privacy
    Terms.tsx                   — /terms
    NotFound.tsx
    locations/
      LocationPage.tsx          — Reusable template for all location pages
      Giffnock.tsx              — /driveways-giffnock (G46)
      NewtonMearns.tsx          — /driveways-newton-mearns (G77)
      Clarkston.tsx             — /driveways-clarkston (G76)
      Thornliebank.tsx          — /driveways-thornliebank (G46)
      Barrhead.tsx              — /driveways-barrhead (G78)
      Bearsden.tsx              — /driveways-bearsden (G61)
      Milngavie.tsx             — /driveways-milngavie (G62)
      Shawlands.tsx             — /driveways-shawlands (G41)
    projects/
      BlockPavingNewtonMearns.tsx  — /projects/block-paving-driveway-newton-mearns
      PatioGiffnock.tsx            — /projects/patio-installation-giffnock
    blog/
      DrivewayCostGlasgow.tsx              — /driveway-cost-glasgow (2025 guide)
      BlockPavingVsResin.tsx               — /block-paving-vs-resin-driveways
      HowLongDoBlockPavingDriveways.tsx    — /how-long-do-block-paving-driveways-last
      DrivewaySigns.tsx                    — /5-signs-driveway-needs-replacing
  components/
    SiteHeader.tsx      — Sticky nav with Services + Areas dropdowns, top bar, mobile menu
    SiteFooter.tsx      — Full footer (orange CTA banner, services, areas, contact, legal links)
    SchemaMarkup.tsx    — JSON-LD LocalBusiness + Review structured data
    PageCTA.tsx         — Reusable quote CTA section
    QuoteForm.tsx       — EmailJS-connected quote form (loading spinner, error handling, success state)
    ServiceCard.tsx
    ReviewCard.tsx
    NavLink.tsx
    ui/                 — shadcn/ui components
  assets/
    logo.png            — AB Paving & Landscaping logo
    hero-driveway.jpg
    service-*.jpg
    before/after-driveway.jpg
    team-working.jpg
    gallery-collage.jpg
```

## Route Table
| Path | Component |
|------|-----------|
| `/` | Index |
| `/about` | About |
| `/block-paving-driveways` | BlockPavingDriveways |
| `/resin-driveways-glasgow` | ResinDriveways |
| `/patios-slabbing` | PatiosSlabbing |
| `/landscaping` | LandscapingPage |
| `/garden-transformations` | GardenTransformations |
| `/gallery` | Gallery |
| `/reviews` | Reviews |
| `/contact` | Contact |
| `/privacy` | PrivacyPolicy |
| `/terms` | Terms |
| `/driveways-giffnock` | Giffnock |
| `/driveways-newton-mearns` | NewtonMearns |
| `/driveways-clarkston` | Clarkston |
| `/driveways-thornliebank` | Thornliebank |
| `/driveways-barrhead` | Barrhead |
| `/driveways-bearsden` | Bearsden |
| `/driveways-milngavie` | Milngavie |
| `/driveways-shawlands` | Shawlands |
| `/projects/block-paving-driveway-newton-mearns` | BlockPavingNewtonMearns |
| `/projects/patio-installation-giffnock` | PatioGiffnock |
| `/driveway-cost-glasgow` | DrivewayCostGlasgow |
| `/block-paving-vs-resin-driveways` | BlockPavingVsResin |
| `/how-long-do-block-paving-driveways-last` | HowLongDoBlockPavingDriveways |
| `/5-signs-driveway-needs-replacing` | DrivewaySigns |

## Development
- Run: `npm run dev` (configured as "Start application" workflow)
- Build check: `npm run build`
- No backend/database — pure frontend static site
- EmailJS public key must be set as Replit secret `VITE_EMAILJS_PUBLIC_KEY`

## Notes
- Social links (Facebook/Instagram) use placeholder URLs — user should update to real profile URLs
- Google Maps embed on Contact page shows general Glasgow area
- All location pages use the `LocationPage.tsx` template component for consistency
