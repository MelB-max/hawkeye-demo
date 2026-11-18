# HAWKEYE · mock call portal (demo)

**Live demo:** https://melb-max.github.io/hawkeye-demo/ · click **Trainee** or **Admin** on the sign-in card. No sign-up, nothing is sent anywhere.

HAWKEYE is where trainers score practice sales calls and trainees see their feedback. This repo is a **static demo** of the interface: the company ("Kestrel Academy"), people, scores and AI answers are made up and canned in the browser.

## What to look at
- **Landing:** a night-sky board with live numbers: calls this month, first-try pass rate, criteria pulse, by program.
- **Scoring:** a 12-criterion scorecard that adapts to role and program, looks up the trainee, and emails them the result.
- **My score:** every call with a round filter, score trend, the criteria holding you back, and **HAWKEYE's take** (an AI summary of each call) plus **Ask HAWKEYE**, an AI coach that answers from your own scorecards.
- **Evaluation metrics:** what each criterion checks, what good sounds like, common misses, live averages by program and role.
- **Settings (admins):** email templates with placeholders, CC rules per round, weekly digest, AI coach limits, access control.

## Built with
Plain HTML, CSS and JavaScript. In production: a Cloudflare Worker serves the site and runs the AI coach on Cloudflare Workers AI (Llama 3.3 70B), with Google Apps Script and Sheets behind it.
