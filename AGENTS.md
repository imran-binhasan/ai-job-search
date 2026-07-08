# Job Application Assistant for Imran Bin Hasan

## Role
This repo is a job application workspace. opencode acts as a career advisor and application assistant for Imran, helping with:
1. **Job fit evaluation** - Assess job postings against your profile (skills, experience)
2. **CV tailoring** - Adapt CV templates to target specific roles
3. **Cover letter writing** - Draft targeted cover letters
4. **Interview preparation** - Prepare answers, questions, talking points
5. **Career strategy** - Advise on positioning

## Candidate Profile

### Identity
- **Name:** Imran Bin Hasan
- **Email:** imranbinhasan.work@gmail.com
- **LinkedIn:** linkedin.com/in/imran-binhasan
- **GitHub:** github.com/imran-binhasan
- **Location:** Dhaka, Bangladesh
- **Languages:** Bengali, English
- **Status:** Currently employed, actively looking

### Education
- **BSc in CSE** (2024-2027, Weekend) - **Presidency University** (CGPA 3.69/4.00)

### Professional Experience
- **Fullstack AI Developer** (Jan 2026 - Present) - **Coredevs Ltd**
  - Led MVP development of a geospatial sports app for a YC-backed startup; delivered full product from architecture to deployment
  - Engineered microservice-based, config-driven algo trading system in Node.js (Binance, Bybit, Alpaca) — <50ms order-to-fill latency, strategy backtesting, multi-instance live execution
- **Software Engineer (Backend)** (Mar 2025 - Dec 2025) - **AppifyDevs**
  - Architected enterprise HRMS handling payroll for 2000+ employees across 10+ countries
  - Delivered 5+ e-commerce/SaaS products (AI chat, payments, analytics dashboards)
  - Rebuilt IJRP academic journal platform — 4000+ submissions, peer-review workflow
- **Junior Fullstack Developer** (Jun 2024 - Feb 2025) - **Qwik IT**
  - Built e-commerce platforms, landing pages, admin dashboards
  - Contributed to enterprise SaaS for talent optimization

### Technical Skills
- **Languages:** TypeScript, JavaScript, Python, Go
- **Backend:** Node.js, NestJS, Express.js, FastAPI, GraphQL, Socket.io, RabbitMQ, gRPC
- **Frontend:** Next.js, React.js, React Native, Expo, Tailwind CSS, Redux Toolkit, Tanstack Query
- **Database:** PostgreSQL, MySQL, MongoDB, Redis, VectorDBs
- **DevOps & Cloud:** AWS, Docker, GitHub Actions, CI/CD, Nginx, Traefik
- **Other:** Multiple ORMs (Prisma, Drizzle, TypeORM, Sequelize, GORM), microservices architecture, AI/LLM integration, system design

### Projects
- **Unirift** - AI-native personal productivity platform built with 9 microservices (Go, Python, TypeScript), custom ReAct agent loop with 2M-token context management, semantic ingestion pipeline, LLM routing via self-hosted LiteLLM across 20+ models
- **WarpDB** - Hybrid in-memory/persistent KV store in Go; 250k+ req/sec, goroutine-based concurrency, ACID-safe writes, pluggable storage engine
- **MegaMart** - Multi-vendor e-commerce platform; dynamic RBAC, RabbitMQ async workflows, Redis caching, NestJS + PostgreSQL, SSLCommerz/bKash/Stripe/PayPal integration

### Target Sectors
- **BD IT Companies:** Fullstack/Backend/AI developer roles at the 500+ tracked Bangladeshi companies
- **Remote:** Node.js/NestJS/Next.js backend or fullstack roles
- **Fintech/EdTech/SaaS:** Product companies using TypeScript, Node.js, React

## Repo Structure
- `cv/` - LaTeX CV variants (moderncv template, banking style)
- `cover_letters/` - LaTeX cover letters (custom cover.cls template)
- `.opencode/skills/` - AI skill definitions for the application workflow
- `.agents/skills/` - Job search CLI tools

## Workflow for New Job Applications
1. User provides a job posting (URL or text)
2. **Always evaluate fit first**: skills match, experience match, behavioral/culture match. Present this assessment to the user before proceeding.
3. If good fit: create targeted CV (`cv/main_<company>.tex`) and cover letter (`cover_letters/cover_<company>_<role>.tex`)
4. **Verify both documents** (see Verification Checklist below)
5. Prepare interview talking points based on the role requirements and your strengths

**Important:** When mentioning agentic coding or AI tooling in CVs/cover letters, explicitly reference **Claude Code** by name.

## Verification Checklist
After creating or updating a CV or cover letter, re-read the generated file and verify **all** of the following before presenting to the user. Report the results as a pass/fail checklist.

### Factual accuracy
- [ ] All claims match actual profile (AGENTS.md / candidate profile) - no fabricated skills, experience, or achievements
- [ ] Job titles, dates, company names, and locations are correct
- [ ] Contact details are correct
- [ ] All company-specific claims (partnerships, products, technology, expansions) have been independently verified via WebFetch/WebSearch - do not trust reviewer agent research without verification

### Targeting
- [ ] Profile statement / opening paragraph is tailored to the specific role (not generic)
- [ ] Skills and experience bullets are reframed to match the job requirements
- [ ] Key job requirements are addressed (with gaps acknowledged where relevant)
- [ ] Nice-to-have requirements are highlighted where there is a match

### Consistency
- [ ] CV follows the standard 2-page moderncv/banking format
- [ ] Cover letter uses cover.cls template and established structure
- [ ] Tone is consistent across CV and cover letter
- [ ] No contradictions between CV and cover letter content

### Quality
- [ ] No LaTeX syntax errors (balanced braces, correct commands)
- [ ] No spelling or grammar errors
- [ ] Agentic coding / AI tooling references mention **Claude Code** by name
- [ ] Cover letter is addressed to the correct person (or "Dear Hiring Manager" if unknown)
- [ ] Cover letter fits approximately one page

### Compiled PDF verification (MANDATORY - never skip)
Both documents MUST be compiled and visually inspected via the Read tool on the PDF output. "Looks fine in the .tex" is not acceptable - LaTeX page-break decisions are unpredictable. Iterate until these all pass:
- [ ] CV compiled with **lualatex** (pdflatex often fails on modern MiKTeX with fontawesome5 font-expansion errors). Cover letter compiled with **xelatex** (cover.cls requires fontspec).
- [ ] **CV is exactly 2 pages** - not 1, not 3
- [ ] **No orphaned `\cventry` titles** - a job/education title must never sit at the bottom of a page with its bullets spilling to the next page. Use `\needspace{5\baselineskip}` before each `\cventry` to prevent this, and `\enlargethispage{2-3\baselineskip}` to rescue a trailing section that just barely spills
- [ ] **Cover letter is exactly 1 page** - signature block must fit with the body, never overflow
- [ ] **Cover letter bullet font matches body font** - `\lettercontent{}` must not wrap `\begin{itemize}...\end{itemize}` (the command's trailing `\\` errors on `\end{itemize}`, and moving itemize outside loses the Raleway font). Standard pattern: close `\lettercontent{}`, then wrap the list in `{\raggedright\fontspec[Path = OpenFonts/fonts/raleway/]{Raleway-Medium}\fontsize{11pt}{13pt}\selectfont \begin{itemize}...\end{itemize}\par}`

### ATS & keyword verification (CV)
ATS parsers read the PDF's embedded text layer, not the rendered page. Extract it with `pdftotext -layout` and verify what a parser sees. `pdftotext` (poppler) is optional - if missing, skip the parseability items with a warning and check keyword coverage from the visual PDF read instead.
- [ ] CV text layer extracts cleanly - no `(cid:*)` markers, `�` replacement characters, or text visible in the PDF but absent from the extraction
- [ ] Email and phone appear as **literal text** in the extraction (icon-glyph noise like `MOBILE-ALT`/`Envelope` is harmless, but a contact detail carried only by an icon or hyperlink is invisible to ATS)
- [ ] Reading order of the extracted text matches the visual order (single-column stock template is safe; multi-column custom templates are where this breaks)
- [ ] Posting keywords covered or honestly absent - synonym-only matches tightened to the posting's exact term where truthfully applicable, keywords the profile genuinely supports added to experience bullets, genuine gaps left visible and **never stuffed**
