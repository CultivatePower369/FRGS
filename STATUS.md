# Project Status

Last updated: 2026-08-07 (Rules & Regulations page — Phase 1)

## Session note — 2026-08-07
Built the new `rules.html` page (Rules & Regulations, Phase 1: sections 01–04 — Match Outcomes, Scoring, Penalties & Stalling, Match Lengths). Sections 05–09 listed in the on-page index as "Coming Soon," no content yet. Added "Rules" to nav and footer on every existing page, and replaced the outdated "IBJJF for Gi / EBI for No-Gi" line on the FRGS Open event card in `events.html` with a "View Competition Rules" button linking to the new page. Design reuses the site's existing components (page-header, red-bar, card patterns) — no new visual system introduced. Legal & Illegal Techniques (Phase 2) not started.

Last updated: 2026-07-06 (pipeline check-in)

## Pipeline check — 2026-07-06
Resuming after a ~month gap. Verified: local repo clean and in sync with origin/main, deploy.yml workflow intact, last GitHub Action run (2026-06-05) succeeded. Pushing this note to confirm the GitHub Action → deploy branch pipeline still fires correctly before resuming real work.

Last updated: 2026-06-03 (end of session)

## Current step
**Step 7 — Set Up GoHighLevel Tags, Forms, Links, and Tracking Fields**
In progress. Working through GHL workflows.

### Workflows — completed
- Spectator tickets

### Workflows — remaining
- Sponsor inquiry
- Sponsor confirmed and paid
- Volunteer inquiry
- Employee
- Mat coordinator
- Referee onboarding
- Post-event follow-ups

## Completed steps

| Step | Description | Notes |
|---|---|---|
| 1 | Lock the Tournament Definition | Done. See locked details below. |
| 2 | Finalize Rules and Division Structure | Done. Set up in Smoothcomp. |
| 3 | Set Up Smoothcomp Event Draft | Done. Details, pricing, deadlines, payments all locked in. |
| 4 | Test Registration and Payment Flow | Done. Full test run completed. Competitors can register, pay, receive confirmation, and appear in Smoothcomp. |
| 5 | Create the Official Event Information Hub | Done. Live at featherrivergrappling.com. |
| 6 | Publish the Tournament Registration Page | Done. Live on Smoothcomp. Flow: buy membership → receive coupon code via email → register on Smoothcomp with discount code. |

## Locked event details

- **Tournament name:** Feather River Grappling Series
- **Date:** November 14, 2026
- **Venue:** Oroville Convention Center
- **Skill levels:** All skill levels
- **Age groups:** 5 and up
- **Website:** featherrivergrappling.com
- **Registration flow:** GHL membership purchase → coupon code email → Smoothcomp registration with discount

## What's next after Step 7

Step 8 — Build the Participant Communication System (email/SMS templates)
Depends on Step 7 being fully connected and tested (Step 9 connects and tests the workflows).

## Open issue — sponsor-confirmed.html redirect not working
`sponsor-confirmed.html` was created, committed, and pushed to GitHub (commit eda7643). Deployed to Cloudways. Page is not loading correctly — redirecting to home page instead. Root cause unknown. Need to diagnose on next session. Possible causes: Cloudways routing/redirect rule, .htaccess, or GHL redirect URL misconfigured.

## Blockers
- sponsor-confirmed.html redirect broken — needs diagnosis next session.
