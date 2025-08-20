# VETSTOR Interview Assignment
## Interview Process
1. Take‑home screening assignment (1–2h)
2. Screening interview (CPO or HR, ~15m)
3. Technical interview (CTO, 1–2h)
4. Final chat (CEO, ~20m)

## The Assignment (2 parts)
We simulate a realistic product request. The product goal is clear; the details are up to you. We value clarity, simplicity, and execution.

### Part 1 — Planning (tickets breakdown)
- Product manager asks for extracting and saving data from existing provided health records: vaccinations and castration. We need to save the extracted data for later usage and display them in the React app. Build extraction pipeline which will work on many different health records, latin words and doctor shortcuts. Pipeline will save data in place and structure of your choice. Then Build a React + TypeScript app with basic UI reading from your data store.
- You have read‑only access to a Supabase Postgres database (details below).
- Your task: Help product manager break down the problem to multiple tickets. Just titles, maybe short description.  
- Deliver your ticket stubs in `Task_1_result.md`.

Note: Part 1 includes both vaccinations and castration. In Part 2 you will implement vaccinations only.

### Part 2 — Implementation (vaccinations only)

1. A list page: show animal IDs with the latest vaccination date (each item links to the detail page).
2. A detail page: show all vaccinations for a given animal.

Technologies, frameworks, hosting and approach, all is completely up to you.

#### Must‑haves
- Read from Supabase
- Use React + TypeScript
- Store the parsed data
- Present them in React app

#### Deliverables
- `Task_1_result.md`: Problem break down for Part 1
- Working app (code in a public repo; fork or your own)
- Deployed URL we can click and test
- Short write‑up of decisions/assumptions in `Task_2_comments.md` (or your README)
- Email the repo link and app URL to jan -at- vetstor.com

#### Recommendations
- Keep it simple; choose tools appropriate for the job
- Feel free to use AI tools and free tiers where helpful
- Deploy whenever it’s useful for you

#### Timebox
- Aim for 1–2 hours max. It’s fine to ship a focused slice that shows your approach and explain where would you go from there.

---

## Data Access (read‑only)
Supabase project URL:

```
https://vmmbjfycdefakulnyzhl.supabase.co
```

Anon key (assignment‑scoped):

```
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InZtbWJqZnljZGVmYWt1bG55emhsIiwicm9sZSI6ImFub24iLCJpYXQiOjE3NTU1OTQ3NDAsImV4cCI6MjA3MTE3MDc0MH0.GrkUW60Hm4vj68zazse1H1GIyg9A-hNx5CPYHpmM_nE
```

Treat the key as public and limited to this assignment. Use it only for reading data.

Look at scripts/readData.ts how to read source.

---

## Evaluation Criteria
- Correctness (vaccination extraction approach, latest date logic, handling missing/duplicate/edge cases)
- Code quality (readability, structure, types, tests)
- Simplicity (avoid unnecessary complexity)
- Clarity of tickets/spec (assumptions, acceptance criteria, dependencies)

What we are not evaluating: pixel‑perfect UI, heavy infra, or complete production hardening.

---

## Getting Started (optional guidance)
- You can scaffold with your preferred tool (Just must be React + TypeScript) and deploy to any cloud host
- Document your assumptions and decisions in `Task_2_comments.md`.

Good luck—and have fun. Keep it focused and pragmatic.