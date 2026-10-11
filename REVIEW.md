# Resume transformation review

Completed October 11, 2026. The authoritative resume is `index.html`; `style.css` controls screen and print presentation. The downloadable PDF at `output/pdf/greyson-alegria-resume.pdf` was exported from that HTML. This review records implementation and validation; subsequent publication is tracked in Git history. The obsolete `master-resume.pdf` is replaced by the new download.

## Positioning and changes

The headline establishes software engineering and AI applications. The two-sentence introduction retains C and Java as the programming foundation and explicitly describes Python as the intended specialization. Python is also supported by an implemented development-planning controller; it is not presented as the language of the voice-receptionist backend.

Three technical projects show service integration, application logic, and client/server engineering. ASG remains under the internship already recorded in the original resume. The cafe website sits under the actual Barista / Server role, without inventing a technical job title. Generic service duties are condensed. Coursework, Haskell, long concept lists, and repetitive technology lines were removed to prioritize evidence and achieve one page. The existing static architecture, contact details, links, teal palette, and browser print action are preserved. The layout is now single-column, uses locally bundled DM Sans and Manrope fonts, and includes a PDF download.

## Evidence and claim boundaries

| Resume content | Evidence inspected | Boundary |
| --- | --- | --- |
| C and Java foundation; education, GPA, honors, employment | User's request and original resume at commit `bc13318` | Supported background, not independent transcript or employer verification. |
| Alegria receptionist and staging backend | [Repository checkpoint](https://github.com/GreysonA75/alegria-automation/blob/16d8be2c82b57f3f503a4688866155044b886e3f/business-system/execution-checkpoint.md), `business-system/automation/normalize-call.mjs`, `business-system/cloudflare-worker/src/index.mjs`, and `src/request-controls.mjs` at the same revision | Code supports signed ingress, normalization, unique-event handling, D1 persistence and queued alerts. Records distinguish historical Retell/n8n/Sheets demo success from disabled staging and unfinished delivery/reconciliation. No commercial production, current live calling, SMS, booking or delivered-alert claim. |
| Python planning controller | [Controller](https://github.com/GreysonA75/alegria-automation/blob/16d8be2c82b57f3f503a4688866155044b886e3f/agent-system/receptionist_agents/controller.py), adjacent `runtime.py`, `README.md`, and `tests/test_controller.py` | Sequential OpenAI Agents SDK roles, structured output, persisted job state, repair limits, usage tracking and unit tests exist. Model roles have no tools. This is planning-only development tooling, not an autonomous coding or customer-service agent. Tests were inspected, not rerun here; live model calls were not made. |
| ASG frontend | [Mobile navigation](https://github.com/GreysonA75/asg-executive-search/blob/46d69c3806608b892817382ed615314cdd3b3624/src/components/layout/MobileNav.tsx), `package.json`, `src/components/sections/SearchProcess.tsx`, `src/app/asg-resume/page.tsx`, `src/lib/metadata.ts`, `next.config.ts`, and route tree at that revision | Next.js/React/TypeScript, reusable components, typed content, routing, keyboard handling and metadata are implemented. Candidate page uses contact links. No recruiting automation, API backend, Vercel production deployment or performance improvement is claimed. |
| ReAppraise | [Client](https://github.com/GreysonA75/ReAppraise/blob/27fa11dce40799e981e2b9ad0f548595154a3fef/ReAppraise/ContentView.swift), adjacent `VisionCloudService.swift`, local `Desktop/DonatePrice/DonatePrice/ReAppraise/PriceEstimator.swift`, and `donateprice-backend/functions/index.js` | Prototype code supports photo input, callable-function requests, asynchronous analysis, stale-response checks, percentile estimates and condition adjustments. Local backend implements Vision and eBay OAuth/Browse calls. Current deployed end-to-end success was not established. |
| PAWNARCHY | `/Users/ga/Documents/ChatGPT/PAWNARCHY/src/server/Combat.luau`, ability modules, `tests/PawnChecks.luau`, `scripts/validate-character-roundtrip.py`, and `docs/TECHNICAL_ARCHITECTURE.md` | Modular gameplay, authoritative validation, progression, HUD and regression fixtures exist. Recorded Studio checks support prototype maturity, but they were not rerun in this task. Actual multiplayer/latency checks and final game systems remain incomplete. No published-game or complete anti-cheat claim. |
| Cafe website | [Website source](https://github.com/GreysonA75/Dulcet-Delish-Website/blob/f317293abc8cc86b6ef5434e7ee17dc1a2458301/index.html), `contact.html`, `script.js`, and local stylesheet at the same project | Responsive pages, keyboard/mobile navigation, a FormSubmit contact form and CafeOrCoffeeShop JSON-LD exist. Form delivery and business outcomes were not tested or claimed. |

Other accessible work was considered: Bean provides another Swift/Overpass API application, and local ReAppraise precursor services add JavaScript backend evidence. Neither displaces the selected projects. The accessible repository inventory did not reveal a stronger standalone C/Java project. The local lab-2 project contains small C++ class/inheritance exercises, which were not relabeled as C or promoted above substantial applications. Python asset-generation and validation scripts also exist in PAWNARCHY, but the planning controller is the clearer Python example. Course notebooks were not promoted as AI engineering experience. Indexed local-knowledge search returned no matching evidence; current files and connected GitHub sources were used instead.

Project ownership is supported by the user's account, request, resume and project records. Source code establishes implementation, not the manual authorship of every line. AI-assisted development is documented in the receptionist records; the resume does not claim unaided coding, professional AI expertise or independent ownership of every engineering decision.

## Career-direction research

Austin's [NexusTrade introduction](https://nexustrade.io/blog/-whos-the-whiz-behind-nexustrade--20230514) identifies Justin as his twin and StarksTech cofounder and describes Austin's developer/architect role. Justin's [own post](https://www.linkedin.com/posts/justinstarks97_nexustrade-no-code-automated-trading-and-activity-7255394872315015168-bL2_) credits Austin with building NexusTrade. This does not establish Justin's ownership of particular platform components. His LinkedIn activity includes liked posts; these were not treated as his engineering accomplishments.

[NexusTrade](https://nexustrade.io/) demonstrates an AI-enabled software product combining research, strategy configuration and testing. Austin's [engineering workflow explanation](https://nexustrade.io/videos/pelosi-sdk-engineer-walkthrough-27092026?t=93.703) discusses design review, implementation, code review and testing. The [StarksTech Gemini competition submission](https://ai.google.dev/competition/projects/nexusgenai) provides a separate example of LLM prompt management and evaluation tooling. These references inform the software-product direction only; none of their accomplishments or technologies were attributed to Greyson.

## Representative early-career requirements

Reviewed October 10-11, 2026. These are a small positioning sample, not an exhaustive market survey or assurance of continuing availability. Ashby results were available through indexed employer-page text; direct extraction of those pages returned JavaScript shells.

| Employer role | Relevant requirements and implications |
| --- | --- |
| [Netic: Agent Platform, New Grad 2026-2027](https://jobs.ashbyhq.com/netic/d9bcb6a2-0e54-4cb3-baec-43f2d74db18f) | Python/asyncio/FastAPI, TypeScript/React, LLM tooling exposure, orchestration and failure recovery. Supports emphasizing real integration and controller code; highlights Python service and evaluation gaps. |
| [Authentic: New Grad Software Engineer](https://job-boards.greenhouse.io/authenticinsurance/jobs/4114318009) | React with Python/FastAPI, web-project experience, data structures, algorithms, design and code review. Supports broad software engineering positioning and the May 2027 graduation date. |
| [Nash: Full Stack Engineering Intern](https://jobs.ashbyhq.com/nash/5d2387ea-c478-433b-b3db-30115d1984c5/) | React/TypeScript, Python services, LLM workflows, REST APIs and relational databases. Strong overlap with the intended product direction; no unverified framework/database was added to skills. |
| [D3: Backend Engineer, New Grad](https://job-boards.greenhouse.io/d3/jobs/4915295008) | 0-2 years; projects count; a backend language, databases, Git, debugging and testable code. Supports keeping practical JavaScript/service work visible alongside C and Java. |

The gaps are deeper Python application ownership, async/backend APIs, database-backed product behavior, and measured agent quality. FastAPI, PostgreSQL, RAG, vector databases, Docker and advanced observability were not added as current skills. A broad software recruiter now sees conventional application and gameplay engineering; an AI recruiter sees service integration and bounded agent tooling; a Python specialist sees legitimate but limited project evidence rather than expert positioning.

## Facts and limitations to confirm

- Confirm the current exact GPA, honors counts, graduation date, and employment titles/dates against personal records. They match the supplied background/original resume; no official academic or employment documents were available.
- The original resume records ASG as Web Development Intern, October 2026-present. That existing title was retained, not inferred from the code. Confirm the employment arrangement if the original entry was provisional.
- The receptionist records indicate that a demo number and working Retell/n8n/Sheets flow existed, superseding the earlier number-purchase blocker. Current provider account availability, billing and n8n service status were not checked. The latest inspected handoffs describe disabled staging, not a public operational service.
- ReAppraise's GitHub client sends `imageBase64`, while the accessible local backend expects `base64`. The deployed backend's current contract is unknown. Confirm/fix this seam before demonstrating a working live image-to-price flow. The resume describes prototype implementation, not production reliability.
- PAWNARCHY has no public project URL in the accessible inventory and still needs multiplayer/latency validation. Do not claim it is published or complete.

## Validation

The visual refinement restores the original typography, teal accents, aligned contact header, and section rules, with more screen spacing. Resume content remains unchanged and the printable body stays single-column. Font licenses are included in `assets/fonts/`.

- No package/build configuration or existing test suite exists in this static resume repository. No application build command applies.
- Local browser returned HTTP 200 and no JavaScript page errors. Checked widths 320, 375, 390, 720, 721, 816 and 1440px with no horizontal overflow.
- Browser Save as PDF invokes `window.print()`. Download PDF returns the generated file. Print CSS hides the action controls.
- PDF: one US Letter page, 10pt body type, tagged and unencrypted. Every resume text segment extracts successfully (accounting for uppercase headings); all nine resume hyperlinks are embedded. Rendered PDF and desktop/mobile layouts visually inspected.
- Five public HTTP links returned 200. The receptionist demo returned 401 and is labeled as requiring sign-in. LinkedIn returned its automated-access status 999; profile availability cannot be confirmed from that response. No public 404 was observed. Contact URI values were preserved; no phone call or email was sent.
- `git diff --check` passes. No underlying project runtime, provider account, deployment or production system was modified or revalidated.

For future PDF updates, edit `index.html`, open it in Chrome, click Save as PDF, and save a Letter-size export to `output/pdf/greyson-alegria-resume.pdf` with browser headers/footers disabled. The task's export used the existing Playwright/Chrome tooling against this same HTML; no PDF content template or new application dependency was introduced.

## Highest-impact next work

Build one substantial Python service-desk application extending the receptionist idea: FastAPI, typed request/response contracts, PostgreSQL, authenticated staff access, async jobs, and a React interface. Add a tool-calling assistant that can inspect service requests and propose appointments, with explicit confirmation before external actions. Make it interview-defensible with mocked-provider integration tests, duplicate/retry/error cases, a fixed agent-evaluation dataset, sanitized logs, CI and a reproducible deployment/demo. These are future accomplishments, not current resume claims.
