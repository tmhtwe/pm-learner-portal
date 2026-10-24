# PM Learner Portal

Tin's learner portal for a weekend product management cohort, the way HelloPM works: lessons week by week, a Saturday live class, a Telegram group and progress tracking. For now it's an MVP that only Tin uses.

## What's here

| Path | What it is |
|---|---|
| `index.html` | **The portal website** (mobile-first, no build step). Served by GitHub Pages. |
| `data/course.json` | **All course content** the website shows: settings, weeks 0–16 and lessons. Edit this to add lessons. |
| `portal/index.html` | The claude.ai version of the portal (with edit mode and the private HelloPM library). |
| `data/weeks/` | Weeks 0–16 of the course outline |
| `data/lessons/` | Lessons (title, type, minutes, link, note, week) |
| `data/settings/` | Course name, start date, class time, live class, recordings and Telegram links |

`data/weeks/`, `data/lessons/` and `data/settings/` are exports from the claude.ai version. The website reads only `data/course.json`.

## Adding a lesson

Add an entry to `lessons` in `data/course.json`:

```json
{ "id": "w01-intro", "week": 1, "order": 1, "title": "What a PM does", "kind": "watch", "mins": 12, "url": "https://youtube.com/...", "note": "" }
```

`kind` is one of `watch`, `do`, `discuss`, `attend` or `read`. Progress ticks are saved in each visitor's browser.

## Not in this repo

- **Learner data.** Progress and any personal details are never committed.
- **The HelloPM archive.** It lives in the private repo `tmhtwe/hellopm-archive` (lesson viewer, documents and index) and in Google Drive. It is never published here.
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
