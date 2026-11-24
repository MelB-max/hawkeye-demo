# HAWKEYE · mock call portal (demo)

**Live demo:** https://melb-max.github.io/hawkeye-demo/ · click **New starter** or **Admin** on the sign-in card. No sign-up, nothing is sent anywhere.

HAWKEYE is where coaches score practice calls and new starters see their feedback. This repo is a **static demo of the interface and navigation**, dressed as "Halcyon", a made-up marketing agency practising client pitch calls. The scorecard, people, scores and AI answers are all fictional and canned in the browser.

## What to look at
- **Landing:** a night-sky board with live-looking numbers: calls this month, first-try pass rate, criteria pulse, by discipline.
- **Home:** the pitch-call journey in one frame, with a swarm of pixel blobs that gathers around whichever step you point at.
- **Practice a pitch call:** an AI plays a prospective client; practise one phase or the whole call, typing or speaking, then get scored with a better line for each fix.
- **Scoring:** an eight-criterion scorecard that adapts to role and discipline, looks up the new starter, and emails them the result.
- **My score:** every call with a round filter, score trend, the criteria holding you back, and **HAWKEYE's take** (an AI summary of each call) plus **Ask HAWKEYE**, an AI coach that answers from your own scorecards.
- **Scoring guide:** what each criterion checks, what good sounds like, common misses, averages by discipline and role.
- **View as a new starter (admins):** see anyone's scores, HAWKEYE's take and the coach exactly as they do.
- **Settings (admins):** email templates with placeholders, CC rules per round, Slack messages, weekly digest, AI coach and practice limits, access control.

## Built with
Plain HTML, CSS and JavaScript. In production: a Cloudflare Worker serves the site and runs the AI coach on Cloudflare Workers AI (Llama 3.3 70B), with Google Apps Script and Sheets behind it.
