# PM Learner Portal

Tin's learner portal for a weekend product management cohort, the way HelloPM works: lessons week by week, a Saturday live class, a Telegram group and progress tracking. For now it's an MVP that only Tin uses.

## What's here

| Path | What it is |
|---|---|
| `portal/index.html` | The portal page (mobile-first, no build step). Published privately on claude.ai. |
| `data/weeks/` | Weeks 0–16 of the course outline |
| `data/lessons/` | Lessons (title, type, minutes, link, note, week) |
| `data/settings/` | Course name, start date, class time, live class, recordings and Telegram links |

The live data is in the claude.ai artifact's database. The files in `data/` are exports of it.

## Not in this repo

- **Learner data.** Progress and any personal details are never committed.
- **The HelloPM archive.** It stays private in Google Drive (HelloPM › Website). The portal's Library tab reads it live, and only Tin can see it.
- **Videos.** These stay in Google Drive (and later Bunny Stream or Mux), because GitHub rejects files over 100 MB.

## Course shape

| Weeks | Focus |
|---|---|
| 0 | Onboarding, tools, meet the cohort |
| 1–4 | Discovery and user research |
| 5–8 | Prioritisation, roadmaps, specs |
| 9 | Catch-up week |
| 10–13 | Metrics, experiments, working with engineers |
| 14–16 | Portfolio project, CV, mock interviews |

Live class: Saturday 9:30am Yangon · 10:00am Bangkok · 4:00pm Auckland (NZ summer).

## Roadmap

- Phase 0 (now): private MVP for Tin
- Phase 1, cohort 1: simple portal with lesson links, no logins
- Phase 2, cohort 2 onwards: Supabase with logins and progress, Burmese-first with a language switcher, low-data mode
