<div align="center">
  <h1>palStack.io</h1>
  <p><strong>Everyday tools for food, money, home and friends.</strong></p>
  <p>
    <a href="https://palstack.io">Website</a> ·
    <a href="https://discord.gg/mcgcp7RdYs">Discord</a> ·
    <a href="mailto:support@palstack.io">support@palstack.io</a>
  </p>
</div>

palStack builds small, privacy-first apps for the ordinary jobs of running a life: what is in the kitchen, where the
money goes, what the house needs, and getting friends together. Each one is a "pal". The core of each is open
source and runs on your own server with Docker; we also run hosted editions for people who would rather not.

No ads, no tracking, and nothing about you is sold.

## The pals

| | What it does | Self-host | Try it |
|---|---|---|---|
| **[finPal](https://github.com/palStack-io/finpal-core)** | Budgets, goals, debt and shared costs, and it teaches money from your own figures as you go | [finpal-core](https://github.com/palStack-io/finpal-core) | [Demo](https://findemo.palstack.io) · [palstack.io/finpal](https://palstack.io/finpal) |
| **[pantryPal](https://github.com/palStack-io/pantrypal-core)** | Know what is in the kitchen, use it before it expires, one shared shopping list, recipes from what you have | [pantrypal-core](https://github.com/palStack-io/pantrypal-core) | [Demo](https://pantrydemo.palstack.io) · [palstack.io/pantrypal](https://palstack.io/pantrypal) |
| **[propertyPal](https://github.com/palStack-io/propertypal-core)** | Maintenance, appliances and warranties, documents, projects and what the house costs | [propertypal-core](https://github.com/palStack-io/propertypal-core) | [Demo](https://propertydemo.palstack.io) · [palstack.io/propertypal](https://palstack.io/propertypal) |
| **[gatherPal](https://github.com/palStack-io/clubpal-core)** | Your friend group, without the admin: plans, invites, rotations and who brings what | [clubpal-core](https://github.com/palStack-io/clubpal-core) (read its security note first) | [Demo](https://clubdemo.palstack.io) · [palstack.io/gatherpal](https://palstack.io/gatherpal) |
| **[jobsearchPal](https://github.com/palStack-io/jobsearchPal)** (labs) | A job-search assistant on your own computer: tailored applications you review and send yourself, plus the unemployment paperwork | [jobsearchPal](https://github.com/palStack-io/jobsearchPal) | [palstack.io/labs/jobsearchpal](https://palstack.io/labs/jobsearchpal) |
| **[pointsPal](https://github.com/palStack-io/pointsPal)** | An open dataset of credit card rewards that powers finPal's card optimiser | Data, MIT | [dist/programs.json](https://github.com/palStack-io/pointsPal/blob/main/dist/programs.json) |

Each repository's README has a quick start. Most pals are up in a few minutes with Docker Compose and a generated
`.env`.

## How we build

- **Your data stays yours.** Self-hosted, a pal talks to nobody unless you switch something on, such as a bank
  connection or email. Each repository documents what can leave your server.
- **Open core.** The self-hosted editions are complete and licensed AGPL-3.0 (pointsPal is MIT). The hosted editions
  add convenience and pay for the work; they never take features away from Core.
- **Built for households.** The pals are made for personal and family use. For commercial use, ask us about a
  commercial licence.
- **AI, said plainly.** We use AI tools such as Claude, ChatGPT and Cursor as part of how we build, and a person
  reviews every change before it ships.

## Get involved

- **Questions and ideas:** [Discord](https://discord.gg/mcgcp7RdYs), or an issue on the pal's repository.
- **Bugs:** open an issue on the pal's repository with what you expected and what happened.
- **Code contributions are paused** while we work out how to review AI-assisted changes well. We will reopen them.
- **Security problems:** please report privately; see our [security policy](https://github.com/palStack-io/.github/blob/main/SECURITY.md).

## Team

A small team with day jobs, building tools we use ourselves.

- **Harun Gunasekaran**: Founder, full-stack architect and engineer
- **Rachel Surette**: Co-founder, marketing and sustainability
- **Elle Russell**: Co-founder, lead UI/UX designer
- **Chris Macioci**: Co-founder, lead DevOps
- **Hannah Sidwell**: Lead QA engineer
- **Chaitanya Gunupudi**: Senior advisor, cybersecurity and architecture

More at [palstack.io/team](https://palstack.io/team).
