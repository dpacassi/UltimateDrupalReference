[![GitHub stars](https://img.shields.io/github/stars/dpacassi/UltimateDrupalReference?style=flat-square)](https://github.com/dpacassi/UltimateDrupalReference/stargazers)
[![GitHub last commit](https://img.shields.io/github/last-commit/dpacassi/UltimateDrupalReference?style=flat-square)](https://github.com/dpacassi/UltimateDrupalReference/commits/main)
[![License: MIT](https://img.shields.io/github/license/dpacassi/UltimateDrupalReference?style=flat-square)](https://github.com/dpacassi/UltimateDrupalReference/blob/main/LICENSE)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)
[![Curated for modern Drupal](https://img.shields.io/badge/Focus-curated%20modern%20Drupal-0a7ea4?style=flat-square)](https://www.drupal.org/)

# Ultimate Drupal Reference

Drupal is powerful, flexible, and absolutely worth learning seriously.

It is also one of those ecosystems where newcomers can lose a lot of time on outdated advice, abandoned modules, old tutorials, historical workflows, and recommendations that were correct once but no longer reflect how modern Drupal projects are built.

This repository exists to reduce that noise.

It is a curated, practical reference for people who want to get productive with Drupal faster — especially developers and site builders who want a practical map of the ecosystem, not just a giant archive of links.

If this README helps you avoid a dead end, onboard faster, or make a better architectural decision, please **star the repository**.
That helps more people discover it and signals that keeping it updated is worth the effort.

## Why this repository exists

This guide is here to help you:

- get oriented in the Drupal ecosystem faster
- understand how a modern Drupal project is typically set up
- avoid outdated tooling and bad defaults
- find relevant modules, themes, and distributions that still matter
- debug problems more methodically
- discover where to learn next once the basics are no longer enough

## Who this is for

This reference is mainly written for:

- developers starting with Drupal or returning after a few years
- site builders who want a stronger overview of the current ecosystem
- agencies and freelancers onboarding new Drupal team members
- technical leads who want a concise reference they can hand to others

## What this repository is not

To stay useful, this project is intentionally **not** trying to be:

- a complete list of every Drupal module, theme, or distribution
- a historical archive of everything that mattered in older Drupal versions
- a replacement for official Drupal.org documentation
- a place where dead links and abandoned recommendations are kept “for completeness”

The goal is signal, not size.

## A few principles behind this guide

- The wording stays **Drupal-version-agnostic**, but the content is maintained to be valid for **modern Drupal projects**.
- This README prefers **fewer, better recommendations** over giant historical lists.
- If something is outdated, unmaintained, or no longer a sensible default, it should not stay here just because it used to matter.
- Official Drupal.org documentation comes first. Community resources come second.
- The goal is usefulness, not completeness.

## How to use this README

Depending on where you are, start here:

- **New to Drupal?** Start with [Getting started with Drupal](#getting-started-with-drupal), then [How to think about Drupal](#how-to-think-about-drupal), then [Site building](#site-building).
- **Already building Drupal sites?** Jump to [Modules](#modules), [Themes](#themes), and [Troubleshooting](#troubleshooting).
- **Returning after a few years?** Read [Installing Drupal locally](#installing-drupal-locally), [Composer](#composer), [Drush](#drush), and [Recipes and site templates](#recipes-and-site-templates) first.
- **Want to contribute?** See [Contributing](#contributing) and help keep the dynamic sections current.

## Contributing

This project gets better through real-world feedback from people actually building Drupal sites.

If you notice an outdated recommendation, a broken link, a missing section, or a module, theme, distribution, article, or learning resource that deserves to be listed here, please open an issue or submit a pull request.

Before contributing, read the [contribution guidelines](CONTRIBUTING.md).

A particularly helpful contribution is not just “add more links”, but improving the signal quality of the list:

- remove outdated resources
- replace weaker links with better current ones
- improve categorization
- add context for why something is still worth using

---

## Table of contents

- [Getting started with Drupal](#getting-started-with-drupal)
  - [Try Drupal without installing anything](#try-drupal-without-installing-anything)
  - [System requirements](#system-requirements)
  - [Installing Drupal locally](#installing-drupal-locally)
  - [Local development alternatives](#local-development-alternatives)
  - [Composer](#composer)
  - [Drush](#drush)
  - [Recipes and site templates](#recipes-and-site-templates)
  - [IDEs and editors](#ides-and-editors)
- [How to think about Drupal](#how-to-think-about-drupal)
- [Site building](#site-building)
- [Theming](#theming)
- [Distributions](#distributions)
- [Modules](#modules)
  - [Administration and developer experience](#administration-and-developer-experience)
  - [Content modeling and editorial experience](#content-modeling-and-editorial-experience)
  - [Commerce](#commerce)
  - [Forms](#forms)
  - [Migration](#migration)
  - [Search](#search)
  - [SEO](#seo)
  - [Security](#security)
- [Themes](#themes)
  - [Admin themes](#admin-themes)
  - [Frontend themes](#frontend-themes)
- [Troubleshooting](#troubleshooting)
- [Learning resources](#learning-resources)
- [Get involved with the Drupal community](#get-involved-with-the-drupal-community)
- [Credits](#credits)
- [License](#license)

---

## Getting started with Drupal

### Try Drupal without installing anything

If you just want to evaluate Drupal, a module, a theme, or a distribution quickly, use [SimplyTest](https://simplytest.me/).
It is excellent for fast experiments, issue reproduction, and quick reviews.

### System requirements

Before starting a real project, always check the current official requirements:

- [Drupal system requirements](https://www.drupal.org/docs/getting-started/system-requirements)
- [Installing Drupal](https://www.drupal.org/docs/getting-started/installing-drupal)

### Installing Drupal locally

For modern local Drupal development, **DDEV is the community-recommended default on Drupal.org**.

That does **not** mean it is the only valid option. It means that if you are starting fresh, want to align with current Drupal.org guidance, and want the path most new Drupal documentation points to, **DDEV is the first choice to recommend**.

Why DDEV is the default recommendation for this README:

- it is the current **Drupal.org recommendation**
- it is reproducible and team-friendly
- it works well with Composer, Drush, and common Drupal workflows
- it has strong cross-platform adoption across the current Drupal ecosystem

Start here:

- [Install Drupal using DDEV for local development](https://www.drupal.org/docs/getting-started/installing-drupal/install-drupal-using-ddev-for-local-development)
- [Local Development Guide](https://www.drupal.org/docs/official_docs/local-development-guide)
- [DDEV documentation](https://docs.ddev.com/)

A typical new-project flow looks like this:

```bash
composer create-project drupal/recommended-project my_site_name_dir
cd my_site_name_dir
ddev config --project-type=drupal --docroot=web
ddev start
ddev launch
```

A few practical notes:

- Keep your project Composer-managed from day one.
- Commit your `.ddev/` config when it is part of the team workflow.
- Prefer a setup that everyone on the project can reproduce easily.
- If a team already has a stable **Lando**, **Docksal**, or **Docker4Drupal** workflow, that is usually a better choice than forcing a migration for no good reason.

### Local development alternatives

This section stays intentionally short.

The goal is **not** to list every way anyone has ever run Drupal locally. The goal is to highlight the options that still matter for **Drupal 11+** work today.

| Tool / approach | Still relevant for Drupal 11+? | Recommendation level | Notes |
|---|---:|---|---|
| **DDEV** | Yes | **Best default for most new projects** | Current Drupal.org recommendation. Strong docs, broad adoption, good team reproducibility. |
| **Lando** | Yes | **Strong alternative** | Still active and supports Drupal 11. Good choice if your team already uses it or prefers its workflow. |
| **Docksal** | Yes | **Niche but still valid** | Still usable for Drupal projects, but less often the first recommendation for new teams today. |
| **Docker4Drupal** | Yes | **Valid for Docker-comfortable teams** | More hands-on and lower-level than DDEV or Lando. Sensible if your team wants more direct control over Docker setup. |
| **Plain local PHP + DB** | Yes | **Only for simple or very specific cases** | Can work, but usually less reproducible and less pleasant for serious team-based Drupal development. |
| **XAMPP / MAMP / WAMP** | Yes | **Not recommended for complex projects** | Fine for quick experiments or legacy habits, but generally weaker for modern Drupal workflows, multi-service setups, and team reproducibility. |

#### How to choose

If you want the practical version:

- **Choose DDEV** if you are starting fresh and want the path most aligned with current Drupal.org guidance.
- **Choose Lando** if your team already uses it successfully or you personally prefer its workflow.
- **Choose Docksal** or **Docker4Drupal** if your team already has strong experience with them and there is a good operational reason.
- **Avoid plain host-based stacks as your default** for larger Drupal projects, especially when multiple developers, extra services, or environment parity matter.

#### Why these are the options worth listing

These are the local-development approaches that still have meaningful relevance for current Drupal work:

- Drupal.org now explicitly recommends **DDEV** for local development.
- Drupal.org still maintains a broader page covering Docker-based local environments such as **Lando**, **Docksal**, and **Docker4Drupal**.
- Lando’s current Drupal plugin explicitly supports **Drupal 11**.
- Docksal and Docker4Drupal are still viable, but they are less often the first recommendation for new Drupal teams than DDEV.
- Plain local PHP stacks and tools like XAMPP/MAMP/WAMP still exist, but for non-trivial Drupal projects they are usually a step backward in reproducibility and team consistency.

### Composer

Composer is standard for modern Drupal development.
Use it to manage core, contributed modules, themes, Drush, and PHP dependencies.

Start here:

- [Using Composer](https://www.drupal.org/docs/develop/using-composer)
- [Using Composer to install Drupal and manage dependencies](https://www.drupal.org/docs/develop/using-composer/manage-dependencies)
- [Starting a site using Drupal Composer project templates](https://www.drupal.org/docs/develop/using-composer/starting-a-site-using-drupal-composer-project-templates)
- [Using Drupal's Composer Scaffold](https://www.drupal.org/docs/develop/using-composer/using-drupals-composer-scaffold)

If you are dealing with an older non-Composer codebase, moving it to Composer is still worth it:

- [Add Composer to an existing site](https://www.drupal.org/docs/installing-drupal/add-composer-to-an-existing-site)

### Drush

For command-line Drupal work, **Drush** is the standard tool.
If you work on Drupal seriously, learn it early.

Start here:

- [Drush](https://www.drush.org/)
- [Install Drush](https://www.drush.org/13.x/install/)
- [Drush on Drupal.org](https://www.drupal.org/docs/develop/development-tools/drush)

A few commands worth knowing right away:

```bash
drush status
drush cr
drush updb -y
drush cex -y
drush cim -y
drush uli
```

### Recipes and site templates

Recipes matter now.
If you learned Drupal years ago, this is one of the areas worth updating in your mental model.

Recipes automate module installation and configuration on an existing Drupal site.
They are a lighter, more composable alternative to the old “everything is a distribution” mindset.

Start here:

- [Drupal Recipes](https://www.drupal.org/docs/extending-drupal/drupal-recipes)
- [How to download and apply Drupal Recipes](https://www.drupal.org/docs/extending-drupal/drupal-recipes/how-to-download-and-apply-drupal-recipes)
- [Recipes Cookbook](https://www.drupal.org/docs/extending-drupal/contributed-modules/contributed-module-documentation/distributions-and-recipes-initiative/recipes-cookbook)

### IDEs and editors

There is no single required editor, but many Drupal developers use **PhpStorm**.
A good setup should give you strong PHP support, YAML and Twig handling, Composer awareness, and Git integration.

A few useful references:

- [PhpStorm](https://www.jetbrains.com/phpstorm/)
- [Drupal API documentation](https://api.drupal.org/api/drupal)
- [Drupal APIs guide](https://www.drupal.org/docs/develop/drupal-apis)

---

## How to think about Drupal

A lot of frustration with Drupal comes from approaching it like a simple page builder or a generic PHP CMS.

Drupal becomes much easier once you understand that it is really a **structured content platform** with a strong configuration system and a powerful extension model.

A few concepts are worth understanding early:

- entities and fields
- bundles and content types
- display modes and form modes
- configuration management
- permissions and roles
- Views
- cacheability metadata
- plugins, services, events, and hooks

Start with:

- [Drupal User Guide](https://www.drupal.org/docs/user_guide/en/index.html)
- [Developer documentation](https://www.drupal.org/docs/develop)
- [Documentation overview](https://www.drupal.org/documentation)

---

## Site building

If you are more on the site-building side, these are good places to start:

- [Drupal site building](https://www.drupal.org/community/contributor-guide/skill/drupal-site-building)
- [Drupal User Guide](https://www.drupal.org/docs/user_guide/en/index.html)
- [Drupal Recipes](https://www.drupal.org/docs/extending-drupal/drupal-recipes)

What good site building usually means in Drupal:

- model content first
- avoid overfitting content types too early
- use Views before writing custom listing code
- keep editorial UX in mind from the beginning
- keep configuration deployable
- do not solve everything with custom code if a well-maintained contrib module already solves it cleanly

---

## Theming

For theming, start with the official docs and learn Twig properly.
If you are building custom frontend systems, also pay attention to Starterkit and Single Directory Components in core.

Start here:

- [Theming Drupal](https://www.drupal.org/docs/develop/theming-drupal)
- [Starterkit theme](https://www.drupal.org/docs/core-modules-and-themes/core-themes/starterkit-theme)
- [Drupal theme folder structure](https://www.drupal.org/docs/develop/theming-drupal/drupal-theme-folder-structure)
- [Twig documentation](https://twig.symfony.com/)

A few practical recommendations:

- Prefer a custom theme or a clean subtheme over heavy random override chains.
- Keep templates, preprocess logic, and CSS architecture readable.
- Use Twig debug in development.
- Treat accessibility and performance as part of theming, not as “later”.

---

## Distributions

Distributions are no longer the only way to package Drupal solutions, but they are still relevant in some cases — especially when a project offers a real productized starting point rather than just a demo install profile.

Below is a curated list of currently relevant options worth knowing.

- [Open Social](https://www.drupal.org/project/social) — community platform and engagement platform for member communities, collaboration, and knowledge sharing.
- [Varbase](https://www.drupal.org/project/varbase) — a CMS starter kit and distribution focused on giving teams a strong structured starting point.

---

## Modules

The list below is intentionally curated.
It is not trying to be a complete directory of Drupal modules.
It is trying to be a good shortlist of modules that are still relevant and sensible to know.

### Administration and developer experience

- [Admin Toolbar](https://www.drupal.org/project/admin_toolbar) — improves the default Toolbar by turning it into a drop-down administration menu for faster navigation.
- [Configuration Split](https://www.drupal.org/project/config_split) — helps separate environment-specific configuration while still working cleanly with Drupal configuration management.
- [Devel](https://www.drupal.org/project/devel) — classic developer toolbox for debugging, inspecting, generating content, and general development convenience.
- [Environment Indicator](https://www.drupal.org/project/environment_indicator) — adds strong visual environment markers so you do not confuse local, staging, and production.

### Content modeling and editorial experience

- [ECA](https://www.drupal.org/project/eca) — a no-code automation engine for Drupal workflows.
- [Field Group](https://www.drupal.org/project/field_group) — groups fields together in forms and displays using wrappers such as tabs, details, accordions, and fieldsets.
- [Linkit](https://www.drupal.org/project/linkit) — rich-text linking helper with autocomplete for internal and external links.
- [Paragraphs](https://www.drupal.org/project/paragraphs) — structured modular content components for richer editorial layouts.
- [Token](https://www.drupal.org/project/token) — placeholder variables and token browsing used across many other modules and workflows.

### Commerce

- [Drupal Commerce](https://www.drupal.org/project/commerce) — the framework-first ecommerce solution for Drupal.

### Forms

- [Honeypot](https://www.drupal.org/project/honeypot) — lightweight anti-spam protection using honeypot and timestamp techniques.
- [Webform](https://www.drupal.org/project/webform) — the go-to form builder for anything from simple contact forms to large multi-step workflows.

### Migration

- [Migrate Plus](https://www.drupal.org/project/migrate_plus) — extends core migration with extra plugins, configuration entities, and examples.
- [Migrate Tools](https://www.drupal.org/project/migrate_tools) — Drush tooling and helpers for running and controlling migrations.

### Search

- [Facets](https://www.drupal.org/project/facets) — facet and filter UI for search-driven experiences, especially with Search API.
- [Search API](https://www.drupal.org/project/search_api) — the standard framework for building serious search experiences in Drupal.
- [Search API Solr](https://www.drupal.org/project/search_api_solr) — Apache Solr backend for Search API when you need more advanced search capabilities.

### SEO

- [Metatag](https://www.drupal.org/project/metatag) — structured metadata and social sharing tags.
- [Pathauto](https://www.drupal.org/project/pathauto) — automatic URL alias generation based on configurable token patterns.
- [Redirect](https://www.drupal.org/project/redirect) — manual redirects and canonical path control.
- [Simple XML sitemap](https://www.drupal.org/project/simple_sitemap) — XML sitemap generation, including multilingual support.

### Security

- [Security Kit](https://www.drupal.org/project/seckit) — security hardening options for headers and related protections.

---

## Themes

This section keeps the list short on purpose.
In modern Drupal projects, I would usually rather see a thoughtful custom theme or subtheme than a giant dependency stack chosen just because it looked convenient on day one.

### Admin themes

- [Gin Admin Theme](https://www.drupal.org/project/gin) — a modern admin experience built around a cleaner editorial and administrative UI.

### Frontend themes

- [Bootstrap5](https://www.drupal.org/project/bootstrap5) — a Bootstrap 5-based theme that can be used directly or as a subtheme base.
- [Radix](https://www.drupal.org/project/radix) — a component-oriented Bootstrap-based theme aimed at more structured frontend workflows.

---

## Troubleshooting

Every Drupal developer eventually hits the same wall:

> “This should work. Why is this not working?”

Good troubleshooting in Drupal is less about random guesses and more about following a disciplined process.

### 1. Confirm that the problem is reproducible

Before anything else:

- reproduce the problem twice
- write down the exact steps
- identify whether it happens for all users or only some users
- identify whether it is environment-specific
- identify whether it is content-specific or configuration-specific

If you cannot reproduce it clearly, debugging gets much harder.

### 2. Check whether you are using a supported release

This sounds obvious, but it saves a lot of time.

- Verify the installed version of the module, theme, or core package.
- Check the project page for release status and compatibility.
- Read the release notes if the problem appeared after an update.
- Check Drupal security advisories if the update story matters.

Useful links:

- [Security advisories](https://www.drupal.org/security)
- [Drupal core security advisories](https://www.drupal.org/security/core)
- [Contributed project security advisories](https://www.drupal.org/security/contrib)
- [Updating Drupal core via Composer](https://www.drupal.org/docs/updating-drupal/updating-drupal-core-via-composer)

### 3. Read the project page properly

A surprising number of issues come from using a project against its intended architecture.

Read:

- the project description
- requirements
- installation instructions
- release notes
- known issues
- linked documentation

Do not skip this step.

### 4. Search the issue queue before opening a new issue

For contrib work, the issue queue is often the best source of truth after the documentation.

Useful links:

- [Drupal project issues documentation](https://www.drupal.org/docs/develop/issues)
- [Find the issues for a project](https://www.drupal.org/community/contributor-guide/reference-information/quick-info/find-the-issues-for-a-project)
- [Searching for issues](https://www.drupal.org/docs/develop/issues/issue-procedures-and-etiquette/searching-for-issues)
- [Drupal core issue queue](https://www.drupal.org/project/issues/drupal)

When searching, include:

- exact error messages
- module name
- core version
- PHP version
- “update”, “cache”, “ajax”, “migration”, “Solr”, and similar qualifiers where relevant

### 5. Check logs before touching code

Look in:

- Drupal reports (`/admin/reports/dblog`) if DB logging is enabled
- web server logs
- PHP error logs
- browser console
- network requests

For CLI-based debugging, Drush is your friend:

```bash
drush status
drush cr
drush watchdog:show
drush config:get system.site
drush pm:list --status=enabled
```

### 6. Rebuild caches, then ask whether cacheability is the real issue

Many “Drupal bugs” are actually one of these:

- stale render cache
- wrong cache tags
- missing cache contexts
- broken max-age assumptions
- configuration imported but old markup is still cached somewhere

If a page behaves differently across users, languages, roles, query parameters, or routes, think about **cache contexts** early.

### 7. Reduce the problem

Try to isolate the issue by asking:

- Does it happen in a minimal View?
- Does it happen with one module disabled?
- Does it happen with the default theme?
- Does it happen with custom code removed?
- Does it happen with a fresh content entity?

A smaller reproduction almost always gets you to the answer faster.

### 8. Check change records when something “used to work”

If a behavior changed after a core update, change records matter.
They are the official record of important core changes.

Useful links:

- [Change records for Drupal core](https://www.drupal.org/list-changes/drupal)
- [Change records policy](https://www.drupal.org/about/core/policies/core-change-policies/change-records)

### 9. Ask in the right place

When you still need help, ask with enough context.

Good places:

- [Drupal Answers](https://drupal.stackexchange.com/)
- [Drupal Slack](https://www.drupal.org/join-slack)
- [Drupal forums](https://www.drupal.org/forum)

A good support request usually includes:

- what you expected
- what happened instead
- exact error message
- steps to reproduce
- relevant module or theme versions
- environment details
- what you already tried

### 10. For custom code: think like a Drupal maintainer

Before writing more code, ask yourself:

- Is there already a Drupal API for this?
- Is this a plugin, service, event subscriber, form alter, or entity access problem?
- Am I fighting core behavior instead of extending it cleanly?
- Would this still make sense six months from now?

That question alone prevents a lot of technical debt.

---

## Learning resources

A good Drupal learning path mixes official docs with practical examples.

### Official documentation first

- [Documentation overview](https://www.drupal.org/documentation)
- [Drupal User Guide](https://www.drupal.org/docs/user_guide/en/index.html)
- [Developer documentation](https://www.drupal.org/docs/develop)
- [Drupal APIs guide](https://www.drupal.org/docs/develop/drupal-apis)
- [Drupal API documentation](https://api.drupal.org/api/drupal)

### Video and talks

- [Drupal.tv](https://drupal.tv/)
- [Drupalize.Me](https://drupalize.me/)

### Community learning

- [Drupal events](https://www.drupal.org/community/events)
- [Find an event to attend](https://www.drupal.org/community/contributor-guide/reference-information/quick-info/find-an-event-to-attend)

### Selected articles and community reads

This section is intentionally small and curated.
The goal is not to collect hundreds of links again.
The goal is to keep a short list of articles that are still genuinely useful for people working on modern Drupal projects.

A good rule for future additions:

- prefer evergreen articles over trend pieces
- prefer technical depth over SEO content
- drop articles once they become version-confusing or operationally outdated
- if an official Drupal.org page covers the topic well, prefer that first

Current picks:

- [Drupal 11: What's New and What's Next](https://www.lullabot.com/articles/drupal-11-whats-new-and-whats-next)
- [Drupal Release Planning in the Enterprise](https://www.lullabot.com/articles/drupal-release-planning-enterprise)
- [Entity API Overview](https://drupalize.me/tutorial/entity-api-overview)
- [Introduction to Migrations with Drupal](https://drupalize.me/tutorial/introduction-migrations-drupal)
- [Build Content Workflows in Drupal](https://www.webwash.net/build-content-workflows-in-drupal/)
- [Lazy Loading in Drupal](https://www.specbee.com/blogs/lazy-loading-in-drupal)

### Keeping this README maintainable

To keep this repository useful over time, maintain the dynamic sections with a few simple rules:

- review article links occasionally and remove dead or clearly outdated ones
- keep the article list short
- prefer replacing weak links over endlessly growing the section
- use pull requests to suggest better current resources

---

## Get involved with the Drupal community

One of Drupal’s biggest strengths is still its community.

A few good places to connect:

- [Drupal community overview](https://www.drupal.org/community)
- [Drupal Slack](https://www.drupal.org/join-slack)
- [Drupal events](https://www.drupal.org/community/events)
- [Drupal Groups](https://groups.drupal.org/)
- [Upcoming Drupal events](https://www.drupal.org/community/events/upcoming-events)
- [Reddit /r/drupal](https://www.reddit.com/r/drupal/)
- [Drupical](https://www.drupical.com/)

If you want to contribute to Drupal itself, start here:

- [Ways to get involved](https://www.drupal.org/contribute)
- [Finding an issue to work on](https://www.drupal.org/community/contributor-guide/reference-information/quick-info/finding-an-issue-to-work-on)

> Come for the code. Stay for the community.

---

## Credits

Maintained by [David Pacassi Torrico](https://www.drupal.org/u/dpacassi).

If you find outdated content, missing modern best practices, or better current references, contributions are welcome.

---

## License

```text
MIT License

Copyright (c) 2018 David Pacassi Torrico

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```