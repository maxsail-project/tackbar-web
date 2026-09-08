# AGENTS.md

## Purpose

This repository contains the public website for **TackBar**.

TackBar is an open-source project for dinghy sailors focused on collaborative post-sailing debriefing.

Main TackBar repository:

https://github.com/maxsail-project/tackbar

This repository contains only the public website. It does not contain the TackBar application.

---

## Development model

Development is AI-assisted, but remains human-controlled.

Codex may:

* inspect the repository;
* analyze existing code and documentation;
* propose implementation approaches;
* implement explicitly requested changes;
* review code;
* identify defects, regressions, accessibility issues, security concerns, and maintainability problems;
* add focused tests or validation when appropriate.

Codex must not independently expand product scope or introduce architectural changes that were not requested.

Prefer:

* small focused increments;
* simple implementations;
* readable code;
* minimal dependencies;
* review-first changes;
* preservation of existing behavior;
* no unrelated refactors.

---

## Source of truth

Before implementing any change:

1. Read this `AGENTS.md`.
2. Read `README.md`.
3. Read any documentation directly relevant to the requested change.
4. Inspect the existing implementation before proposing modifications.
5. Reconcile the requested task with existing documented decisions.

If the requested change conflicts with repository documentation or an existing product decision, identify the conflict before implementing it.

Do not invent product behavior, supported formats, integrations, privacy claims, domains, or functionality.

---

## Website scope

The website is the public presentation layer for TackBar.

Its purpose is to communicate:

* what TackBar is;
* why it exists;
* the TackBar philosophy;
* the current pilot;
* how interested sailors can participate;
* links to the open-source project.

The actual TackBar application is separate.

Current domain model:

* `tackbar.eu` — primary public website;
* `tackbar.eu/es` — Spanish version;
* `tackbar.es` — intended to redirect to the Spanish website;
* `app.tackbar.eu` — reserved for the TackBar application.

Do not change this domain model unless explicitly requested.

---

## Product messaging

Current primary brand messaging:

**TackBar**

**Sail. Debrief. Learn.**

*We sail. We debate it over beers. We learn.*

The beer reference expresses part of the cultural origin and personality of TackBar. It must not imply that alcohol consumption is required or central to participation.

The broader product idea is:

**Sail → Compare → Discuss → Learn**

TackBar should be presented primarily as a tool that helps sailors turn sailing sessions and post-sailing conversations into learning.

Avoid presenting TackBar merely as:

* a GPS tracker;
* a file viewer;
* a CSV uploader;
* a performance dashboard.

Do not exaggerate capabilities that are not currently implemented.

---

## Pilot

TackBar is currently in an experimental pilot phase.

Pilot contact:

`maxsail.project@gmail.com`

Current supported pilot data formats include Vakaros exports:

* `.csv`
* `.csv.gz`

Do not advertise additional formats, devices, integrations, or automatic ingestion mechanisms unless they have been explicitly confirmed for the pilot.

In particular, future integrations must not be presented as currently available.

Participation requests and legal consent are separate actions.

Sending an email requesting access does not constitute consent to participate.

---

## Privacy

TackBar is open-source, but participant data is not open data.

Never imply that:

* personal information;
* GPS tracks;
* sailing-session data;
* participant information

will be published in the public repository.

For the pilot:

* participation is voluntary;
* infrastructure and data processing are intended to remain within the EU/EEA;
* pilot data retention is currently defined as a maximum of six months after the pilot ends;
* formal participation/privacy conditions are provided separately.

Do not introduce analytics, advertising trackers, cookies requiring consent, third-party tracking scripts, contact forms, or new personal-data collection mechanisms without an explicit decision.

---

## Technical principles

Keep the public website deliberately simple.

Default implementation:

* static HTML;
* CSS;
* minimal or no JavaScript;
* no application framework;
* no backend;
* no database;
* no CMS.

Do not introduce React, Next.js, Astro, Vue, Tailwind, Bootstrap, npm dependencies, build systems, or other frameworks/libraries unless explicitly requested.

Prefer web platform capabilities over dependencies.

The site must work when served as static files.

---

## Structure

Prefer a simple structure similar to:

```text
/
├── index.html
├── es/
│   └── index.html
├── assets/
│   ├── images/
│   └── styles.css
├── README.md
├── AGENTS.md
└── LICENSE
```

Modify this structure only when there is a clear reason.

---

## Language

English is the primary language of the website.

Spanish content lives under `/es`.

English and Spanish pages should remain semantically equivalent, although wording may be adapted naturally rather than translated literally.

Do not silently update only one language when the change materially affects both versions.

---

## Visual design

The site should feel:

* nautical;
* modern;
* clean;
* simple;
* human;
* slightly informal;
* focused on dinghy sailing rather than generic SaaS.

Prefer:

* strong sailing imagery;
* real TackBar product screenshots;
* generous whitespace;
* strong typography;
* a small number of clear messages.

Avoid generic startup clichés, excessive cards, gradients, visual noise, fake testimonials, fake statistics, pricing sections, or unsubstantiated marketing claims.

Use only images or assets that are provided, owned, licensed, generated for the project, or otherwise explicitly approved.

---

## UX and quality

Changes must preserve or improve:

* mobile usability;
* tablet usability;
* desktop usability;
* semantic HTML;
* keyboard navigation;
* accessible contrast;
* useful alternative text;
* performance;
* clear navigation between English and Spanish.

Avoid unnecessary JavaScript.

Avoid layout shifts and unnecessarily large assets.

---

## Links and external services

External links should be explicit and trustworthy.

The main TackBar project should link to:

https://github.com/maxsail-project/tackbar

Do not invent URLs for services that do not yet exist.

Until explicitly implemented, do not assume that `app.tackbar.eu` is publicly available.

---

## Git workflow

Git remains human-controlled.

Codex must never automatically:

* stage files;
* commit;
* push;
* create tags;
* create releases;
* merge branches.

Never use:

```bash
git add .
git add -A
git add --all
```

If Git operations are explicitly requested, operate only on the exact confirmed files.

Before reporting completion, show or summarize:

* files changed;
* relevant behavior changed;
* behavior intentionally left unchanged;
* validation performed;
* any remaining limitations or decisions needed.

---

## Change discipline

For every implementation task:

1. Inspect the current state.
2. State the intended focused change.
3. Implement only that scope.
4. Validate the result.
5. Review the diff for unrelated modifications.
6. Report exactly what changed.

Do not perform opportunistic refactors.

Do not alter marketing copy, product terminology, privacy wording, or supported capability claims merely for stylistic preference.

When unsure whether a change affects product meaning, preserve the existing wording and report the concern instead.

---

## Current status

TackBar Web is in its initial public-site / pilot phase.

The priority is not feature richness.

The priority is a small, credible, fast and maintainable public presence for TackBar.
