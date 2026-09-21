# Video Creation Guide — Idea to Publish (3-day cadence)

This is a stupid-proof, step-by-step checklist for producing one long-form video in roughly a 3-day window. Each mandatory step includes exact file paths and copy-paste snippets so the workflow is actionable immediately.

Quick action checklist (do in order)

 1. [ ] Pick & lock an idea
 2. [ ] Validate & write success criteria
 3. [ ] Script & shot plan (save to `content/scripts/`)
 4. [ ] Recording prep
 5. [ ] Record footage
 6. [ ] Edit & export
 7. [ ] Thumbnail & title finalization
 8. [ ] Publish
 9. [ ] Immediate post-publish record
 10. [ ] 7–21 day review

How to use this file

- Follow the numbered top-level items in order. Each top-level item contains mandatory drill-down steps (must do) and optional drill-downs (nice to do if time allows).
- Use `templates/VIDEO.md` and `templates/EXPERIMENT.md` for planning and experiment recording.
- After publishing, complete `templates/REVIEW.md` and copy learnings to `research/LEARNINGS.md`.

## 1) Pick and lock an idea (0.5 day)
Short description: choose a single idea and create a working script file.

### Mandatory
- [ ] 1.1 Open `content/IDEAS.md` and pick one IDEA to validate.

- [ ] 1.2 Add the idea to `content/BACKLOG.md`. Copy-paste and fill the block below:

```
- Working title: I Let 3 AI Agents Build the Same Laravel API
- Status: TODO
- Pillar: AI Coding Experiments
- Expected experiment: Compare outputs, measure fixes required
- Notes: Record side-by-side edits, show tests running
```

- [ ] 1.3 Create a working script file by copying `templates/VIDEO.md` into:

`content/scripts/YYYY-MM-DD-working-title.md`

Paste this minimal starter at the top of the new file (replace bracketed values):

```
Working title: [Working title]
Final title:
Status: TODO
Idea: [one-sentence idea]
Why someone should care: [one line]
Hook: [one sentence]
Success criteria:
- [e.g., CTR > 6%]
```

### Optional
- [ ] 1.4 If this is an experiment, create `content/experiments/YYYY-MM-DD-slug.md` from `templates/EXPERIMENT.md` and fill Hypothesis and Evidence fields.

---

## 2) Quick validation & success criteria (0.25 day)
Short description: confirm the idea has a clickable hook and measurable success metrics.

### Mandatory
- [ ] 2.1 Rewrite the `Hook:` in the script if it wouldn't attract a click from a stranger. Edit `content/scripts/YYYY-MM-DD-working-title.md`.
- [ ] 2.2 Add 1–2 measurable success criteria to the `Success criteria:` section (examples: "CTR > 6%", "Avg view duration > 4 minutes").

### Optional
- [ ] 2.3 Add a one-line competitor note to `research/COMPETITORS.md` if a public channel inspired the idea.

---

## 3) Script & shot plan (0.5 day)
Short description: write a focused script and a brief shot list with timestamps.

### Mandatory
- [ ] 3.1 Fill the script sections in `content/scripts/YYYY-MM-DD-working-title.md`: Hook, Setup, Experiment, Problems, Result, Learnings, Next Video.
- [ ] 3.2 Add a short shot list with timestamps and commit the file. Example:

```
[00:00] Hook — show failing test / problem
[00:20] Setup — explain codebase and hypothesis
[01:30] Experiment start — AI agents shown doing work
[06:00] Failures and fixes — human in the loop
[08:30] Result & Learnings
```

### Optional
- [ ] 3.3 Place one-slide visuals in a local `slides/` folder for reference during recording.

---

## 4) Recording prep (0.25 day)
Short description: prepare demos, audio and OBS for a smooth recording session.

### Mandatory
- [ ] 4.1 Put demo code in a demo repo or branch and remove all secrets.
- [ ] 4.2 Run an audio test and save it as `audio_test_YYYY-MM-DD.wav` locally.
- [ ] 4.3 Configure OBS scenes (editor, terminal, browser) and verify transitions.

### Optional
- [ ] 4.4 Record a 30s face intro clip if you plan to include one.

---

## 5) Record (0.5–1 day)
Short description: record short, clearly-named clips that map to the script timestamps.

### Mandatory
- [ ] 5.1 Record segments and name raw files: `slug_part01.mp4`, `slug_part02.mp4`, ...
- [ ] 5.2 Copy raw clips to a single folder and create `recording_index.txt` listing filenames and brief notes.
- [ ] 5.3 Save a copy of the final script in the same folder and note the demo repo link.

### Optional
- [ ] 5.4 Record a 30–60s vertical highlight for Shorts and save as `slug_short.mp4`.

---

## 6) Quick edit (0.5–1 day)
Short description: assemble the story, export captions, and produce the final MP4.

### Mandatory
- [ ] 6.1 Assemble footage to match the story structure. Keep edits tight.
- [ ] 6.2 Export captions (.srt) and store them alongside the final video.
- [ ] 6.3 Export final video as `slug-final-1080p.mp4` and save the editable project file locally.

### Optional
- [ ] 6.4 Add light music from YouTube Audio Library and minimal lower-thirds.

---

## 7) Thumbnail & title polish (mandatory before publish)
Short description: finalize title, create thumbnail and write the published record.

### Mandatory
- [ ] 7.1 Set `Final title:` in `content/scripts/YYYY-MM-DD-working-title.md`.
- [ ] 7.2 Create thumbnail `thumbnails/YYYY-MM-DD-slug.png` (1280×720); keep the layered source locally.
- [ ] 7.3 Create `content/published/YYYY-MM-DD-slug-published.md` with this template and fill it:

```
Title: [Final title]
Published: [YYYY-MM-DD]
Thumbnail: thumbnails/YYYY-MM-DD-slug.png
Script: content/scripts/YYYY-MM-DD-working-title.md
Description: [First 2–3 lines]
Notes: [short publishing notes]
```

### Optional
- [ ] 7.4 Create a 30s social teaser and save under `content/shorts/`.

---

## 8) Publish checklist (mandatory on publish day)
Short description: upload, set metadata, and add analytics placeholders.

### Mandatory
- [ ] 8.1 Upload or schedule the video on YouTube. Paste Final title and the description from the published record.
- [ ] 8.2 Include demo repo links and a link to the `content/published/` record in the YouTube description.
- [ ] 8.3 Set playlist, tags, visibility, language and upload the thumbnail.
- [ ] 8.4 Post a pinned comment with key links and a CTA.
- [ ] 8.5 Add an analytics placeholder row to `analytics/DASHBOARD.md`. Paste this example into the Video table:

```
| # | video | publish date | pillar | views | impressions | CTR | average view duration | % viewed | subscribers gained | revenue | notes |
|---|---|---:|---|---:|---:|---:|---:|---:|---:|---:|
| 1 | [Final title] | YYYY-MM-DD | [Pillar] | - | - | - | - | - | - | - | - |
```

### Optional
- [ ] 8.6 Share the Short/teaser and full video link on social platforms.

---

## 9) Immediate post-publish steps (same day)
Short description: archive published assets and capture initial review facts.

### Mandatory
- [ ] 9.1 Ensure `content/published/YYYY-MM-DD-slug-published.md` exists and contains title, thumbnail and description.
- [ ] 9.2 Create a draft review: open `templates/REVIEW.md`, paste Title, Publish date and Thumbnail, then save as `analytics/videos/YYYY-MM-DD-slug-review.md`.

### Optional
- [ ] 9.3 Add a short entry to `research/LEARNINGS.md` with the publishing hypothesis.

---

## 10) 7–21 day review and iterate (mandatory within 3 weeks)
Short description: use real metrics, record learnings and choose the next step.

### Mandatory
- [ ] 10.1 Complete `templates/REVIEW.md` with real metrics (CTR, AVD, subscribers gained) and save to `analytics/videos/YYYY-MM-DD-slug-review.md`.
- [ ] 10.2 Add a `research/LEARNINGS.md` entry using the template (Date, Observation, Evidence, Hypothesis, Action, Confidence) and link the review.
- [ ] 10.3 Update `content/BACKLOG.md` to reflect follow-up, repeat, or retire decisions.

### Optional
- [ ] 10.4 If product demand appears, add a note to `products/IDEAS.md` with links to the review and evidence.

---

## Minimum publishing metadata to record (must do)

- Final title
- Short description (first 2–3 lines)
- Published date/time
- Thumbnail filename
- Playlist
- One-line hypothesis you tested

## Practical timing guide (3-day example)

- Day 0: Idea selection, validation, script & experiment template (items 1–4).
- Day 1: Record all footage (item 5) and start basic assembly.
- Day 2: Edit, finalize thumbnail/title, publish and do immediate post-publish steps (items 6–9).
- Day 3–21: Collect data, review and iterate (item 10).

## Small but critical rules (repeat often)

- Keep experiments time-boxed; if an experiment will take more than 2 weeks, split into smaller publishable chunks.
- Sanitize secrets and never publish private credentials.
- Do not over-polish early videos; validation comes from audience signals.
- Always separate facts (metrics) from interpretation in `templates/REVIEW.md` and `research/LEARNINGS.md`.

## Quick links (use these files)

- Planning template: `templates/VIDEO.md`
- Experiment template: `templates/EXPERIMENT.md`
- Post-publish review: `templates/REVIEW.md`
- Ideas: `content/IDEAS.md`
- Backlog: `content/BACKLOG.md`
- Published scripts: `content/published/`
- Learnings: `research/LEARNINGS.md`
- Thumbnails guidance: `research/THUMBNAILS.md`
- Titles guidance: `research/TITLES.md`
- Analytics dashboard: `analytics/DASHBOARD.md`
- Product ideas: `products/IDEAS.md`

If anything in this checklist is unclear, update this file directly so the process remains the single source of truth for your workflow.
