# TackBar Web Roadmap

This roadmap defines the initial evolution of the public TackBar website.

The goal is to create a **small, credible, fast and maintainable public presence** for TackBar without introducing unnecessary technical complexity.

The roadmap applies to:

**Repository:** `maxsail-project/tackbar-web`

The TackBar application itself is developed separately in:

**Repository:** `maxsail-project/tackbar`

---

# v0.1 — Public Website Structure

## Objective

Create the first functional public version of the TackBar website.

The priority is to communicate clearly:

* what TackBar is;
* who it is for;
* the product philosophy;
* the current pilot;
* how sailors can participate;
* where the open-source project lives.

## Scope

Create:

* English homepage at `/`;
* Spanish homepage at `/es/`;
* responsive layout;
* language switch;
* TackBar hero;
* product positioning;
* pilot participation section;
* GitHub link;
* contact information;
* minimal footer.

## Core messaging

Primary brand message:

**TackBar**

**Sail. Debrief. Learn.**

*We sail. We debate it over beers. We learn.*

Product flow:

**Sail → Compare → Discuss → Learn**

## Pilot information

Current supported pilot data formats:

* Vakaros `.csv`
* Vakaros `.csv.gz`

Pilot contact:

`maxsail.project@gmail.com`

The website must make clear that requesting access and accepting the pilot/privacy conditions are separate actions.

## Technical constraints

Use:

* static HTML;
* CSS;
* minimal or no JavaScript.

Do not introduce:

* frameworks;
* build systems;
* backend services;
* databases;
* analytics;
* tracking scripts;
* unnecessary dependencies.

---

# v0.2 — Visual Identity

## Objective

Give TackBar Web a recognizable and coherent visual identity.

## Scope

Define and implement:

* TackBar wordmark / logo treatment;
* typography;
* primary visual language;
* color palette;
* spacing and layout rules;
* nautical visual references;
* hero image.

## Hero

Replace the initial placeholder with an approved dinghy-sailing image.

The hero should communicate sailing and teamwork rather than software.

## Design principles

The site should feel:

* nautical;
* modern;
* clean;
* human;
* slightly informal;
* focused on dinghy sailing.

Avoid generic SaaS aesthetics.

---

# v0.3 — Real Product Story

## Objective

Show that TackBar is a real working product, not only a concept.

## Scope

Add approved screenshots from the TackBar application.

Primary candidate:

* Session Viewer.

Potential secondary visual:

* collaborative session comparison or debrief view.

## Messaging

Explain visually how TackBar supports:

**Sailing data → Comparison → Conversation → Learning**

Do not fabricate product interfaces or advertise functionality that is not actually available.

---

# v0.4 — Privacy and Pilot Information

## Objective

Provide a clear public reference for privacy and pilot participation.

## Scope

Add appropriate public information pages, potentially including:

* `/privacy/`;
* `/pilot/`;
* Spanish equivalents.

The exact structure should be decided before implementation.

## Privacy principles

The site should communicate clearly that:

* TackBar is open-source;
* participant data is not open data;
* GPS tracks are not published in the public repository;
* participation in the pilot is voluntary;
* pilot infrastructure and data processing remain within the EU/EEA;
* pilot data retention is currently defined as a maximum of six months after the pilot ends;
* complete participation and privacy conditions are provided before participation.

The website itself should avoid collecting personal information beyond what is explicitly approved.

---

# v0.5 — Public Deployment

## Objective

Publish TackBar Web as the official public entry point for the project.

## Domains

Target structure:

* `tackbar.eu` → main public website;
* `tackbar.eu/es` → Spanish website;
* `tackbar.es` → redirect to the Spanish website;
* `app.tackbar.eu` → reserved for the TackBar application.

## Scope

Configure:

* production hosting;
* HTTPS;
* domain routing;
* Spanish-domain redirect;
* caching;
* basic security headers;
* final responsive validation;
* production link validation.

## Deployment principles

Prefer:

* static hosting;
* EU/EEA infrastructure;
* minimal operational complexity;
* no unnecessary external services.

---

# Future

Future versions are intentionally undefined.

Possible future needs may include:

* additional product screenshots;
* news or project updates;
* contribution information;
* additional supported sailing devices;
* automatic activity integrations;
* richer pilot onboarding;
* public application access.

These items are **not committed scope**.

They should only enter the roadmap after an explicit product decision.

---

# Development Principles

Across all versions:

1. Keep the website simple.
2. Do not introduce functionality without a clear product need.
3. Preserve English and Spanish semantic equivalence.
4. Do not advertise unsupported TackBar capabilities.
5. Prefer real sailing imagery and real TackBar screenshots.
6. Keep personal sailing data separate from the open-source project.
7. Maintain good mobile, tablet and desktop usability.
8. Keep Git operations human-controlled.
9. Implement changes in small, reviewable increments.
10. Prioritize credibility and clarity over feature richness.

---

**TackBar**

**Sail. Debrief. Learn.**

*We sail. We debate it over beers. We learn.*
