# ScholarSaathi – Smart Scholarship Finder

> No student should miss an opportunity due to lack of information.

Built for **Innovate India Hackathon 2026** (Round 2) by Shailender Kumar Suman.

**Live demo:** https://shailender-kumar-suman.github.io/ScholarSaathi/

## What it does
- Takes a one-time student profile (course, year, state, gender, category, income, marks, minority and disability status).
- Marks each scholarship as "may be eligible" or "not matching yet" and explains **which rule failed**.
- Shows whether the 2026-27 application window is open or closed.
- Lists the documents to keep ready for each scholarship.
- Lets students save a shortlist with their own apply-by dates and see days left.
- No login. All data stays in the student's own browser (localStorage).

## Tech
HTML, CSS and plain JavaScript in a single file (`index.html`). No build step, no dependencies.

## Run it
Download `index.html` and double-click it. It opens in any modern browser.

## Add a scholarship
Open `index.html`, find the `DATA` list and copy one entry. Fill in:
`id, name, by, amt, courses, gender / cats / minority / disability / years / top20 (only if the rule applies), maxInc, minMarks, link, note, end, win, src`.

## Data and verification
Only schemes checked against the National Scholarship Portal (NSP) and public notices are listed. Each card shows the check date and source. Currently: AICTE Pragati, AICTE Saksham, PM-USP Central Sector Scholarship (CSSS), UGC National Scholarship for PG Studies, Punjab Post Matric Scholarship for SC students, PM YASASVI Post Matric (OBC/EBC/DNT). State-specific rules are supported (Punjab first); other states can be added as data.

Known uncertainty: the CSSS income limit appears as ₹4.5 lakh in the scheme description and ₹8 lakh in one 2026-27 article. The app uses ₹4.5 lakh and asks students to confirm on NSP.

## Limitations
Eligibility shown here is a guide, not a guarantee. The scholarship provider makes the final decision. Rules and dates change every year, so always confirm on the official portal.

## Roadmap
More verified scholarships (central, Punjab, private), AI-assisted plain-language summaries of notices, Hindi and Punjabi support, deadline reminders, an admin screen.
