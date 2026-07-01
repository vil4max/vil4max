# Agent brief: `vil4max.github.io`

Copy this file to another agent or open on iPhone to copy sections.

**Repo:** https://github.com/vil4max/vil4max.github.io  
**Base branch:** `main`  
**Feature branch:** `cursor/resume-ats-highlight-64a1` (create from `main`)

## Context

Profile review is done. The `vil4max` repo is updated in PR #2 (README without phone, PDFs regenerated). The site repo is behind.

**Workflow (from `constraints.md`):** edit `content/resume-source.json` first → sync HTML in the same session → `npm run resume:validate` → `npm run resume:pdf:all`.

---

## Commit 1: `fix(resume): anchor early career to Dec 2013 start date`

First job: **December 2013**. Headline everywhere: **12+ years** (not 10+).

### `content/resume-source.json`

- `roles[early-career].displayFull` → `Dec 2013 – May 2017`
- `roles[early-career].displayShort` → `2013 – 2017`
- `earlyCareerShort` → `2013–2017: junior iOS in product companies and indie App Store apps — first role Dec 2013; full timeline at vil4max.github.io.`

### Sync HTML

- `cv.html` — early career dates: `Dec 2013 – May 2017`
- `experience.html` — `2013 – 2017`
- `index-short.html` — `early-career-short` block text

---

## Commit 2: `fix(resume): highlight key roles, add ATS keywords, remove public phone`

### 1. Remove phone from public web

Remove `+380509864522` and all `<a href="tel:...">` from every HTML file:

- `index.html`
- `index-short.html`
- `cv.html`
- `experience.html`
- `projects.html`

Remove from both screen and print contact blocks (`header-meta-contacts--print`).

In `content/resume-source.json` → `contacts`:

```json
"phone": "+380509864522",
"phonePublic": false
```

Phone stays in JSON for private use only — **not rendered** on site or PDF.

### 2. ATS keywords (literal text)

**`content/resume-source.json`:**

- `meta.summary` — append: `Stack: Swift Concurrency, async/await, Combine, SwiftData.`
- `meta.skillsLine` and `skillsLineDetailed`:
  `Swift · SwiftUI · UIKit · Swift Concurrency · async/await · Combine · SwiftData · SPM · WatchKit · Apple platform SDKs`
- `roles[globallogic].technologies` / `technologiesLine` — add `Swift Concurrency`, `async/await`
- `roles[pasha].technologies` / `technologiesLine` — add `Swift Concurrency`, `async/await`, `Combine`

**Sync in HTML:**

- `cv.html` — `.skills-ats` and `.exp-tech-line` for GlobalLogic and PASHA
- `index-short.html` — `.skills-ats` and tech lines
- `experience.html` — `.exp-tech-tags` for GlobalLogic and PASHA

### 3. Highlight Watch AI + Birmarket, compact the middle

**Add to `resume.css`:**

- `.exp-role-head` — combined line: Company · Title · Dates
- `.exp-company-loc-line` — location on its own line
- `.experience-item--highlight` — accent border/shadow for key roles
- `.experience-item--compact` — compact view; `li + li { display: none }` (only first bullet visible)
- `.project-card--primary` — accent on landing
- `.featured-projects-primary` — 2-column grid for top projects
- `.earlier-roles-compact` + `.compact-role-list` — collapsed “Earlier production work” block

**Add to `resume-short.css`:**

- `.exp-role-head`, `.exp-company-loc-line`, `.experience-item--highlight` under `.short-cv`

**`cv.html` / `index-short.html` / `experience.html`:**

- GlobalLogic and PASHA → class `experience-item--highlight`
- Role format:

```html
<div class="exp-role-head">
  <span class="exp-company-name">GlobalLogic</span>
  <span class="exp-role-sep">·</span>
  <span class="exp-role-title">Senior iOS Engineer</span>
  <span class="exp-role-sep">·</span>
  <span class="exp-role-dates">Jan 2026 – Jun 2026</span>
</div>
<div class="exp-company-loc-line">Kyiv, Ukraine · Remote</div>
```

(Remove separate `exp-company-line` + `exp-role` for these two roles.)

- SOLVVE, Electus, GBKSoft, early-career → class `experience-item--compact`

**`index.html` (landing):**

- Watch AI and Birmarket → `.featured-projects-primary` with `project-card--primary`
- Drinkit → one card in `.featured-projects-grid`
- Replace PLAYHERA and Eastern Union full cards with:

```html
<div class="earlier-roles-compact">
  <h4>Earlier production work</h4>
  <ul class="compact-role-list">
    <li><strong>PLAYHERA</strong> — SOLVVE · 2019–2020 · UIKit, RxSwift, REST · <a href="projects.html#project-playhera">details</a></li>
    <li><strong>Eastern Union</strong> — GBKSoft · 2017–2018 · UIKit, REST · <a href="projects.html#project-eastern-union">details</a></li>
  </ul>
</div>
```

---

## Validate and publish

```bash
npm run resume:validate
npm run resume:pdf:all
```

If `vil4max` is a sibling repo, commit regenerated PDFs to `vil4max/assets/`:

- `Max_Vilchevskiy_Senior_iOS_Engineer.pdf`
- `Max_Vilchevskiy_Senior_iOS_Engineer_detailed.pdf`

**Commits:**

1. `fix(resume): anchor early career to Dec 2013 start date`
2. `fix(resume): highlight key roles, add ATS keywords, remove public phone`

Push, open PR to `main`, wait for GitHub Pages deploy.

### Smoke-check after deploy

- [ ] No `+380` in page source
- [ ] Skills contain `async/await`, `SwiftData`, `Combine`
- [ ] Watch AI and Birmarket visually larger than other roles
- [ ] Early career shows `2013`, not `2014`
- [ ] PDF downloads without phone in header

---

## Files to touch

```
content/resume-source.json
cv.html
index-short.html
experience.html
index.html
projects.html
resume.css
resume-short.css
```

## Out of scope (optional, separate PR)

- Remove or rephrase `English — Intermediate` on landing and PDF (US/EU remote)
- Sync `career/linkedin-profile.md` if it lives elsewhere
