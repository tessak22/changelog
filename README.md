# tessak22 changelog

A running record of what I'm actually working on. Dates, what shipped, what got figured out, what got decided. Proof of work.

I'm Tessa—Founding GTM Lead at [Tabstack](https://tabstack.io) (Mozilla-backed browser automation infrastructure for AI agents), founder of [Built for Devs](https://builtfor.dev) (developer adoption intelligence platform), and builder of [Selah](https://selahlearn.com), a faith-rooted homeschool management platform I made for my own family.

---

**Filter by tag:** `tabstack` `tabstack-docs` `quiver` `built-for-devs` `selah` `rival` `control-plane` `laravel` `statiq` `homeschool` `code` `strategy` `speaking` `meetings`

---

## April 2026

### April 15
`tabstack` `tabstack-docs` `quiver` `code` `strategy`

**Tabstack:** Standup. Competitor landscape research, market analysis, and CRM approach work between sessions. Researched email marketing and drip campaign strategies using the Resend API—exploring how to build journey-stage-based email automation into Quiver.

**Tabstack Docs:** 25 new and rewritten content files across four PRs—comparison pages positioning Tabstack against direct competitors and common alternatives, new depth guides covering core API patterns and integration scenarios, SDK-first rewrites of existing guides, and updated reference documentation.

---

### April 14
`tabstack` `quiver` `rival` `scout` `meetings` `code` `strategy`

**Tabstack:** Standup and a design sync. Competitor landscape research, ICP mapping, and go-to-market sequencing work between sessions.

**Tabstack Tech Writer:** Built the full technical content pipeline from scratch—SDK reference docs (TypeScript, Python, PHP), quickstarts, depth guides, SEO comparison pages against eight competitors, and example app tutorials. Four tiers of content shipped in a single evening sprint.

**Scout:** Designed and specced a new prospect intelligence tool—find everything public about a person, track when it changes, reach out at the right moment. Full CRM data model designed: Accounts, Interactions, Events, Insights. Bridged to [Quiver](https://github.com/tessak22/quiver)'s shared database so prospect signals feed directly into the GTM workflow. 41 issues scoped.

**Quiver** ([tessak22/quiver](https://github.com/tessak22/quiver)): Intent detection, monthly pattern reports, in-app notifications, artifact grooming, and AI-powered context import all landed.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Built a working demo—competitor intelligence brief rendered as a structured UI with section-by-section layouts for homepage, profile, reviews, blog, and more. Scan history page shipped. Scheduled daily scans deployed to Netlify with a background function that runs at 6am UTC.

---

### April 13
`tabstack` `quiver` `rival` `meetings` `code` `strategy`

**Tabstack:** Four meetings—an external call, standup and sprint planning, a design sync, a weekly 1:1 with manager, and a Product Hunt and growth engineering cross-share. Competitor landscape research, ICP mapping, and go-to-market sequencing work between sessions.

**Quiver** ([tessak22/quiver](https://github.com/tessak22/quiver)): Campaign detail improvements shipped—content tab added, archived artifacts hidden by default with a toggle, context import polished. MCP tool timeout bug fixed—notification fan-out was blocking responses. Marketing skills library updated from upstream.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Code review and commit work in parallel.

---

### April 12
`tabstack` `quiver` `rival` `code`

**tessakriesel.com:** Built a full custom Ghost v6 theme from scratch—terminal aesthetic with VT323 and JetBrains Mono fonts, scanline overlay, ASCII easter egg, 27 theme files across 5 phases. Homepage with six sections (hero, currently, writing, speaking, about, subscribe). Post and page templates, speaking history feed with year filters, projects page, changelog page with git log styling, wall of love, contact, and a custom 404. Deployed to Fly.io on Ghost v6 with SQLite on a persistent volume. Built a GitHub changelog import script that pulls from tessak22/changelog, parses the markdown structure, converts to Ghost HTML, and uploads via Admin API with per-project color-coded tags.

**Quiver** ([tessak22/quiver](https://github.com/tessak22/quiver)): Full codebase audit merged—security hardening, optimization, and traceability across the whole app. Remote MCP HTTP endpoint added so the agent layer can reach the app without local setup. Bulk artifact actions shipped. Docs, spec, and in-app help updated.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Profile schema expanded with ICP and audience intelligence fields. Homepage added as a first-class scan page type. Test coverage gaps closed. Production README and seed tooling improvements.

**DevRel Growth Advisor** ([tessak22/devrel-growth-advisor](https://github.com/tessak22/devrel-growth-advisor)): Published an open-source agent skill—a DevRel Growth Advisor with six reference frameworks (journey, metrics, feedback, content, competitive, team) and a prompt library. Polished the README and framework files throughout the day.

Got the Rize MCP integration working end-to-end. Created [tessak22/changelog](https://github.com/tessak22/changelog).

---

### April 11
`tabstack` `quiver` `rival` `code`

**Quiver** ([tessak22/quiver](https://github.com/tessak22/quiver)): Quiver v1 shipped—full AI marketing command center. Auth, onboarding wizard, context editor with versioning and AI-proposed update review, five AI session modes with skill injection and SSE streaming, artifact library with status workflow and version history, campaign management, performance logging with AI synthesis, dashboard with close-the-loop queue, and team settings. 69 tests, 35 marketing skill frameworks, TypeScript strict mode, five rounds of code review. Immediately after v1 merged: v1.1 landed with 13 more features including context export, performance CSV export, read-only session share links, campaign reference links, AI review mode before saving context changes, and 33 new tests. Then the full MCP server shipped—all 23 Quiver tools exposed for use with Claude, Cursor, and other MCP-compatible clients, with AI synthesis extracted to a shared core. Customer research layer added—VoC quote library, AI-powered analysis, hypothesis tracking. Content layer added—markdown storage, SEO/OG metadata, distribution tracking, metric snapshots, public API, and calendar view. 71 new tests, 13 new MCP tools. Build issues and onboarding lockout bug resolved. Dark mode shipped.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Blog and reviews scan page types added—blog extracts content strategy and topic signals, reviews extracts complaint themes that map directly to competitor weaknesses. Deep Dive prompt templates shipped with three pre-built modes: Messaging & Positioning, Developer Sentiment, and Recent Strategic Moves. Homepage scan type added with messaging and positioning schema, automate fallback, and diff-highlighted change detection. Profile schema expanded with ICP and audience intelligence fields. Production README and seed tooling shipped. Test coverage gaps closed across brief, demo route, and SSE utility.

---

### April 10
`tabstack` `quiver` `rival` `meetings` `code` `strategy`

**Tabstack:** Six meetings—a Product Hunt strategy session, a user research overview, an intro call, a weekly 1:1 with manager, an external call, and a GTM strategy sync. Competitor landscape research, messaging framework development, and go-to-market sequencing work between sessions.

**Quiver** ([tessak22/quiver](https://github.com/tessak22/quiver)): Big shipping day in parallel—demo route, Deep Dive UI, API Insights, dashboard, API routes, data layer, and scanner orchestration all landed.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Agent working through PR review feedback.

---

### April 9
`tabstack` `rival` `meetings` `strategy`

**Tabstack:** Five meetings—a new hire onboarding session, standup, an all-hands product demo day, a customer research strategy sync, and a fireside chat. Competitor landscape research, messaging framework development, and Q2 GTM planning between sessions.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Agent working through PR feedback in parallel.

---

### April 8
`tabstack` `meetings` `strategy`

**Tabstack:** Meetings through the day. CRM and Airtable setup—organizing customer records and interview targets. Competitor landscape research and go-to-market sequencing work.

---

### April 7
`tabstack` `meetings`

**Tabstack:** First day. Full day of onboarding.

---

### April 6
`rival` `selah` `code`

**[Selah](https://selahlearn.com):** Full Resources UI shipped—selection management across subjects and learning layers, a catalog browser with subject/layer/style/faith-based/trial filters, add/edit modal for both catalog and custom resources, student learning profile fields, and career direction gating for grade 7+. 16 feature tests, 68 assertions. Bug fixes and review cleanup alongside it.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Serialization bug fix in error handling.

---

### April 5
`selah` `code`

**[Selah](https://selahlearn.com):** Running until well after midnight. The resource intelligence system landed—MCP-driven resource recommendations, set-resource-selection tool with undo support and atomic audit logging, primary demotion rollback on undo, and full household scoping hardened throughout. Subject resource links migrated from a JSON column to a proper relational table. Notification scope bug fixed. Agent workflow documentation updated.

---

### April 4
`selah` `rival` `code`

**[Selah](https://selahlearn.com):** Multiple review rounds closing out the resource intelligence and subject resource links PRs. MCP OAuth issue tracked down and fixed—two separate root causes, both resolved.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Tabstack integration libraries shipped—diff summaries, SSE stream handling, Deep Dive modes, and page-type schemas. CI split into parallel checks. Codebase audit merged.

---

### April 3
`selah` `rival` `code`

**Pre-hire prep:** LinkedIn Tabstack experience entry written and iterated ahead of day one.

**Rival** ([tessak22/rival](https://github.com/tessak22/rival)): Initial Tabstack integration library implementations.

**[Selah](https://selahlearn.com):** Subject resource links relational table work underway.

---

### April 2
`strategy`

**Pre-hire research:** Deep dive on the browser automation landscape ahead of starting at Tabstack. Developer feedback, market positioning, 30-60-90 framework, and GTM strategy thinking.

---

## March 2026

### March 31
`built-for-devs` `selah` `speaking` `code`

**PagerDuty LiveStream**—live developer-facing conversation on tooling and developer experience.

**Built for Devs:** DevRel Playbook fully distributed. HN submission live. Identified Reddit auto-removal happening due to karma thresholds.

**[Selah](https://selahlearn.com):** Finishing subject resource links work late night.

---

### March 30
`built-for-devs` `selah` `homeschool` `meetings` `code`

**Built for Devs:** Customer call. Heavy post-launch follow-through messaging.

**[Selah](https://selahlearn.com):** Diagnosed a notification bug and filed a new feature issue.

**Homeschool:** Finalized a health plan and flagged some placeholder content to fix.

---

### March 29
`built-for-devs` `selah` `code`

**[Selah](https://selahlearn.com):** Resource library data model work.

**Built for Devs:** Sessions tracked through the day.

---

### March 28
`selah` `code`

**[Selah](https://selahlearn.com):** Big shipping day. Resource library, evidence portfolio, spaced repetition UI, mobile-first parent layout, iCal feed, IXL PDF import, in-app notifications, TEKS grade normalization, and removal of the inline AI assist in favor of the MCP chatbot approach.

---

### March 27
`selah` `built-for-devs` `code` `strategy`

**Built for Devs:** Afternoon messaging and product work.

**[Selah](https://selahlearn.com):** Late evening—kicked off the big multi-PR sprint. Notifications, mobile layout, AI assist removal, TEKS normalization, student PIN hardening, all landing that night.

---

### March 26
`selah` `built-for-devs` `homeschool` `code` `strategy`

**[Selah](https://selahlearn.com):** Homepage features section designed. Student progress review via MCP. Looked into whether a student was using AI to do their work—flagged one item for follow-up. Resource library and onboarding architecture decisions locked—7-step onboarding wizard, AI planning assistant for paid plans, assistant-proposes/parent-approves as the core principle.

**HuggingFace:** Migrated the Texas TEKS dataset to the Selah org and improved discoverability.

Explored a conceptual redesign of version control for AI agent workflows—named the concept "Thesis."

---

### March 25
`selah` `built-for-devs` `homeschool` `code`

**[Selah](https://selahlearn.com):** Diagnosed the broken Student Help feature and filed a batch of issues to fix it. Key architecture decisions locked around student journals and the parent-approval model.

**Built for Devs:** Audited the Developer Adoption Score approach and identified gaps to fix.

**Homeschool:** Rebuilt a physics activity—it had no hands-on layer, just a passive video.

---

### March 24
`built-for-devs` `strategy`

**Built for Devs:** Two long messaging blocks. Pre-launch coordination.

---

### March 23
`built-for-devs` `meetings`

**Built for Devs:** Customer call. Utility work in the afternoon.

---

### March 20
`built-for-devs` `code` `strategy`

**Built for Devs Product Hunt launch day.** Running from morning to evening. Built for Devs and the DevRel Playbook went live. Core launch copy anchor: "Dev tools live and die by the first 10 minutes of a developer's experience—and most teams have no idea what's happening in those 10 minutes."

---

### March 19
`built-for-devs` `homeschool` `code` `strategy`

**Built for Devs:** Day-before grind. Product Hunt launch description and strategy drafted. Monetization model finalized. Evening bug fixes and spec work. HN submission drafted. Reddit posts written for founders-only communities.

**Homeschool:** Curriculum planning for the family via Selah.

---

### March 18
`selah` `built-for-devs` `homeschool` `code`

**[Selah](https://selahlearn.com):** AI features, billing, marketing homepage, attendance log, transcript import, user guide rewrite, student help chat, timezone fixes, nav reorganization—all landed. Used Selah MCP to draft 2026 annual curriculum plans for the kids.

**Built for Devs:** DevRel Playbook social content drafted, published to the website, Stripe set up. 30-60-90-365 strategic plan drafted.

---

### March 17
`selah` `built-for-devs` `code`

**[Selah](https://selahlearn.com):** Agent docs updated, mobile layout fixes, marketing messaging drafted, homepage launch announcement written. Student help tutor prompt loosened, student journal, parent journal view, timezone and MCP fixes.

**Built for Devs:** Final pre-launch work alongside the Selah sprint.

---

### March 16
`selah` `built-for-devs` `homeschool` `code` `strategy`

**LinkedIn:** Profile audit complete—headline rewrite, About section reordered, Built for Devs and Devocate entries updated. Featured section planned, 15 post ideas queued.

**[Selah](https://selahlearn.com):** Standards fixes, curriculum plan delete, MCP tools, IXL and Khan Academy integrations, preschool mode, library card credentials, nav reorganization, data migrations, and the student-facing homework help chat feature built.

**Homeschool:** Curriculum plans drafted for multiple students via Selah MCP.

---

### March 14
`selah` `code`

**[Selah](https://selahlearn.com):** Day-long sprint—settings, MCP tool expansion, grade-banded subjects, TEKS standards seeding, annual planning tools, and several bug fixes. Environment setup was a slog—persistent local server errors fought across the afternoon and evening before landing clean.

---

### March 13
`selah` `code`

**[Selah](https://selahlearn.com):** The earliest commits. Library checkout list, annual planning, student work-ahead navigation, a login bug fix, AI settings page, and a student dashboard data fix. Spent the better part of the day fighting environment setup issues before shipping started.

---

### March 12
`built-for-devs` `code`

**Built for Devs:** Weekend build work—a couple of evening sessions still fighting the persistent local server error.

---

### March 11
`built-for-devs` `statiq` `code`

**Built for Devs:** Multiple sessions chasing the same persistent local server error across morning, midday, and evening.

**StatIQ:** Engineering team coordination happening alongside it.

---

### March 10
`built-for-devs` `statiq` `code`

**Built for Devs:** Local debugging continued—multiple sessions across the whole day still working through the server error.

**StatIQ:** Security audit wrapped up, branch protection and team workflow docs written, autonomous ticket workflow set up via Claude multi-agent loop.

---

### March 9
`built-for-devs` `statiq` `code` `meetings`

**Built for Devs:** External call to troubleshoot the persistent server error together. Multiple more sessions grinding through it. Day six of the rebuild sprint—evaluation recording pipeline and developer profile enrichment finished.

**StatIQ:** Security and optimization analysis, frontend task backlog.

---

### March 6
`built-for-devs` `code`

**Built for Devs:** Still debugging the persistent local server error—multiple sessions from morning through evening. Build continuing underneath it all.

---

### March 5
`built-for-devs` `laravel` `code` `meetings`

**Laravel:** Weekly DevRel sync. LinkedIn profile update.

**Built for Devs:** Eight code blocks—deployment and environment configuration work throughout. One of the heaviest days of the sprint.

---

### March 4
`built-for-devs` `laravel` `code` `speaking` `meetings`

**PagerDuty podcast** prep—topic: rebuilding Built for Devs in Laravel.

**Built for Devs:** Day one of the 6-day Laravel rebuild. Morning code session, back into code through the afternoon and evening. Pricing locked. VBF messaging framework established—canonical pitch and language rules set.

---

### March 3
`built-for-devs` `laravel` `code` `strategy` `meetings`

**Built for Devs:** Reviewed the Tabstack job offer. Product Hunt taglines brainstormed. TTV analytics specs drafted. Design feedback review meeting. Code into the evening.

**Laravel:** Ecosystem research and content in the morning.

---

### March 2
`built-for-devs` `statiq` `code` `meetings`

**Built for Devs:** All-day code and messaging. Technical specs defined for the evaluation recording pipeline. Engineering docs and DevRel Playbook content marketing topics refined.

**StatIQ:** Weekly sync in the evening.

---

### March 1
`built-for-devs` `code`

**Built for Devs:** Two marathon code and messaging blocks. MVP environment work and feature development throughout the day.

---

## February 2026

### February 28
`built-for-devs` `code`

**Built for Devs:** Invoice and billing work in the morning. Then a six-hour code session that started in the late afternoon and ran to midnight. The beginning of the rebuild.

---

### February 27
`built-for-devs` `laravel` `strategy`

**Laravel:** Full morning compiling and analyzing performance metrics from the Cloud Anniversary event—documented results and wrote a "vibes report" synthesizing team feedback.

**Built for Devs:** Self-hosted metrics dashboard architecture planned and scoped.

---

### February 26
`laravel` `built-for-devs` `code` `meetings`

**Laravel:** Debugging AI agent capabilities in the Laravel Skills platform. Weekly DevRel sync. Reviewed the Agent Skills Directory with the team. Security audit filtering built. Pull request work through the afternoon and evening.

**Laravel Skills:** Production bug fixes, security audit display in UI, skill filtering by audit status, agent workflow rules updated.

---

### February 25
`laravel` `built-for-devs` `selah` `code` `strategy` `meetings`

**Laravel:** All-hands meeting covering the Cloud Anniversary results. Drafted a 30/60/90-day plan for the Director of Developer Relations role. Two video calls. Early morning code, long documentation stretch, code session to close.

**Laravel Skills:** Mobile spacing fix.

**[Selah](https://selahlearn.com):** Early architecture and environment work in the evening.

---

### February 24
`laravel` `built-for-devs` `selah` `speaking` `strategy`

**Laravel Cloud One-Year Anniversary livestream**—all-day 12-hour stream celebrating Laravel Cloud's first year. Produced backup developer questions for every session, coordinated team communications throughout, worked on Laravel Skills environment configs and MCP tools between sessions.

Post-event results: 5,100 YouTube views, 1,134 watch hours, 179 peak concurrent viewers, 691 HubSpot leads, 2,800 dub.co clicks, 397 LinkedIn engagements across three posts.

**[Selah](https://selahlearn.com):** Early concept brainstorming in the final stretch of the day.

---

### February 23
`laravel` `built-for-devs` `statiq` `meetings` `strategy`

**Laravel:** Spent most of the afternoon building the Cloud Anniversary landing page—design reviews, code work, pull requests, and coordinating with the team through multiple video calls.

**StatIQ:** Weekly sync in the evening.

---

### February 22
`statiq` `code`

**StatIQ:** Billing system, game-time logic, coach performance analytics, engineering standards docs. Multiple long sessions through the morning and afternoon. Monorepo initial commit.

---

### February 21
`built-for-devs` `code`

**Built for Devs:** Late-night code sprint. Published developer evaluations for Control Plane and Laravel Cloud.

---

### February 20
`laravel` `built-for-devs` `statiq` `code` `strategy`

**Laravel:** Heavy work all morning—Cloud Anniversary landing page copy drafted, social media content written, event logistics coordinated, Office Hours session attended.

**Built for Devs:** Distribution strategy locked—HN and Reddit (founders only). DevRel playbook content strategy established around symptom-search SEO. MVP development in the afternoon.

**StatIQ:** Engineering coordination in the evening.

---

### February 19
`laravel` `built-for-devs` `meetings` `strategy`

**Laravel:** Weekly DevRel sync to plan the Cloud Anniversary livestream. Afternoon spent on logistics and marketing calendar.

Exploratory interview for a Senior Director, Developer Product Marketing role—explored and declined.

---

### February 18
`laravel` `built-for-devs` `strategy` `meetings`

**Laravel:** Drafted a competitive analysis framework for Heroku. Learning block in the evening—AI troubleshooting and feedback synthesis.

**Built for Devs:** Findings reports, marketing strategy, competitor analysis, FAQ work.

---

### February 17
`laravel` `built-for-devs` `selah` `code` `meetings`

**Laravel:** Daily sync. Weekly DX review covering Laravel Cloud feedback and Laravel Skills progress. Laravel Boost installed, skills directory and feed consolidated onto a single homepage, search and filter UX polished. Devlog and social media content written.

**[Selah](https://selahlearn.com):** Published the Texas TEKS standards dataset to HuggingFace—real TEA CASE API data replacing the AI-generated placeholder records that had been causing bugs in onboarding.

---

### February 16
`laravel` `built-for-devs` `code` `strategy`

**Laravel:** Built `tessak22/php-skills` (Laravel Skills) in a single day—full skills directory with live import from skills.sh, community feed with social platform adapters, search, caching, Cloud deployment config, and a full test suite. Deployed to Laravel Cloud and documented the first-deploy findings. Blog content drafted around the build.

---

### February 15
`built-for-devs` `statiq` `laravel` `code`

**StatIQ:** Devlog updates, API and deployment work, Claude Code orchestration blog post drafted, multi-agent system research.

**Built for Devs:** MVP work including AI-powered ICP matching research. Mux and screen recording research.

---

### February 14
`built-for-devs` `code`

**Built for Devs:** First tracked day. AI-powered ICP matching feature development and platform integration research.

---

### February 5
`laravel` `control-plane` `strategy`

**Control Plane:** Homepage copy contract work using the VBF framework. Laravel coordination alongside.

---

## January 2026

### January
`laravel` `control-plane` `strategy`

**Control Plane:** Developer product marketing and growth strategy contract work.

**Laravel:** Contract running through this period. Rize wasn't tracking yet so no session-level detail.
