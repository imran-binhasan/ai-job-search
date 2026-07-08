# Search Queries for Job Scraper

<!-- SETUP: Customize these queries based on your skills, target roles, and location -->

## Search Sites

Primary (Danish job market):
- **jobindex.dk** - largest Danish job board
- **linkedin.com/jobs** - LinkedIn job listings (filter: Denmark / your city)
- **karriere.dk** - IDA's job board (engineering/science roles)
- **jobfinder.dk** - another major Danish job board
- **akademikernes.dk** - academic union job board

Secondary (company career pages via Google):
- Direct Google searches with `site:` filters for known target companies

## Query Categories

Queries are grouped by priority. Each query should be combined with your location terms (e.g. "Copenhagen", "Sjælland", "Hovedstaden") where the site supports it.

### Priority 1: [YOUR_PRIMARY_ROLE_TYPE]

These match your strongest and most desired career direction.

```
site:jobindex.dk "[YOUR_PRIMARY_JOB_TITLE]" [YOUR_CITY]
site:jobindex.dk "[YOUR_KEY_SKILL]" [YOUR_CITY]
site:linkedin.com/jobs "[YOUR_PRIMARY_JOB_TITLE]" [YOUR_COUNTRY]
```

### Priority 2: [YOUR_DOMAIN_EXPERTISE]

These match your domain expertise.

```
site:jobindex.dk [YOUR_DOMAIN_KEYWORD_1] [YOUR_CITY] OR [YOUR_REGION]
site:jobindex.dk [YOUR_DOMAIN_KEYWORD_2] [YOUR_COUNTRY]
site:linkedin.com/jobs [YOUR_DOMAIN_KEYWORD_1] [YOUR_CITY] [YOUR_COUNTRY]
```

### Priority 3: [YOUR_ADJACENT_ROLE_TYPE]

Adjacent roles you could pivot into.

```
site:jobindex.dk "[YOUR_ADJACENT_TITLE_1]" [YOUR_KEY_SKILL] [YOUR_CITY]
site:jobindex.dk "[YOUR_ADJACENT_TITLE_2]" [YOUR_KEY_SKILL] [YOUR_CITY]
```

### Priority 4: Broader Technical / Consulting

Wider net for general technical roles.

```
site:jobindex.dk [YOUR_KEY_SKILL] developer [YOUR_CITY]
site:linkedin.com/jobs "[YOUR_KEY_SKILL] developer" [YOUR_CITY]
site:jobindex.dk "technical consultant" [YOUR_DOMAIN] [YOUR_CITY]
```

## Location Filter

When evaluating results, verify the job location is within reasonable commute distance from your home. Define acceptable areas:
- [YOUR_CITY] and surrounding areas
- [ACCEPTABLE_AREA_1]
- [ACCEPTABLE_AREA_2]
- [BORDERLINE_AREA] (borderline - ~X min by transit)
- [TOO_FAR_AREA] (too far)

## Date Filter

Only include jobs posted within the last 14 days, or with an application deadline that has not yet passed. If a posting date cannot be determined, include it but flag as "date unknown".

## Adapting Queries

If the user specifies a focus area, select queries from the matching category and also generate 2-3 custom queries for that focus. For example:
- "/scrape [focus_area]" -> relevant category queries + custom focus-specific queries

## Bangladesh Market

When the user targets Bangladesh (BD) roles, search these company career pages and job boards. Verified companies with React/JS/Python/Node tech stacks.

**BD IT Ecosystem Stats (2026):** ~4,500 IT firms (2,650+ BASIS-registered), 50,000+ CS graduates/year, $1.6B+ IT export revenue. Major tech clusters: Karwan Bazar, Shyamoli, Banani, Badda, Uttara. Developer rates: $15-55/hr. BD has one of the deepest and most cost-effective software engineering talent pools globally.

**Total tracked:** 91 companies from original 595 GitHub list + 26 major additional companies + 33 smaller/niche companies + 13 foreign companies hiring remotely from BD = **163 tracked BD companies**.

### BD Job Boards

```
site:linkedin.com/jobs "software engineer" "Bangladesh" OR "Dhaka"
site:linkedin.com/jobs "full stack" "Bangladesh" OR "Dhaka"
site:linkedin.com/jobs "frontend" OR "backend" developer Bangladesh
site:linkedin.com/jobs "react" OR "python" OR "node" Bangladesh
```

### BD Third-Party ATS (find openings at companies using these platforms)

```
site:jobs.smartrecruiters.com "Bangladesh" OR "Dhaka" software engineer
site:jobs.lever.co "Bangladesh" OR "Dhaka" engineer
site:ideascale.breezy.hr "Bangladesh" OR "Dhaka"
site:app.hrythmic.com "Bangladesh" OR "Dhaka"
site:bd.linkedin.com/jobs "react" OR "python" OR "node" "Dhaka"
site:bdjobs.com react OR python OR javascript OR node
site:dohaj.com software engineer Dhaka
site:dhakacareers.com software engineer
site:atb-jobs.com software engineer Dhaka
site:bdtechjobs.com "react" OR "python" OR "node"
```

### BD ATS Platform Queries (BD companies use these ATS providers)

```
site:easy.jobs "Bangladesh" OR "Dhaka" software engineer
site:hire.trakstar.com "Bangladesh" OR "Dhaka" engineer
site:factorialhr.com "Bangladesh" OR "Dhaka" developer
site:niyog.co "Dhaka" software engineer
site:app.airwork.ai "Dhaka" engineer
site:iitjobs.com "Dhaka" software engineer
site:recruitment.welldev.io "Dhaka" engineer
site:career.southtechgroup.com "programmer" OR "developer"
```

### BD Remote / Foreign Companies Hiring Bangladeshi Engineers

Foreign companies actively recruiting from Bangladesh for remote roles. These offer USD salaries ($500-$5,000+/mo) and often have BD founders or hiring managers.

| Company | Stack | Hiring Channel | Notes |
|---------|-------|---------------|-------|
| Field Nation (USA) | React, Node.js, PHP, React Native, AWS | https://jobs.lever.co/fieldnation?location=Dhaka | ✓ Lever ATS; Dhaka office + remote; SaaS marketplace |
| Alex Solutions (Australia) | React, TypeScript, Java, Material-UI, Redux | https://bd.linkedin.com/jobs/view/4122769358 | ✓ 100% remote; data catalog platform; senior full-stack |
| LAB3 (USA) | React, Vite, Node.js, Firebase, Firestore | https://jaabz.com/jobs/165888-full-stack-developer | ✓ Remote; US hours (9-5 EST); HIPAA experience preferred |
| AGT Software Partners | React, Node.js, TypeScript, GraphQL, Azure | https://builtin.com/job/full-stack-engineer/7884633 | ✓ 100% remote from anywhere; MERN stack; insurance/fintech |
| Anovium | Python, FastAPI, React, PostgreSQL | LinkedIn (remote - Bangladesh) | ✓ Remote; TMS/transportation systems |
| Chromatics AI | .NET C#, React.js, TypeScript, SQL | LinkedIn (remote - Bangladesh) | ✓ Remote; AI company; 100-150K BDT |
| CoverGo InsurTech | Various | LinkedIn (remote - Bangladesh) | ✓ Remote; insurtech |
| G2I Inc | JavaScript, Python, AI/ML | LinkedIn (remote - Bangladesh) | ✓ Remote; training AI data |
| MarketSwipe | Flutter, Next.js | LinkedIn (remote - Bangladesh) | ~Contractual remote |
| Wing Assistant | React Native | LinkedIn (remote - Bangladesh) | ~Remote; $830/mo |
| Volksbyte (Germany) | PHP, Laravel, React, JavaScript | LinkedIn / volksbyte.com | ✓ Remote from BD; EU hours overlap; 40-120K BDT |
| Trilogy (USA) | C# | LinkedIn (remote) | ✓ Remote; $60K/yr for senior C# devs |
| Dviz Technologies | Python, Django, React, Airflow | remoteok.com | ✓ Remote; AI-powered data platform |

### BD Facebook Groups & Pages for Tech Jobs

Active Facebook groups where BD companies post openings:
- **NodeJS Bangladesh** (FB group) - Node.js, full-stack roles
- **Programming Hero Community** (FB group) - junior/mid roles
- **BUET Career Club** (FB page) - quality listings from vetted companies
- **atB Jobs Bangladesh** (FB page) - job aggregator
- Company pages: Crystal Technology BD, Bluebay IT, Sincos Automation, Prime Bank Securities

### BD Facebook / Social Search Patterns

BD tech hiring happens heavily on Facebook groups and pages:
```
site:facebook.com "software engineer" Dhaka hiring
site:facebook.com "react developer" Bangladesh "we are hiring"
"job circular" "software engineer" site:facebook.com Dhaka
"IT job" Bangladesh site:facebook.com 2026
site:linkedin.com/company "software" Dhaka "51-200 employees"
```

### BD-Specific Google Dork Patterns
Search for company career pages or third-party ATS pages mentioning BD hiring:
```
"careers" OR "jobs" "Bangladesh" "software engineer" react
"we are hiring" Dhaka software engineer react
"open positions" Dhaka react developer
"bamboohr" OR "lever" OR "greenhouse" Dhaka engineer
"job" OR "career" site:*.com.bd software engineer
```

### Verified BD Company Career Pages

Career pages identified via web search (✓ = dedicated career page found; ~ = uses email/LinkedIn/third-party ATS). Use the URL column as the primary target when scraping.

| Company | Tech Stack | Career URL | Notes |
|---------|-----------|------------|-------|
| Adplay Technologies (VU Mobile) | JavaScript, React, WordPress | http://vumobile.biz/ | ~Email/LinkedIn recruitment; parent co. adplaytechnology.com |
| Adventure Dhaka Limited | Golang, JAVA, Flutter, React, Nextjs | https://www.atb-jobs.com/company-profile/adventure-dhaka-limited | ~Uses atB Jobs; also careers@bd.adventurekk.com |
| All Generation tech | Python, Go, Docker, Azure | https://allgentech.bamboohr.com/careers | ✓ BambooHR career page |
| Anchorblock Technology | JavaScript, Python, ReactJS, NodeJS, NestJS, Django | https://anchorblock.ai/ | ~Small team (~6), email-based hiring; hr@liberate-labs.com |
| Augmedix Inc. | Android, Java, JavaScript, AngularJS, NodeJS, AWS | https://augmedix.com.bd/career/ | ✓ Dedicated BD career page |
| Binate Solutions | Java, Python, Ruby | https://www.binate-solutions.com/ | ~Posts on bdjobs.com; email careers@binate-solutions.com |
| Bit Mascot (Pvt.) Ltd. | Java, JavaScript, Python, TensorFlow | https://www.bitmascot.com/careers/ | ✓ Career page + career@bitmascot.com |
| bkash | Java, Spring, PHP Laravel, Android, JavaScript | https://www.bkash.com/en/career | ✓ Dedicated career page |
| Bongo | JavaScript, Node, React, Android, iOS, AI | https://bongobd.com/ | ~Email careers@bongobd.com; posts on LinkedIn |
| Braincraft Limited | Java, Go, JavaScript, AngularJS, NodeJS | https://www.braincraftapps.com/work-with-us | ✓ Career page + career@braincraftapps.com |
| Cefalo Bangladesh | .Net, Python, Rails, React, iOS, Android | https://career.cefalo.com/ | ✓ Dedicated career page (Norway-based) |
| Circle Fintech | React, Javascript, Python, Node, Django | https://www.circlefintech.com/ | ~Small team (~5), email-based |
| Codemen Solutions | JavaScript, TypeScript, .NET, React, Node.js, AWS | http://www.codemen.com | ~Posts on dohaj.com, skill.jobs |
| COdesign | Nuxt, Django Rest Framework | https://co.design/careers/ | ✓ Career page |
| Daraz Bangladesh | PHP, Laravel, Vue, Node, GraphQL, Angular | https://careers.daraz.com/ | ✓ Career page (Alibaba Group) |
| DataSoft | Java, Spring Boot, Angular, Vue | https://datasoft-bd.com/career | ✓ Career page + career@datasoft-bd.com |
| Dingi Technologies | JavaScript, Java, React, Node, Flutter | https://www.dingi.tech/ | ~Small team (~7), email-based |
| Divine IT Limited | Python, Django, Flask, React, Node, Vue, Angular | https://www.divineit.net/ | ~Posts via LinkedIn/email; career page garbled |
| Dizi Nova Limited | JavaScript, C#, React, .Net, Flutter | http://www.dizinova.com/ | ~No dedicated career page found |
| Dynamic Solution Innovators (DSi) | Java, Spring Boot, Node.js, React, Next.js, AngularJS | https://app.hrythmic.com/recruit/openings/company/dsinnovators/ | ✓ Uses Hrythmic ATS |
| Embedded Logic Operations (ELO) | Node, React, Angular, Next.js, NestJS, Flutter | https://elobyte.com/ | ~Small team (~12), LinkedIn-based |
| Enosis Solutions (USA) | Java, PHP, Python, C# | https://enosisbd.pinpointhq.com/ | ✓ Uses Pinpoint ATS + career@enosisbd.com |
| Exabyting Technologies | Java, JavaScript, Node.js, Express.js, Python, Django | https://exabyting.com/join-our-team/ | ✓ Dedicated career page |
| Fieldnation (USA) | React, Node.js, TypeScript, AWS, Docker, K8s | https://jobs.lever.co/fieldnation?location=Dhaka | ✓ Lever ATS (Dhaka filter) |
| Flinkeo | Next.js, React, Python | https://flinkeo.online/ | ~Small, email-based |
| Flyte Solutions | JavaScript, Node, React, React Native | https://careers.smartrecruiters.com/FlyteSolutionsLtd | ✓ SmartRecruiters ATS |
| Fringecore | JavaScript, React, React Native, Node, ML | https://fringecore.sh/careers | ✓ Career page (Notion-based) |
| Furqan Software | Go, JavaScript, React, Firebase | https://furqansoftware.com/careers/ | ✓ Career page + careers@furqansoftware.com |
| GeekSSort | Laravel, Flutter, ReactJs, VueJS, NextJS | https://geekssort.com/career-page/ | ✓ Career page + careers@geekssort.com |
| Giga Tech Limited (BEXIMCO) | Java, Python, Django, JavaScript, .NET | https://gigatechltd.com/career/ | ✓ Career page (BEXIMCO group) |
| Golden Harvest InfoTech (GHIT) | Java, Spring, .Net, React JS | https://jobs.bdjobs.com/companyofferedjobs.asp?alias=0&companyname=Golden+Harvest+InfoTech&id=59542 | ~Uses bdjobs.com for postings |
| Grit Technologies Limited | Javascript, Python, Go, React Native, Docker, AWS | https://www.grit0.com/ | ~Posts on dohaj.com, LinkedIn |
| Hogarth Dhaka | JavaScript, React, Node, AWS | https://www.hogarth.com/careers | ✓ Career page (WPP group) |
| hSenid Mobile Solutions Limited | Java, NodeJS, Spring, AWS | https://hsenidmobile.com/careers/ | ✓ Career page + careers+bdde@hsenidmobile.com |
| HypeScout | JavaScript, React, Node, Flutter, Swift | https://www.hypescout.co/ | ~Small team (~7-9), LinkedIn |
| IdeaScale Bangladesh | Java, Spring, ReactJS | https://ideascale.breezy.hr/ | ✓ Uses Breezy ATS |
| InfancyIT | PHP, Java, JavaScript, Node.js, Vue.js, React.js | http://www.infancyit.com | ~Small team (~6), email-based (info@infancyit.com) |
| Inflack Limited | PHP, Java, JavaScript, Python, Django | http://inflack.com/ | ~Small team (~8), email-based |
| Inovace Technologies | PHP, Python, JavaScript, Angular, Vue | https://inovacetech.com/ | ~Email hr@inovacetech.com; posts on dhakacareers.com |
| Inument | Dotnet, Javascript, Java, NodeJS, React, Flutter | https://inument.com/careers/ | ✓ Career page |
| Invento Software Limited | JavaScript, Python, Django, WordPress, PHP | https://invento.com.bd/career/ | ✓ Career page |
| IXORA Solution | React, Vue, Typescript, NodeJS, Django, Flutter | https://ixorasolution.com | ~Not verified; small company |
| Kite Games Studio | Swift, React, Kotlin, PyTorch | https://www.kitegamesstudio.com | ✓ Career page on site |
| Kona Software Lab | Java, JavaScript, Android, AI, Blockchain | https://konasl.com/careers | ✓ Career page |
| LightCastle Partners | JavaScript, React, Node | https://lightcastlepartners.com/careers/ | ✓ Career page (consulting firm) |
| Mazegeek Technologies BD Ltd. | PHP, JavaScript, Node.js, Vue.js, Angular, React, Python | https://careers.smartrecruiters.com/MazeGeekTechnologiesBDLtd | ✓ SmartRecruiters ATS |
| ME SOLshare Ltd. | Java, Android, Python (Django), JavaScript (ReactJS) | https://solshare.com/career/ | ✓ Career page (climate-tech) |
| Misfit Technologies | Python, Django, Ruby, JavaScript, React, AI, ML | https://misfit.tech/ | ~HQ in Singapore; BD office small |
| MonstarLab Bangladesh | Java Spring, Laravel, NextJS, NestJS, Flutter | https://monstar-lab.com/bd/ | ✓ Global consultancy (Japan HQ) |
| Namespace IT | Laravel, React, Next.js, Django, ML | https://namespaceit.com/career/current_job_opening | ✓ Career page + career@namespaceit.com |
| NetCoden Inc | Node.js, Vue.js, React, PHP, Laravel | https://netcoden.com/ | ~Small; email-based |
| Netizen IT Limited | Java, Python, Spring, Android, ReactJS, Angular, AWS | https://netizenit.com/ | ~Career page has US roles; email careers@numerique.com |
| Newroz Technologies Limited | Java, Spring Boot, Flutter, Kotlin, React | https://www.newroztech.com/ | ✓ Active on LinkedIn; career@newroztech.com |
| Nogor Solutions Limited | PHP Laravel, JavaScript, Vue | https://nogorsolutions.com/career | ✓ Career page + career@nogorsolutions.com |
| Onecodesoft | PHP, Javascript, Python, Flutter, NodeJs, ReactJS | https://onecodesoft.com/career | ✓ Career page |
| Optimizely (formerly Newscred) (USA) | Python, NodeJS, Angular2, MongoDB | https://www.optimizely.com/ | ✓ Global careers page; Dhaka office |
| Orange Toolz | Laravel, AngularJS, React Native, NodeJS, AWS | https://orangetoolz.com/ | ~Email-based hiring |
| OrvionSoft | C#, ASP.NET Core, Angular, React, NextJS, NodeJS | https://www.orvionsoft.com/ | ✓ Career page on site |
| Paperfly Ltd | React, Vue, PHP, Laravel | https://www.paperfly.com.bd/ | ✓ Site active (was down during check) |
| Pathao Ltd | Go, PHP, Nodejs, K8s, Android, iOS | https://pathao.com/ | ✓ Major platform; career page likely |
| Penta Global Ltd | Java, Python, React, Node, PostgreSQL, K8s | https://www.pentabd.com/ | ✓ Site reachable |
| Portonics Limited | Android, iOS, PHP, React, Nodejs, Python | http://portonics.com/ | ✓ Site reachable |
| RiseUp Labs | Flutter, Swift, Typescript, React, Java, Django, NodeJS | https://riseuplabs.com | ✓ Site reachable |
| Robust Research And Development Ltd. | Flutter, Typescript, NextJS, Python | https://rrad.ltd/ | ✓ Site reachable |
| Rokomari | Flutter, Java, Spring, NextJS, Python | https://www.rokomari.com/ | ✓ Major BD e-commerce platform |
| SCT Bangla Limited | PHP, JavaScript, React, Angular, Flutter | https://www.sct-bangla.com/ | ✓ Site reachable |
| SELISE Digital Platforms (Switzerland) | Android, iOS, AngularJS, NodeJS, Python, .Net | https://selisegroup.com/ | ✓ Swiss company with BD office |
| ShareTrip | PHP, NodeJS, ReactJS, Android, iOS, AWS | https://sharetrip.net/ | ✓ BD travel platform |
| ShellBeeHaken | Java, Javascript, React, Next.Js, Spring Boot, AWS | https://shellbeehaken.com/ | ✓ Site reachable |
| Shopup | JavaScript, Node, React, Ruby on Rails, Flutter, AWS | https://shopup.com.bd/ | ✓ BD e-commerce platform |
| Silicon Orchard Limited | PHP, NodeJS, ReactJS, Blockchain | https://www.siliconorchard.com/ | ✓ Site reachable |
| Softzino Technologies | Android, iOS, React, React Native, JavaScript, Vue, Flutter | https://softzino.com/ | ✓ Site reachable |
| SovWare | PHP, JavaScript, ReactJS, Flutter | https://www.sovware.com/ | ✓ Site reachable (WordPress plugins) |
| Square Health Ltd. | Java, Angular, React, Android | https://career.squarehealth.com.bd/ | ✓ Career page (was 503 during check) |
| SSL Wireless | Java, JavaScript, PHP, Laravel | https://www.sslwireless.com/ | ✓ Site reachable |
| TAPPWARE Solutions Limited | PHP, Laravel, Django, Java, J2EE, VueJS, Flutter | https://tappware.com/ | ✓ Site reachable |
| TechCare | Android, Java, Node | https://www.techcarebd.com/ | ✓ Site reachable |
| Technext Limited | JavaScript, React, Next.js, .NET Core | https://technext.it/ | ✓ Site reachable |
| Technohaven Company Limited | NodeJS, Angular, React, Android, ML, Blockchain | https://technohaven.com | ✓ Site reachable |
| TechnoNext | JavaScript, React, Golang, Flutter | https://www.digigate360.com/ | ✓ Site reachable |
| Telenor Health A/S | PHP, Nodejs, JavaScript/React, Python/Django, iOS, Android | https://telenorhealth.com | ✓ Site reachable (Telenor group) |
| Themeperch Limited | JavaScript, React, Next.js, Tailwind CSS | https://themeperch.net | ✓ Site reachable |
| ThemeXpert | PHP, Laravel, JavaScript, React | https://www.themexpert.com/ | ✓ Site reachable |
| TimeTackle (US) | Java, Springboot, React, JavaScript | https://www.timetackle.com/ | ✓ Site reachable |
| TruckLagbe | JavaScript, Node, Angular, Flutter | https://trucklagbe.com | ✓ Site reachable |
| UPAY (UCB Fintech) | Python, Django, Flask, JavaScript, React, Node | https://www.upaybd.com/ | ✓ Site reachable |
| Vivasoft Limited | Java, C#, React.js, GoLang, Python, Flutter | https://www.vivasoftltd.com/ | ✓ Site reachable (200+ employees) |
| weDevs Ltd | PHP, WordPress, VueJs, Flutter | https://wedevs.com | ✓ Site reachable |
| Workspace InfoTech Limited | Java, Python, Django, Angular, ReactJS | https://www.workspaceit.com | ✓ Site reachable |
| WPDeveloper | PHP, WordPress, JavaScript, Vue.js, ReactJS | https://wpdeveloper.com | ✓ Site reachable |
| XpeedLab | nodeJS, ReactJS, Angular, Java, Flutter, MongoDB | https://xpeedlab.tech/ | ✓ Site reachable |
| YOTECH Limited | JavaScript, Node, Angular, React, Next, Flutter | https://www.yotech.ltd | ✓ Site reachable |
| Zaynax Limited | JavaScript, Node, React, Next, Android, iOS | http://www.zaynax.com | ✓ Site reachable |

### Additional BD Tech Companies (beyond original 595 GitHub list)

Notable Bangladeshi IT companies discovered via web research that were NOT in the original GitHub AsciiDoc table. These hire for fullstack/frontend/backend/software engineer/AI roles.

| Company | Tech Stack | Career URL | Notes |
|---------|-----------|------------|-------|
| Brain Station 23 | React, Python, Java, Node, AI/ML | https://brainstation-23.easy.jobs/ | ✓ easy.jobs ATS; 850+ employees; CMMI L3, ISO 27001; founded 2006 |
| BJIT Group | Java, Python, React, PHP, AI/IoT | https://bjitgroup.com/career | ✓ Career page (no current openings); 1000+ emp; Japan-Bangladesh JV |
| Kaz Software | PHP, Python, React, RoR | https://kazsoftware.hire.trakstar.com/ | ✓ Trakstar ATS; 150+ emp; founded 2004 |
| Therap (BD) Ltd | Java, React, Python, DevOps | https://therap.hire.trakstar.com/ | ✓ Trakstar ATS (10+ openings including React Developer); 400+ emp; US healthcare SaaS |
| Tiger IT Bangladesh | .NET, Java, PHP, Mobile | https://www.tigerit.com/ + careers@tigerit.com | ~Email/LinkedIn/bdjobs; 200+ emp; biometric ID solutions |
| Dream71 Bangladesh | Laravel, Ruby on Rails, React, Vue | https://dream71.com/career | ✓ Career page (no current jobs but active on LinkedIn/dohaj); 70+ emp; e-Gov |
| REVE Systems | Java, Spring Boot, JSP, JavaScript | https://www.revesoft.com/career | ✓ Career page with resume drop; 200+ emp; telecom/VoIP |
| SouthTech Group | .NET, C#, Python, Angular, VB.NET | https://career.southtechgroup.com/ | ✓ Career page; 120+ emp; ISO 9001; founded 1996 |
| WellDev Bangladesh | Java, Angular, .NET, TypeScript | https://recruitment.welldev.io/ | ✓ Own RMS; 180+ emp; Swiss-owned; hires often |
| Astha IT (AIT) | .NET, Python, React, AWS, Terraform | https://ait.inc/career/ | ✓ Career page (multiple open roles: Backend, Cloud); 100+ emp; Fortune 500 clients |
| Intelligent Machines | Node.js, TypeScript, Python, AI/ML | https://intelmachines.ai/career | ✓ Career page; 20+ emp; AI products; clients include BAT, IDLC |
| Ollyo | React, PHP, MySQL, WordPress | https://ollyo.com/careers/ | ✓ Career page + FactorialHR ATS; SaaS products |
| ReliSource Technologies | .NET, Next.js, Python, AI, Azure | https://www.relisource.com/careers/ | ✓ Career page (16+ openings: AI, DevOps, .NET); 300+ emp; Boston HQ |
| Craftsmen | Python, AWS, streaming media | https://careers.craftsmensoftware.com/ | ✓ SmartRecruiters (Senior Backend open); 80+ emp; Norwegian clients |
| Sazim | React, Node.js, Java, Spring Boot, TypeScript | https://www.sazim.io/careers | ✓ Career page (hybrid in Mohakhali); 30+ emp; founding 2021 |
| Markopolo AI | Python, TypeScript, React, NestJS, AI | https://markopolo.ai/careers + hr@markopolo.ai | ✓ Career page + email; 20+ emp; VC-backed (HF0); behavioral AI |
| Nascenia | Ruby on Rails, PHP, .NET | https://nascenia.com/careers/ | ✓ Career page with form; 50+ emp; BASIS award winner |
| Mediusware | Full-stack, AI, SaaS, mobile | https://mediusware.com/career | ✓ Career page (3 openings); Upwork Top Rated; hr@mediusware.com |
| Pridesys IT | Angular, React, Java, Spring Boot | https://pridesys.com/careers/ | ✓ Career page (multiple engineer openings); CMMI L3, ISO 27001; ERP |
| Fiber@Home Global | Python, Django, JavaScript, MySQL, Linux | https://www.fiberathome.net/career | ✓ Career page; 900+ emp; telecom infrastructure |
| Polygon Technology | Laravel, PHP, Python, React, Vue | https://careers.smartrecruiters.com/polygontechnology | ✓ SmartRecruiters ATS; 50+ emp |
| Bdtask Limited | Python/Django, PHP, React, React Native | https://www.bdtask.com/career.php | ✓ Career page (multiple openings); hr@bdtask.com |
| Soft BD Limited | PHP, JavaScript, DevOps, UI/UX | https://www.softbd.com/career | ✓ Career page; 80+ emp; founded 2006 |
| Daffodil Software Ltd | Various (Java, PHP, mobile) | https://www.daffodilsw.com/career/ | ✓ Career page; part of Daffodil Group |
| Grameen Solutions | Java, PHP, mobile | career@grameensolutions.com | ~Email-based hiring; Nobel Peace Prize affiliated |
| Dexian Bangladesh | Python, AI/ML, cloud | https://dexian.com/about-us/locations/dhaka-bangladesh/ | ~Staffing firm; hires for client companies; walk-in events |
| SELISE Digital Platforms | Java, Angular, React, Node, .NET, Python | https://selisegroup.com/job-application/ + https://selisegroup.com/about-us/#selise-career | ✓ Swiss HQ; 450+ engineers in BD; AWS/Microsoft Gold Partner |
| LeadSoft Bangladesh | Java, React, Angular, Blockchain, IoT | https://leadsoft.com.bd/career | ✓ CMMI L5; 300+ emp; founded 1999; one of oldest in BD |
| Riseup Labs | React, Angular, Vue, Node, Python, Flutter | https://riseuplabs.com/career/ | ✓ ISO 27001, SOC 2; 150+ emp; clients: UNICEF, UNDP, WHO |
| Genex Infosys PLC | Java, Python, .NET, Angular, React | https://www.genexinfosys.com/career | ✓ Publicly listed IT company; large workforce; BPO + software |
| Inovio | Python, Django, React, Angular, Swift | https://www.inovio.com.bd/ | ~Smaller firm; full-stack web/mobile |
| Hawar IT | Web, mobile, custom software | https://hawarit.com/ | ~Small dev shop |
| 6senseHQ / 6sense Technologies | React, Node, AI, IoT | https://6sensehq.com/ | ~30+ offshore experts; FinTech, Health, EdTech |
| jayedcorp | PHP, Laravel, Python, Django, Node, React | https://jayedcorp.com/ | ~Full-stack dev services; GCP/AWS |
| Volksbyte (German-based) | JavaScript, React, PHP, Laravel, HTML Canvas | https://volksbyte.com/ + apply via LinkedIn | ✓ German company hiring BD remote; PHP/React stack |
| Kodestorm | Web, mobile, cloud solutions | https://kodestorm.com/ | ~Small dev shop |
| Olivine | Laravel, PHP, Vue.js, cloud | https://olivine.com.bd/ | ~Backend/web dev services |
| Smart Software Ltd | ERP, web, eCommerce | https://smartsoftwareltd.com/ | ~ERP & eCommerce solutions |
| Ontik Technology | WEB3, cloud, full-stack | https://ontiktechnology.com/ | ~Tech consultancy since 2016 |
| AppifyDevs / Appifylab | NestJS, Laravel, Node, React, Shopify | https://appifydevs.com/ + LinkedIn (AppifyDevs) | ~Hiring backend devs (remote); Shopify/NestJS focus; site sometimes unstable |
| Core Devs Ltd | Node.js, Python, React, MongoDB, Web3, AI | https://www.coredevs.io/Careers.html + https://career.coredevsltd.com/ | ✓ Career page (multiple open roles: Node.js, Python, Full-Stack, Automation); web3/blockchain focus; 23 emp |
| SoftStandard Solutions | Java, Python, Kafka, Hadoop, big data | https://softstandard.com/career/ | ~US-based IT staffing firm; 12 emp in BD; jobs mostly require US relocation; hr@softstandard.com |
| Technix Technology | React, JavaScript, TypeScript | https://technixtechnology.com/ | ~React/Next.js development shop |
| Star Computer Systems Limited (SCSL) | C# .NET, React, TypeScript, Redux | https://www.stargroup-bd.com/career | ✓ Career page (software engineer openings); part of Star Group |
| Grit System | ReactJS, NextJS, TypeScript, MUI | https://gritsystem.com/ | ~React-focused dev shop in Mirpur |
| Intellixio | Next.js, React, TypeScript, Tailwind | https://intellixio.com/ | ~On-site in Uttara; Next.js focus |
| M360 ICT | React, Next.js, TypeScript, GraphQL | https://m360ict.com/ | ✓ Hiring frontend devs; Banani office |
| Klinkode | Laravel, React | https://klinkode.com/ | ~Laravel + React dev shop |
| Leadsync AI | React, Next.js, TypeScript | https://leadsyncai.com/ | ~AI startup; Uttara office |
| BYSL Global Technology Group | AngularJS, Node.js, VR, AI/ML | https://byslglobal.com/ | ~Hiring full-stack engineers |
| Startsmartz Technologies | Next.js, NestJS, PostgreSQL, Docker, n8n | https://startsmartz.net/ + info@startsmartz.net | ✓ Hiring senior AI full-stack dev; AI workflow automation |
| GlobeXHire | Laravel, Python, Vue.js, K8s, Kafka | https://globexhire.com/ | ✓ Hiring full-stack dev; cloud-native |
| Navieasoft PLC | Laravel, Node.js, React, Vue, Next.js | https://navieasoft.com/ | ~AdTech SaaS; 5-10yr experience roles |
| Tekarsh | Modern frontend, backend, microservices | https://tekarsh.com/ | ✓ Hiring senior SWE (150K BDT); payment platforms |
| TechZoddha | Python, JavaScript, LLM, AI agents | https://techzoddha.com/ | ~AI agent development studio |
| Bengal Byte | AI, software, talent acquisition | https://bengalbyte.ai/ | ~AI-first tech company; Nikunja office |
| Miaki | Python/Django, Node.js, React | https://miaki.co/ | ✓ Multi-country service provider; hybrid in Dhaka |
| Dakpeon24 IT | React, Python | https://dakpeon24.com/ | ~Hiring full-stack (React + Python); remote |
| BD BOOKS LIMITED | Python FastAPI, React, Next.js, MERN, Docker | Posted on dohaj.com (search "BD BOOKS LIMITED" on dohaj) | ~Posts on dohaj.com (5 vacancies); Purana Paltan; edtech/ecommerce platform |
| Terabyte AI | React, Next.js, Figma, Tailwind, Django | https://terabyteai.com/ | ✓ AI dev studio hiring frontend; remote |
| Dorik | Node.js, TypeScript, MongoDB, PostgreSQL, GraphQL, Redis | https://dorik.com/ + career@dorik.com | ✓ Website builder (YC-style); hiring senior backend; 160-250K BDT + equity; remote/Sylhet |
| Crystal Technology Bangladesh Ltd | Full-stack (varied stack) | Facebook: Crystal Technology Bangladesh Ltd | ~Posts hiring on Facebook; small-mid size firm |
| Bluebay IT Limited | Next.js, React, Redux, MUI, Angular, Vue | https://bluebayit.com/ | ~Smaller dev shop; hires through Facebook/LinkedIn/postings |
| Sincos Automation Technologies Ltd | Node.js, Angular, Java, Spring Boot, IoT | https://sincosbd.com/ | ~Industrial automation; IoT division hires software engineers |
| Synesis IT PLC | Java, React, React Native, AI/ML, Oracle, Python | https://synesisitltd.com/ + LinkedIn (Synesis IT PLC) | ✓ CMMI L3, ISO 27001, ISO 9001; 550+ emp; e-Governance specialist; hiring AI/React/SQA; Kawran Bazar |
| LEADS Corporation Limited | Java, Spring, DevOps, software engineering | https://leads.com.bd/current-vacancies/ | ✓ Career page (hiring DevSecOps, SWE); 200+ emp, founded 1992; banking/insurance/ERP; Mirpur |
| Sheba Platform Ltd | Laravel, PHP, MySQL, Elasticsearch, Redis | https://careers.smartrecruiters.com/ShebaPlatformLimited | ✓ SmartRecruiters ATS; 146 emp; service marketplace (sheba.xyz); hiring Sr. Backend (Laravel) |
| Shohoz | PHP, Laravel, Angular, Node.js, Python, Flutter, Docker, K8s | https://www.shohoz.com/ + LinkedIn (Shohoz) | ✓ Online ticketing platform; 124 emp; $18.4M funding; Banani; Director of Engineering role |
| Apsis Solutions Ltd | Java, Spring, full-stack, cloud, managed services | https://apsissolutions.com/career/ | ✓ Career page; 111 emp, founded 2011; Banani; CRM/ERP/fintech/telecom; global delivery |
| ShopUp | Go (Golang), React, React Native, PostgreSQL, Docker | https://shopup.org/career + SmartRecruiters | ✓ $75M Series B (Valar); B2B commerce (Mokam, REDX, Baki); Tejgaon; hiring Full Stack (Go+React) |
| Chaldal | F#, .NET Core, React, React Native, TypeScript, Python, Scala | https://chaldal.tech/ | ✓ YC-backed online grocery; 237 emp; Banani; hiring Fresh Grad SWE + Senior SWE; functional programming |
| OnnoRokom Software Ltd | Web dev, enterprise apps, system integration | https://onnorokomsoftware.com/ + LinkedIn | ~47 emp, founded 2011; Kawran Bazar; hires via LinkedIn forms; part of OnnoRokom Group |
| Orange Business Development Ltd | Web dev, e-Governance, LMS, mobile apps, UX/UI | https://orangebd.com/ + LinkedIn (orangebd) | ~42 emp; e-Governance/e-Newspaper/LMS; award-winning; Baridhara DOHS; founded 2005 |
| Bondstein Technologies Ltd | Android (Kotlin), iOS (Swift), IoT, Python, Django, ML | https://careers.smartrecruiters.com/BondsteinTechnologiesLtd | ✓ SmartRecruiters ATS; 36 emp; IoT leader (Runner Group); Tejgaon; hiring Jr Mobile SWE + ML Intern |
| NexKraft Limited | PHP, JavaScript, React, Python, software dev | https://nexkraft.com/career/ | ✓ Career page + hello@nexkraft.com; 33 emp; Lake Circus; hiring PHP Dev (Intern), PM |
| TechNext Limited | Node.js, React, Python/Django, PHP, UI/UX | https://technext.it/careers/ + Freshteam ATS | ✓ Freshteam ATS + career page; Sylhet/Dhaka; SaaS (MailBluster, ThemeWagon); hiring Full-Stack, QA |
| Kolpolok Limited | Odoo, Flutter, Android, iOS, Python, VPN tech | https://kolpolok.com/career/ + career@kolpolok.com | ✓ Career page + email; ISO 9001:2015; VPN/SaaS; Shyamoli; hiring Trainee SWE, Odoo Dev |
| iXora Solution Ltd | Python, Angular, .NET, React, Odoo, PostgreSQL | https://ixorasolution.com/career/ | ✓ Career page; ERP/Odoo specialist; Mirpur; hiring Data Engineer, Full-Stack, Odoo Dev |
| Orange Solutions Ltd | Full-stack, ERP, mobile apps, IoT, cloud, cyber security | https://makeitorange.com.bd/ + LinkedIn (Orange Solutions Ltd) | ~18+ years, ISO 9001:2015; 250+ clients; also known as Make IT Orange |
| Bangladesh Software Solution | Node.js, Python/Django, Databricks, React, cloud | https://bssoln.com/ + LinkedIn (Bangladesh Software Solution) | ~26 emp; Dhanmondi; hires for Dutch clients (Databricks, Node.js); hybrid work |
| SOFTIC | Flutter, Dart, AI/ML, digital marketing | https://softic.ai/ + LinkedIn (softicai) | ~13 emp, founded 2022; Dhaka; AI & custom software; hiring Flutter Dev |
| Onethread | Node.js, Express, MongoDB, MySQL, React, JS | https://onethreadapp.com/ + hires via LinkedIn/Interactive Cares | ~13 emp; BD's first homegrown PM SaaS; remote team; hiring Node.js Dev (remote) |
| Apploye (BD team) | React Native, Python/Django, React, PostgreSQL, Docker, K8s | https://apploye.com/ + LinkedIn (Apploye) | ~25 emp (24 in BD); time tracking SaaS (US-registered); BD-based engineering team |
| Shohoz Software | POS software, software sales | https://shohozsoftware.com/career/ | ✓ Career page; POS software solutions; hiring Software Sales Intern |
| STITBD | Node.js, web dev, digital marketing, CCTV | https://stitbd.com/ + LinkedIn (stitbd) | ~13 emp; Dhaka; small full-service IT firm; hiring Node.js Developer |
| AKIJ iBOS Limited | ASP.NET, PHP, Node.js, Laravel, Angular, React, Vue, Flutter | https://ibos.io/career/ | ✓ Career page + submit resume; 192 emp (106 tech); part of Akij Group; Lalmatia; hiring SQA, SWE |
| BRAC IT Services (biTS) | Java, Spring, PostgreSQL, Azure, DevOps, data | https://www.bracits.com/career/ | ✓ Career page; 567 emp; Gulshan; hiring Java SWE, Data Engineer, Lead DevOps; BRAC's IT arm |
| Divine IT Limited | Python, Django, React, Angular, ERP | https://www.divineit.net/about/careers/ | ✓ Career page; 114 emp; CMMI L3, ISO certified; Uttara; hiring Trainee SWE (Python); ERP products |
| Akij Group IT Department | .NET (ASP.NET Core, C#), React, Next.js, Oracle, Redis | Hiring via dohaj.com, LinkedIn (Akij Group IT) | ~Large conglomerate IT dept; hiring Technical Lead (Textile ERP), SWE; .NET + React stack; 30+ IT staff |
| Pubali Bank PLC (IT Division) | Java, software development, banking systems | https://dohaj.com/search?q=Pubali+Bank | ~Hiring 40+ software developers; 518 branches; largest private bank in BD; tech-forward |
| Pakiza Software Limited | Cripton Pro ERP, React, .NET, Oracle, AI/BI | https://pakizasoftware.com/ + LinkedIn (Pakiza Software) | ~Textile/RMG ERP specialist; CMMI L3; 75+ professionals; 41 years of group experience |
| Betopia Group (IT) | Node.js, React, Next.js, full-stack development | https://bdjobs.com/h/details/1469708 (Frontend Dev posting) | ~5,000+ emp group; Gulshan; hiring Frontend Dev (Node.js + React/Next.js); diversified conglomerate |
| BRAC Bank PLC (Technology Division) | Java, Spring, microservices, mobile, API | https://hotjobs.bdjobs.com/jobs/bracbank/ (Tech Talents program) | ~Leading bank hiring Tech Talents; CSE/EEE graduates; in-house software development |
| Monstarlab Bangladesh | Full-stack, React, Node, AI, digital consulting | https://monstar-lab.com/bd/ + LinkedIn (monstarlab) | ~23+ emp in BD; Japanese global digital consultancy; 28 countries; Mohakhali office |
| Dcastalia Limited | Web dev, mobile apps, DevOps, custom SW | https://dcastalia.com/ + info@dcastalia.com | ~Banani; founded 2009; full-service software development; government + private clients |
| ADN DigiNet Ltd | Web dev, mobile apps, cloud, business automation | https://www.adndigitalbd.com/ + LinkedIn (ADN Digital) | ~98 emp, founded 2017; Dhaka; offices in Sweden & Australia; software dev + messaging |
| Jatri | Node.js, React, mobile (Flutter), transit tech | https://jatri.co/career + career@jatri.co | ✓ Career page + email; transit/mobility app; hiring Sales, Platform; VC-backed startup |
| MN Infotech | Web dev, app dev, BPO, digital services | https://mninfotech.com/ + LinkedIn (MN Infotech) | ~210 emp (33 in BD/rest offshore); Demra; hires Client Coordinators, night shift |
| TechnoVista Ltd | Full-stack, enterprise software, outsourcing | https://technovista.com.bd/ + info@technovista.com.bd | ~CMMI L3; founded 1999; software design, development, maintenance, outsourcing |
| Pioneer Alpha Ltd | R&D software, IT-enabled products/services | https://pioneeralpha.com/ + hello@pioneeralpha.com | ~Emerging R&D software company; Dhaka; verified GitHub org (32 public repos) |
| Excel IT AI Bangladesh | Web apps, mobile apps, enterprise SW | https://www.excelitai.com/ + info@excelitai.com | ~Dhaka; software dev company; GitHub org with 34 public repos; full-stack |
| Strawberry Dhaka Tech Ltd (SDT) | Enterprise systems, full-stack | https://sdt.com.bd/ + LinkedIn (strawberrytechlimited) | ~Mirpur DOHS; enterprise software solutions; GitHub org; founding 2025 |
| Dhrubok Infotech Services Ltd | iOS, Android, web, enterprise solutions | https://dhrubokinfotech.com/ + info@dhrubokinfotech.com | ~Shyamoli; built Dhaka Bank Go+ mobile app; full-service app development |
| EasySoft Bangladesh Ltd | Retail POS, ERP, VAT, accounting, HR, e-commerce | https://easysoft.com.bd/ | ~23+ years; largest retail software provider in BD; POS/ERP/Hospital solutions |
| Naas Solutions Limited | C#, ASP.NET MVC, .NET Core, Web API, React/Vue | https://bdjobs.com/h/details/1485627 (SWE posting) | ~Banasree; hiring .NET developers; custom software solutions |
| Smart Software Ltd | Web dev, e-commerce, design, cyber security | https://smartsoftware.com.bd/ + LinkedIn (Smart Software Ltd) | ~35 emp; Dhaka; full-service web/software; also at smartsoftwareltd.com |
| Advanced Software Development (ASD) | Banking apps, ERP, banking software | https://asdbd.com/ + info@asdbd.com | ~25 emp; Gulshan; founded 2004; banking/ERP software specialist |
| SSL Wireless | Java, JavaScript, PHP, Laravel | https://www.sslwireless.com/ | ✓ Site reachable; fintech/mobile financial services |
| Singularity Limited | Web, mobile, AI, data science | https://singularity.net.bd/ | ~BASIS member; software & IT services |
| Apurba Technologies Ltd | PHP, WordPress, web dev | https://apurba.com.bd/ | ~BASIS member; software development |
| ATI Limited | Java, Android, web | http://atibd.com/ | ~BASIS member; IT solutions |
| Alchemy Software Limited | Java, Oracle, PHP, .NET, Android | https://alchemy-bd.com/ | ~Chittagong; BASIS member; established software co |
| AlgorixIT LTD | Web, mobile | https://algorixit.com/ | ~Dhanmondi; software dev |
| BlueBees Limited | Web, mobile, DevOps, cloud | https://bluebees.ai/ | ~BASIS member; tech solutions |
| Genuity Systems Ltd | Java, Spring, Hibernate | https://genuitybd.com/ | ~BASIS member; software dev |
| Integrated Software & Technologies Ltd | Java, .NET, web | https://intechbd.com/ | ~BASIS member; software solutions |
| Isratts Technologies | Web, mobile, e-commerce | https://isratts.com/ | ~BASIS member |
| ITmedicus | Health IT, web, mobile | https://itmedicus.com/ | ~Healthcare software; BASIS member |
| Kompass Technologies Limited | PHP, Java, web | https://kompasstech.net/ | ~BASIS member |
| Kovair Software Bangladesh | ALM, DevOps, SaaS | https://kovair.com/ | ~US-headquartered; BD office; ALM solutions |
| Medina Tech Ltd | PHP, Laravel, web | https://medina-tech.com/ | ~BASIS member |
| Metafour Asia | Telecom, OSS/BSS | https://metafour.com/ | ~UK-headquartered; BD office; telecom software |
| Mevrik Ltd | Web, mobile, e-commerce | https://mevrik.com/ | ~BASIS member |
| Millennium Information Solution Ltd | Java, web, mobile | https://millenniumit.com.bd/ | ~BASIS member; hi-tech park tenant |
| MononSoft Ltd (JMI Group) | Java, Android, web | https://mononsoft.com/ | ~Part of JMI Group; software dev |
| NeerLab | Android, iOS, React Native | https://neerlab.com/ | ~BASIS member; app development |
| Newgen Technology Ltd | Java, PHP, Android | http://newgenbd.com/ | ~BASIS member |
| Nextech Limited | PHP, Laravel, web | https://nextechbd.com/ | ~BASIS member |
| Nybbles System Limited (NybSys) | Java, Android, web | https://nybbles.com/ | ~BASIS member; software dev |
| PixelNet Technologies Ltd | Web, mobile, cloud | https://pixellab.co/ | ~BASIS member |
| Progoti Systems Limited | Java, ERP, web | https://progotisystems.com/ | ~BASIS member |
| Remotion IT | Web, mobile, AI | https://remotionit.com/ | ~BASIS member |
| Renessa Info Systems Ltd | Java, PHP, web | https://renessa.com.bd/ | ~BASIS member |
| ServicEngine Ltd | Web, mobile, cloud | https://servicenginebd.com/ | ~BASIS member |
| Spring Rain IT | PHP, Laravel, web | https://springrainit.com/ | ~BASIS member |
| Strativ BD Ltd | React, Node, Python, AWS, React Native | https://strativbd.com/ + LinkedIn | ~BASIS member; software dev & consulting |
| Streams Tech Inc | .NET, web, mobile | https://streamstech.com/ | ~BASIS member; software solutions |
| SOFTBOFFIN | Web, mobile, AI | https://softboffin.com/ | ~BASIS member |
| Software Lighthouse | PHP, Laravel, Vue, web | https://softwarelighthouse.net/ | ~BASIS member |
| SoftwarePeople | .NET, web | https://softwarepeople.com.bd/ | ~BASIS member |
| Sonali Polaris FT Limited | Core banking, financial SW | https://sonalipolaris.com/ | ~JV between Sonali Bank & Polaris; core banking |
| SPeeddigit PVT | Web, mobile, ITES | https://speedigit.com/ | ~BASIS member |
| SSD-TECH | Java, .NET, web, mobile | https://ssd-tech.com/ | ~BASIS member; Systems Solutions & Dev Tech |
| Telcobright Limited | Telecom, VoIP, BSS/OSS | https://telcobright.com/ | ~BASIS member; telecom software |
| Vantage Labs BD | Web, mobile, cloud | https://vantagelabsbd.com/ | ~BASIS member |
| Wafi Solutions | Android, iOS, web, cloud | https://wafisolutions.com/ | ~BASIS member |
| IBCS-Primax | Java, .NET, ERP | https://ibcsprimax.com/ | ~BASIS member; software solutions |
| InterCloud Ltd | Cloud, connectivity, VoIP | https://intercloudbd.com/ | ~BASIS member; cloud & telecom services |
| MARS Solutions Ltd | Java, Android, web | https://marssolutionsltd.com/ | ~BASIS member; software dev |
| EternaEX | AI solutions, enterprise apps, AWS, SOC 2 | https://eternaex.com/ | ~AI development agency; 200+ clients; AWS Certified Team; SOC 2 Compliant |
| Eoxi | ERP, AI SaaS, LMS, full-stack | https://eoxi.net/ | ~Mirpur; ERP and AI software development; founded 2023 |
| Shaitrish | Full-stack, AI, web/mobile apps | https://shaitrish.com/ | ~Mohammadpur; software dev agency; 8-person team |
| ShahTech Solutions | Custom SW, web design, e-commerce, SEO | https://shahtechsolutions.com/ + info@shahtechsolutions.com | ~Mirpur; govt clients (Ministry of Science); small-mid firm; 4+ years |
| MicroKodes Ltd | Finance, ERP, HRM, CRM, web/mobile apps | https://microkodes.com/ | ~Uttara; founded 2012; govt + private projects; software dev |
| Green Delta Insurance PLC (IT) | React Native, Node.js, TypeScript, Android, iOS | https://dohaj.com/search?q=Green+Delta+Insurance | ~Leading general insurer; AAA rated; hiring Mobile App Dev (React Native + Node); Mohakhali |
| Mercantile Bank PLC (IT Division) | ASP.NET (MVC), Java Spring, Python Django, Oracle | https://chakricircular.com/job/software-developer-it-division/ (Mercantile Bank) | ~Private commercial bank; hiring software developers (IT Division); 3-5yr experience |
| IPDC Finance PLC (IT) | Java, full-stack development, Spring | https://dohaj.com/job-details/full-stack-software-developer-ipdc-finance-plc-778374 | ~Top 20 finance co; hiring Full Stack Developer; Java/Spring; Dhaka |
| Modhumoti Bank PLC (ICT Division) | Java, Spring, Core Banking, security | https://dohaj.com/search?q=Modhumoti+Bank+PLC (ICT Division) | ~Hiring SWE, IT Security, DBA, Network engineers; core banking systems |
| Astha Life Insurance (IT) | ASP.NET, C#, Flutter, HTML, JS, MSSQL | https://dohaj.com/job-details/manager-senior-manager-it-astha-life-insurance-company-limited-416694 | ~Hiring IT Manager + Flutter Dev; in-house ERP development; Mohakhali |
| MBangla Softwares (MBangla Ltd) | ERP, supply chain, cloud, enterprise software | https://mbangla.com/about/ | ~Division of MBangla conglomerate; ERP/cloud infrastructure for industrial sectors |
| Foodpanda Bangladesh | Mobile, web, delivery platform, data | https://foodpanda.com/ + BASIS member | ~Global food delivery platform; BD office as BASIS member; tech roles likely |
| Priyo Ltd (priyo.com) | PHP, web, portal, content platform | https://priyo.com/ + BASIS member | ~Internet portal; BASIS member; largest BD content portal; hiring potential for dev roles |
| Softineers | Full-stack, web/mobile, cloud | https://bdtechjobs.com/companies (Softineers) | ~Listed on BD Tech Jobs; small-mid software firm |
| Gain Solutions | Custom SW, web dev, IT consulting | https://bdtechjobs.com/companies (Gain Solutions) | ~Listed on BD Tech Jobs; software dev & IT services |
| Innova Soft Ltd | Custom apps, web solutions, IT services | https://bdtechjobs.com/companies (Innova Soft Ltd) | ~Listed on BD Tech Jobs; small software co |
| Venturas Ltd | Software dev, IT services | https://bdtechjobs.com/companies (Venturas Ltd) | ~Listed on BD Tech Jobs; technology services |
| FluvoSoft | Java, Spring Boot, Go, gRPC, Kafka, K8s | https://www.fluvosoft.com/ + GitHub (fluvosoft) | ~BD-based; microservices specialist; GitHub org with Spring Boot + Go templates |
| Benchmark Software Bangladesh Ltd | Microfinance MIS, integrated accounting | https://benchmarksoftwarebd.com/ + benchmarkltdbd@gmail.com | ~Middle Badda; microfinance/accounting software specialist; small firm |
| AKIJ ONLINE LIMITED | PHP, Python, Java, Node, MySQL, MongoDB, Redis | https://akijonline.com/ | ~Part of Akij Group; one-stop IT solutions since 1997; hardware, ISP, ERP, custom dev |
| ANDnet Solutions Limited | C#, Java, JS, Kotlin, PHP, Python, Angular, React, Flutter | https://andnetsolutions.com/ | ~10+ emp; web/mobile dev, IT services since ~2005 |
| ANWAR ENTERPRISE SYSTEMS LIMITED | Software, IoT, AI Solutions | https://aes.software/ | ~Part of Anwar Group (~29 in tech division); founded 2021 |
| ARITS Limited | Laravel, MySQL, React, Java, Python, JS | https://aritsltd.com/ | ~15 emp; Dhaka-based software dev since 2015 |
| ARN TECH | PHP, Laravel, React, Magento, Angular, Node, Android/iOS | https://arntechbd.com/ | ~Web/app dev since 2009; eCommerce, ERP, custom software |
| ASL Systems LTD. | Aviation IT, enterprise systems | https://asl.aero/ | ~11-50 emp; specialized aviation IT; 20+ years |
| ATB Lab Ltd. | Flutter, TypeScript, Java, Docker, Laravel, React, K8s, Python | https://atb-lab.jp/ + https://atb-jobs.com | ~11 emp; Japanese-managed offshore dev; has career portal |
| ATC TECH LIMITED | IT Solutions, custom software, system integration | https://atctechltd.com/ | ~Offices in BD, Dubai, USA; 10+ years |
| Aamartech Limited | Cloud, cybersecurity, software dev | https://aamartech.llc/ | ~10 emp; US-Bangladesh JV; 360° IT solutions |
| Aan-Nahl | PHP, CakePHP, Laravel, WordPress, MySQL, jQuery | https://aan-nahl.com/career/ | ~22 emp; custom software & mobile dev; career page |
| Abelling | AI/ML, computer vision, NLP, data labeling | https://abelling.ai/ | ~15-18 emp; serves US & EU clients |
| AccenTech Limited | ASP.NET, C#, AngularJS, PHP/Laravel, Django | https://accentechltd.com/ | ~2 emp; custom software, BPA, mobile apps |
| Accord Technologies Limited | Cloud-native, AI, automation, SaaS | https://accordtechltd.com/ | ~ISO 27001/9001; product: AccordHRM; fintech/edtech/logistics |
| Acote Limited | TensorFlow, Python, React, Angular, Vue, Node, Docker, Unreal | https://acotegroup.com/ | ~66 emp; full-stack AI, software, BPO; Banani office |
| Adplay Technology Limited | ASP.NET Core, Python, MySQL, programmatic ad platform | https://adplaytechnology.com/ | ~26 emp; AdTech DSP; acquired by Azerion (2022) |
| Again Software Solutions | PHP, Laravel, POS, ERP, e-commerce | https://againsoft.com/ | ~8+ years; 150+ clients; products: AgainCart, AgainPOS |
| Agemark Technology | Web apps, POS, ERP, School/Hospital mgmt | https://agemarksoft.com/ | ~Founded 2015; 762+ projects, 455+ clients |
| Agile Bytes | Web, API, AI/ML, 3D design, mobile | https://agile-bytes.com/ | ~Founded 2020; serves govt/public sector |
| Akaar IT Ltd. | Figma, Flutter, React, Firebase, Tailwind | https://akaarit.com/ | ~16 emp; POS/ERP product (AmarSolution); 3000+ clients |
| Al-Hiyal Automation Limited | RPA, Power BI, Power Apps, Azure, .NET | https://alhiyal.com/ | ~20-50 emp; founded 2007; Dhaka + US office |
| Alchemy Software Limited | Web, mobile apps | https://alchemy-bd.com/career | ~24 emp; HQ Chittagong + Dhaka; founded 2010 |
| Alice Labs Pte. Ltd. (Revora) | AI/ML, conversational AI, Node, React, cloud SaaS | https://myalice.ai/career | ~Singapore-incorporated, BD operations; $500k seed from Anchorless Bangladesh |
| Ambala IT | PHP, Laravel, React, Python, ERP, SaaS, mobile apps | https://ambalait.com/ | ~Since 2016; Dhaka + UK + Ghana; products: Naba ERP, MicrofinPlus |
| Amber Software Solutions Limited | .NET, SQL, Desktop/Web ERP, POS | https://ambersoftwaresolutions.com/ | ~Since 2011; Gulshan; products: Retail POS, ISP Billing, Distribution ERP |
| Annanovas IT LTD. | PHP, Laravel, React Native, iOS/Android, AI/ML | https://annanovas.com/career | ~Since 2010; Dhaka; 300+ projects, 100+ clients; offshore dev |
| AnyConnect Bangladesh (Smarter AI) | IoT, C/C++, Computer Vision, WebRTC, Cloud APIs | https://anyconnect.com/careers | ~11-50 (BD office); Singapore HQ; IoT video PaaS |
| Aplectrum Solutions Ltd. | .NET, PHP, Mobile (Android/iOS) | https://aplectrum.com/ | ~11-50 emp; Dhaka; web/mobile apps, HR/payroll ERP |
| AppDevs | Flutter, Fintech, PHP/Laravel, mobile, web | https://appdevs.net/careers | ~11-50 emp; Dhaka + London; fintech SaaS |
| Appnap Technologies | iOS, Android, Web, UI/UX | https://appnap.io/ | ~50-200 emp; consumer mobile apps; 4.8M+ active users |
| AppsCode Ltd. | Go, Kubernetes, KubeDB, KubeVault, Voyager | https://appscode.com/ | ~100+ emp; cloud-native K8s products; enterprise-grade |
| Arbree Limited | Web, custom software, QA, staff augmentation | https://arbreesolutions.com/ | ~11-50 emp; UK (Luton) HQ + Dhaka office; 100+ projects |
| Arogga Limited | PHP/Laravel, React, iOS/Android, e-commerce | https://arogga.com/careers | ~51-200 emp; online pharmacy platform; 3M+ customers |
| Augmedix BD Ltd | AI, NLP, EHR integration, WebRTC, Cloud | https://augmedix.com/careers | ~501-1,000 emp; US healthcare AI company; Dhaka office |
| Auth Lab | WordPress (PHP), React, Vue.js | https://authlab.io/jobs | ~120+ emp; Sylhet; WP plugins (Fluent Forms, FluentCRM, Ninja Tables) |
| Authentic Four Technology | Laravel, React, Python, Flutter, AWS | https://authenticfour.com/ | ~201-500 emp; Chattogram; ERP, mobile apps, hospital mgmt |
| Axilweb Limited | WordPress, Shopify apps, React, PHP, Python, AI | https://axilweb.com/ + https://jobs.axilweb.com/ | ~50-100 emp; Banani; products: Crewlix HRM, FormCRM |
| B-Trac Solutions Ltd | Android, Web, PHP, Python, IoT | https://btracsolutions.com/ | ~Part of Bangla Trac Group; builds Android/web apps |
| BACKDOOR PRIVATE LTD | Cybersecurity (Metasploit, Nessus, SIEM) | https://backdoor.com.bd/ | ~20-50 emp; Dhaka; SOC services, VAPT, compliance |
| Bdtask Limited | PHP (Laravel/CodeIgniter), React, Python/Django, AWS | https://bdtask.com/career.php | ~50-249 emp; 45+ SaaS products; exports to 100+ countries |
| Barikoi Technologies Limited | Python, Node, React, geospatial APIs, AI | https://barikoi.com/ | ~63 emp; hyperlocal maps; $182K seed from IDLC |
| Battery Low Interactive Ltd | Unity, PHP (Laravel), Python (Django/Flask), Angular | https://batterylowinteractive.com/ | ~43 emp; First AR/VR company in BD |
| Beatnik Technology limited | PHP, Laravel, Node, React, Angular, Flutter, AWS | https://beatniktechnology.com/ | ~10-49 emp; 10+ years; BASIS & eCAB member |
| Berger Tech Consulting Limited | SAP, MS Dynamics 365, AWS, Azure, UiPath, Power BI | https://bergertechbd.com/ | ~27 emp; subsidiary of Berger Paints; founded 2022 |
| Beyond Bracket Limited | PHP, Python, MERN, Odoo, Laravel | https://beyondbracket.com/category/career/ | ~14 emp; offshore dev agency; founded 2021 |
| Be Data Solutions Limited | Python, data engineering, Odoo, ML/AI | https://bedatasolutions.com/careers/ | ~UK-led data & AI consultancy; Dhaka hub |
| Big Bang Computer Ltd | Healthcare/ERP, MIS, web dev | https://bigbang.com.bd/ | ~55 emp; since 2000; ISO 9001:2008 |
| Bimafy Ltd | Laravel/PHP, React, iOS/Android | https://bimafy.com/ | ~50-200 emp; insurance marketplace platform |
| BinduLogic Limited | React, Node, microservices, cloud-native, AI/ML | https://bindulogic.com/ | ~50-100 emp; healthcare tech; powers 14+ public health facilities |
| Bizzntek Ltd | .NET, Azure, Dynamics 365, Power BI, SharePoint | https://bizzntek.com/ | ~50-100 emp; Microsoft Gold Partner; UAE/BD/US/AUS |
| Bohubrihi Technologies Ltd (Shikho) | Next.js, React, Node, cloud | https://bohubrihi.com/ | ~100-300 emp; EdTech; VC-backed (Learn Capital, DSG) |
| Brain Station 23 PLC | .NET, Java, PHP, Angular, React, Node, AWS, Azure | https://brainstation-23.com/career | ~850+ emp; CMMI L3, ISO 27001; clients in 30+ countries |
| Brainify Bangladesh | Java, C#, ASP.NET, PHP, React, Node, NEXT | https://brainifybd.com/ | ~11-50 emp; provides dev teams to Norwegian clients |
| Bright River Bangladesh | AI, 3D, AR, Python, ML | https://bright-river.com/ | ~1K-5K global; visual content solutions; BD office |
| Brillmark Technologies BD | Shopify, WordPress, full-stack, DevOps, Cloud | https://brillmark.com.bd/ | ~Small; A/B testing & CRO agency; US parent |
| BugsBD | SIEM, PAM, VAPT, endpoint security | https://bugsbd.com/ | ~51-200 emp; cybersecurity company; founded 2016 |
| Byte Trek Ltd | Web, mobile, AI, cloud, BPO | https://bytetrek.com/ | ~11-50 emp; IT services/BPO; founded 2017 |
| CASHe Alliance Ltd | AI/ML, cloud-native, FinTech | https://cashealliance.com/ | ~JV fintech credit platform |
| CIS Tech Ltd | React, Node, IoT, Cloud, AI | https://cistechltd.com/ | ~50-100 emp; offices in BD, US, Germany, Ghana |
| CMED Health Ltd | AI, IoT, mobile (Android/iOS), cloud | https://cmed.com.bd/ | ~100+ emp; AI-driven digital health platform; APICTA awards |
| COBAIT Bangladesh Ltd | .NET, Azure, cloud infrastructure | https://cobait.com/ | ~50-100 emp; US-based MSP with BD office |
| CURSOR Limited | PHP, JS, React, MySQL, ERP systems | https://cursorbd.com/career | ~30-80 emp; products: Cursor ERP, POS, Hotel/Hospital Mgmt |
| Care-Box Limited | E-commerce platform, mobile app | https://care-box.com/career | ~50-100 emp; online pharmacy with in-house dev team |
| Caretutors Technologies Ltd | React, Node, mobile apps | https://caretutors.com/ | ~50-100 emp; #1 tutoring marketplace in BD |
| Classic IT & Sky Mart Ltd | PHP, School Mgmt, ERP, POS, Pharmacy, E-commerce | https://classicit.com.bd/career | ~Real product-based software; 1500+ clients |
| CliqPack LTD | AI, SaaS, Cloud, Python, React/JS, Laravel | https://cliqpack.com/career/ | ~51-200 emp; HQ Melbourne + Dhaka + Chattogram |
| CodeMarshal IT Systems Ltd | Face Recognition, OCR, KYC, Python/AI | https://codemarshal.com/ | ~Small; real AI/ML product company; FaceMarshal product |
| CodersBucket Ltd | Laravel, Python/Django, Next.js, React Native, Node | https://codersbucket.com/career/ | ~14+ yrs; 180+ projects; SaaS products (Hello HRM) |
| Core3Lab Limited | Java, .NET, Python, Go, PHP, Laravel, Flutter, React, Vue | https://core3lab.com/vacancies/ | ~Dhaka; 100+ tech proficiencies; offshore dev |
| Corexlab Limited | Next.js, Web/Mobile, AI, Blockchain | https://corexlab.com/join-us/ | ~Dhaka + Australia; 50+ specialists |
| CtgShop Software | ASP.NET, Android, iOS, Cloud, FIX Protocol | https://ctgshop.com/ | ~11-50 emp; fintech OMS for stock brokers; Chittagong, founded 2014 |
| Cyber Aeronautycs Ltd | Cybersecurity (Acronis, Sophos, Syteca) | https://cyberaeronautycs.com/ | ~Cybersecurity MSP; Banani, Dhaka |
| DAPCO Ventures | Custom software, SaaS, mobile apps, IT consulting | https://dapcoventures.com/ | ~51-200 emp; CMMI L3, ISO 27001; US + Dhaka office |
| DataFort Limited | RPA, workflow automation, document mgmt | https://datafortbd.com/ | ~50-200+ emp; enterprise digital transformation |
| DataMart BD Limited | Custom software, web/mobile apps, data analysis | https://datamartbd.com/ | ~11-50 emp; custom software dev; founded 2016 |
| Datavanced | AI-augmented software dev (OpenAI/GPT, Claude) | https://datavanced.com/ | ~US-headquartered; BD, India, Turkey dev teams |
| Dana Fintech Ltd | AI/ML credit scoring, eKYC API, digital lending | https://dana.money/ | ~11-50 emp; fintech startup; seed-funded |
| Desh Soft Ltd | .NET, PHP, Java, iOS, Android | https://deshsoft.com/career | ~Offices in BD, Malaysia, Japan, Canada; ERP products |
| DeshiCommerce | No-code e-commerce SaaS platform | https://deshicommerce.com/ | ~Part of Bluebird Interactive; product company |
| DevsStream Limited | Custom software, web/mobile apps, UI/UX | https://devsstream.com/career | ~UK & BD offices |
| DevsZone | Laravel, Python, Django, AI/ML, cloud | https://devszone.com/career | ~40+ emp; 9+ years; 300+ projects |
| Dhrubok Infotech Services | React, Next.js, Vue, Java/Spring, Node, Flutter, AI/ML | https://dhrubokinfotech.com/career | ~350+ projects, 30+ countries; full-stack dev shop |
| Diverzent Ltd | Enterprise software, RPA, BI, automation | https://diverzent.com/career | ~Enterprise SW implementation; career page |
| Doctime Ltd | Telemedicine platform | https://doctime.com.bd/ | ~Health-tech startup |
| Dotpot iT | Next.js, Node, DevOps, AI, mobile/web | https://dotpotit.com/ | ~50+ emp; London & Dhaka offices |
| Dreamerz Lab Ltd | Laravel (PHP), Unity, 3D/XR/VR | https://dreamerzlab.com/career | ~Clients: Activision, Suzuki, BAT, Berger |
| ECB Technologies | Temenos T24, core banking | https://ecbtechnologies.com/ | ~Banking software (Temenos T24); Dhaka office |
| EFOLI | Shopify apps, B2B eCommerce | https://efoli.com/career | ~Award-winning Shopify Partner; 15+ yrs |
| ERP.com.bd | Cloud ERP, web-based modules | https://erp.com.bd/ | ~Real ERP software provider |
| EUPHORIA INFOTECH | AI, IoT, ERP, Data Science, Analytics | https://euphoriainfotech.com/career | ~21 yrs; 100+ clients; India/BD |
| EWN Bangladesh | Web/mobile dev, UI/UX | https://ewnbd.com/career | ~Web/mobile dev agency |
| Echologyx Ltd | Shopify, Magento, WP, React, Node, .NET | https://echologyx.com/career | ~UK-HQ, BD offices; CRO/dev agency |
| Eclipse Intellitech | Python, Django, Node, PHP, Laravel, React, Angular, Flutter | https://eclipseintellitech.com/career | ~Full-service digital agency |
| EcoSoftBD | Stock market analysis software | https://ecosoftbd.com/ | ~Product: Smarter Stock; thousands of users |
| Einstech Studio | SMS, WAP, IVR, software, mobile VAS | https://einstechstudio.com/career | ~Real tech co (VAS/software products) |
| Elitbuzz Technologies | Zoho Suite, Odoo ERP, chatbots, digital marketing | https://elitbuzz.com/ | ~IT consulting; UAE + BD + 6 countries |
| Eurosia Technologies Limited | AI/Data, RPA, software dev, UI/UX, Cloud | https://eurosiatech.com/ | ~Real full-stack tech company |
| Eyevary Limited | System integration, web apps, IoT, AI | https://eyevary.com/ | ~2-10 emp; Dhaka |
| Fair Pattern LTD | AI, Cloud (Azure/AWS), ML, IT staffing | https://fairpattern.com/ | ~51-200 emp; HQ NYC + Dhaka office |
| Feenix Lab | Web/mobile, SEO, digital marketing | https://feenixlab.com/career | ~11-50 emp; NYC & Dhaka offices |
| Finva Soft Limited | React, Next.js, PHP, Laravel, MySQL | https://finvasoft.com/ | ~Health-tech; BASIS member; products: DiaLab, Medisfy |
| Foqas Group | AI, finance, tech subsidiaries | https://foqas.com/ | ~Holding group with AI/tech subs |
| G10 Infotech Limited | Cybersecurity, IaaS, SaaS, Cloud, IT consulting | https://g10infotech.com/ | ~Partners: Cisco, MS, Dell, Fortinet, AWS, VMware |
| GCTL Infosys | C#, .NET, PHP, Laravel, Python, Java, Magento | https://gctlinfosys.com/ | ~BASIS member; Dhaka + Germany offices |
| GFGG IT Solutions | Salesforce ecosystems | https://gfggit.com/career | ~Salesforce consultancy; career page |
| Graaho Ltd | Python, React, Angular, Java, AWS, Azure, AI/ML | https://graaho.com/career/ | ~51-200 emp; AWS Advanced Tier Partner; clients: Dell, US Army |
| GoZayaan Limited | Travel booking platform | https://gozayaan.com/ | ~Travel tech startup |
| Gold Kinen Technologies | Gold savings app, fintech | https://goldkinen.com/career | ~11-50 emp; fintech |
| HABRO SYSTEMS LIMITED | PHP, Laravel, React, Python, Node, ASP.NET, Java, AWS | https://habrosystems.com/ | ~Products: EduMax, eJabeda, BhabanMac; BASIS/BCS member |
| HSENID Mobile Solutions | Enterprise SW, Telecom, HR (PeopleHR), AI Chatbots | https://hsenid.com/ | ~Sri Lanka HQ + BD subsidiary; 40+ countries |
| Harris Web Works (Harris Digital) | B2B eCommerce, NetSuite, Shopify, Magento, AWS | https://harrisdigital.io/ | ~US (CT) + Dhaka office |
| HasTech IT Limited | Odoo ERP, Shopify, WooCommerce, Magento, Webflow | https://hastechit.com/careers/ | ~150+ countries; 10K+ businesses |
| HealthOS Limited | Healthcare infrastructure platform | https://healthosbd.com/ | ~6K+ pharmacies, 64 districts; Series-stage startup |
| Hishabee Technologies | ASP.NET Core (ABP), SaaS ERP | https://hishabee.com/ | ~ERP SaaS: Inventory, Sales, HR, Payroll |
| Hubar Tech Limited | Telecoms software | https://hubartech.com/jobs | ~Sister company of UK Exos Systems Ltd |
| IRINFOSYS LIMITED | AI/ML, IoT, Big Data, Blockchain, Cloud | https://irinfosys.com/career | ~11-50 emp; founded 2024 |
| IT Magnet BD | Java, PHP, C#, SQL, ERP | https://itmagnetbd.com/ | ~CMMI L3, ISO 9001:2008; founded 2001 |
| IT WAY BD | Custom software, ERP, CRM, HRM, POS, mobile | https://itwaybd.com/career | ~51-200 emp; product: Xtreem ERP; since 2018 |
| ITclan BD | Web, mobile, software, DevOps, SEO, QA | https://itclanbd.com/career | ~43+ team; Trustpilot 4.5/5; since 2016 |
| IYLMA Innovation Ltd | Custom software, web, mobile, cloud; products: HMS, ERP, LMS | https://iylma.com/ | ~Real software product company |
| Ideaxen | Software, mobile apps, IoT, ERP; products: Bepari, BaniAdam | https://ideaxen.com/ | ~Real software dev co |
| Idlewild Digital | Python/Django, J2EE, Android, Drupal, CRM | https://idlewildigital.com/career | ~2-10 emp; since 2015 |
| Inovi Solutions | Salesforce (Apex, Lightning) | https://inovisolutions.com/join-us/ | ~Salesforce consulting/dev |
| IBSSBD | Laravel, Vue, Inertia, Tailwind | https://ibssbd.com/ | ~Custom SW dev; server/e-commerce platform |
| IoT Lab BD | PHP, Node, Ruby, .NET, WP, Drupal, Joomla; IoT | https://iotlabbd.com/ | ~Software + IoT dev |
| Iqrasys Solutions | C#, ASP.NET, JS, Laravel, React, Angular, Android/iOS | https://iqrasys.com/career | ~POS, ERP, custom SW |
| Ishraak Solutions | Python, Flutter, OpenCV; AI/ML focus | https://ishraak.com/career/ | ~AI software dev, ERP, chatbot |
| Ind Innovation | Cloud, Data Center, Enterprise Network, ICT Security | https://indinnovation.com/career | ~2000+ emp in 20+ countries; UK-affiliated |
| Inflack Limited | Custom SW, AI/ML, Cloud/DevOps, Mobile Apps | https://inflack.com/ | ~Govt clients (BCC, BARD, BIAM) |
| Inflame Solutions Ltd | Web, SaaS, SW dev, AI Automation, ERP | https://inflamesolutions.com/career | ~BASIS member; multiple ERP products |
| Infosoftbd | Cloud Contact Center, AI Voice, SMS/API, Omni-Channel | https://infosoftbd.com/ | ~CPaaS; banking/retail/healthcare focus |
| Infosonik Systems | Security, Data Center, IoT, Managed Services | https://infosonik.com/ | ~Partners: Cisco, Fortinet, Oracle, NetApp, Huawei |
| Inleads IT | Web, ERP, E-Commerce, digital marketing | https://inleadsit.com/career | ~30+ staff; BASIS member; Malaysia branch |
| Innovative Technology & Engineering | Software dev, digital transformation, AI/ML, Cloud | https://innovativetechbd.com/ | ~Uttara, Dhaka |
| Inovace Technologies | IoT (Tipsoi HRM, SensorTrail IIoT), firmware | https://inovacetech.com/ | ~HQ Singapore; tech office Shahbag, Dhaka |
| i-Mesh Ltd | Custom software (HRMS, VMS, AMS), mobile, web | https://imeshbd.com/ | ~BASIS/ECAB member; since 2006 |
| iHelpBD | CRM, call center software, omnichannel, IVR, AI | https://ihelpbd.com/career/ | ~500+ clients; since ~2019; career page |
| bitBirds Solutions | Web/app dev, hosting, domain reg, IT support | https://bitbirds.com/ | ~BASIS member; since 2012 |
| KITE GAMES STUDIO | iOS/Android native, AI/ML | https://kitegamesstudio.com/career | ~51-200 emp; 18M yearly downloads |
| KloverCloud BD Ltd | Kubernetes, Go, React, CI/CD, DevOps | https://klovercloud.com/ | ~11-50 emp; cloud-native platform company |
| LUMINALOGIK | React, Node, offshore dev, custom software | https://luminalogik.com/ | ~Offshore dev shop; Chattogram + Melbourne |
| Leotech | ERP, eCommerce, Healthcare, POS, Web, Mobile, Data Center | https://leotechbd.com/career | ~Full-stack software house; multiple products |
| Line Reflection Ltd | PHP, MySQL, JS, React, Node, Next, Gatsby, Spring, Docker | https://linereflection.com/career | ~Dhaka + Cupertino; custom SW, DevOps, IoT, QA |
| LuminousLabs | React, Laravel, Node, Flutter, Python, Odoo, AWS | https://luminouslabsbd.com/career | ~Real full-stack/SaaS company |
| DataBind Technology | Web, Mobile, FinTech, Cyber Security, Data Analytics | https://databindtech.com/career | ~IT consulting + FinTech + full-stack dev |
| Hamba Games | Unity 3D | https://hambagames.com/ | ~Mobile game studio; 550M+ downloads |
| Mediusware Ltd | Next.js, C#, C++, JS, PHP, Go, .NET, AWS, Azure, AI | https://mediusware.com/career | ~120+ engineers; Microsoft partner; outstaffing/SaaS |
| Metroonn Limited | Document mgmt, scanning, cyber security | https://metroonn.com/ | ~Products: ArcMate Enterprise suite |
| Microters | Next.js, WordPress plugins, SaaS platforms, AI | https://microters.com/career | ~Software/dev/digital agency; 64+ countries |
| Microxen Technology | Next.js, React, Laravel, Node, fintech SaaS | https://microxen.com/careers | ~Delaware-registered; product: Keeal payment platform |
| MoMagic Bangladesh | DCB, PSMS, app dev, billing infra | https://momagicbd.com/ | ~100M+ transactions; partners: bKash, GP, Robi |
| Musketeers Idea Ltd | ERP suite (Accounting, NGO, HRM, Hospital) | https://musketeersidea.com/ | ~miSoftware ERP suite |
| NXGIT Soft | ASP, PHP, Laravel, Node, Shopify, Magento | https://nxgitsoft.com/ | ~POS, Accounting, Travel, Hospital, School products |
| Nerddevs Ltd | React, Vue, Flutter, Node, Next, MongoDB, Redis, PostgreSQL | https://nerddevs.com/ | ~Since 2015; clients: ACCA, British Council |
| NetCoden | C++, C#, PHP, Vue, Node, Python, Laravel | https://netcoden.com/career | ~Montreal + Dubai + Dhaka; career page (hiring) |
| Neuron33 Ltd | AR, VR, software dev, game dev, DevOps | https://neuron33.com/career | ~Gulshan, Dhaka + US contact |
| Next Solution Lab | React, Vue, Angular, PHP, Python, .NET, Node, AI/ML | https://nextsolutionlab.com/career | ~AI R&D; open roles: Lead AI/ML Eng, Full Stack |
| Notionhive Bangladesh | NextJS, WordPress (headless CMS), web/app dev | https://notionhive.com/career | ~60+ staff; 1600+ projects; 12 yrs |
| Nusratech | AI, cloud, product engineering, MarTech | https://nusratech.com/ | ~Clients: UNICEF, GrameenPhone, Banglalink |
| OS CLiCKS | Django, Flask, Laravel, Yii, Magento, ML/AI, Python | https://osclicks.com/ | ~11-50 emp; Dhaka; est. 2008 |
| Octaglory Limited | Distribution Management SaaS Platform | https://octaglory.com/ | ~SaaS distribution mgmt; AI forecasting, POS |
| OpenRefactory | AppSec/SaaS (iCR, PCB products) | https://openrefactory.com/ | ~US-headquartered; BD entity; security products |
| Orboroi Bangladesh | AI data annotation/model evaluation | https://orboroi.com/ | ~AI/data services company |
| Otix Technologies | Next.js, React, web/mobile, AI/ML, cloud | https://otixtech.com/career | ~Sylhet; 6+ emp; BASIS member |
| PMaspire Technologies | Project management training, exam simulator | https://pmaspire.com/ | ~Singapore-based; Global Knowledge Centre in Dhaka |
| Parallaxlogic Infotech | Custom software, IT consulting | https://parallaxlogic.com/career.html | ~31 emp; Microsoft Gold Partner; ISO certified; founded 2010 |
| Paribahan.com | Transport ticketing platform | https://paribahan.com/ | ~BASIS/e-CAB member; bus/cruise/flight ticketing |
| ParonSoft Solutions | App dev, web dev, e-commerce, mobile apps | https://paronsoft.com/ | ~100+ clients; Dhaka |
| Piistech Limited | ASP.NET MVC, .NET Core, C#, MS SQL, Java, PHP, Python | https://piistech.com/ | ~Founded 2017; Uttara; Clutch award winner; BASIS/e-CAB |
| PixelVega | Web infrastructure, CMS, SaaS, custom apps | https://pixelvega.com/career | ~Houston TX HQ; career page (Sr UX Designer, PM, BD) |
| Pirthe Limited | Software/web/mobile dev, e-commerce | https://pirthe.com/ | ~Govt clients: Land Records Ministry, BEPZA |
| Primacy Infotech | Odoo ERP, PHP, Mobile (Android/iOS), Web | https://primacyinfotech.com/ | ~Odoo Silver Partner; custom ERP |
| Programming Hero | JavaScript, TypeScript, React, Next, Node, MongoDB | https://programming-hero.com/ | ~Edtech; coding bootcamp |
| QA Harbor | QA services, staff augmentation, security testing | https://qaharbor.com/career | ~QA company; career page |
| Qtec Solution | .NET, AI, Angular, AWS, Azure, Django, Docker, Flutter, Java | https://qtecsolution.com/career | ~Staff aug; 100+ tech stack; career page |
| Quantanite Bangladesh | AI/ML (QiQ platform), customer ops, data ops | https://quantanite.com/career | ~Enterprise BPO+AI; 25M+ interactions/yr |
| REBING TECH | AI/ML, custom SW, web/mobile apps, data & analytics | https://rebingtech.com/ | ~15 yrs; products: SaleSync, QuickSum, FarmFlow |
| Ridmik Labs | Android (Ridmik Keyboard) | https://ridmiklabs.com/ | ~11-50 emp; Dhaka; 10M+ downloads |
| Ringer Soft | ERP, POS, School Mgmt, E-Commerce | https://ringersoft.com/ | ~11-50 emp; Chittagong; founded 2015 |
| RoBenDevs | WordPress, Node, React, Data | https://robendevs.com/careers/ | ~11-50 emp; Banani; founded 2022; hiring Sr. DevOps, Sr. Full-stack |
| Raindrops Tech Ltd | Custom software, web, e-commerce, cybersecurity | https://raindropstech.com/ | ~Dhanmondi; MD Nishat Mushfiqua |
| STARTISE LIMITED | WordPress product (WPDeveloper, Storeware, Templately) | https://startise.com/career/ | ~6M+ users; 45+ plugins; parent of WPDeveloper |
| STATA IT Limited | IoT, mobile apps, web dev, ERP, e-commerce | https://statait.com/career | ~Smart home automation + software dev |
| Skylark Soft Limited | ERP for textile/garment (goRMG, PROTRACKER, AQAI, HRKIT) | https://skylarksoft.com/careers | ~CMMI L3, ISO 27001/9001; 100+ clients; 12 countries; hiring |
| Softzino Technologies | React/Next.js, Node, Odoo, SaaS (BARNOi, Hishabi) | https://softzino.com/join-us/career | ~Odoo partner; own SaaS products; actively hiring |
| Solutya Private Limited | React/Next.js, Node, NestJS, Express, Azure, AWS | https://solutya.com/career | ~16 open positions; ThemeForest seller; ERP |
| Soppiya Innovation Limited | React/Next.js, multi-tenant SaaS | https://soppiya.com/career | ~Product: EcommerceOS (Shopify competitor) |
| Squad Innovators | React, Next.js, TS, Tailwind, Laravel, PHP, MySQL | https://squadinnovators.com/ | ~50+ projects; ISO 9001; e-commerce focus |
| Soft IT Security | POS, School Mgmt, HR/Payroll, Hospital Mgmt | https://softitsecurity.com/career | ~PHP, web apps, Android; career page |
| SoftCare IT | IT consulting, web, mobile, game dev, ERP, POS, HRM | https://softcareit.com/career | ~BASIS/e-CAB; 569 projects; since 2017 |
| Softify Technologies | C# .NET, ASP.NET MVC, SQL Server, PHP/MySQL | https://softifytech.com/career | ~Products: Sales & Inventory, Accounting, HRM, POS, ERP |
| Softograph Ltd | AI, deep analytics, products: Inspecto, ICE, Proggya | https://softograph.com/career | ~AI/ML product company; Oxford University case studies |
| Softopark IT Ltd | Python, MERN, Webflow, WP, Shopify, Django, React Native | https://softopark.com/career | ~15 team; 389+ websites; 1210+ clients; since 2015 |
| Sys Dev Ltd | WordPress, Oracle DB, Java, HTML/CSS/JS | https://sysdevltd.com/careers/ | ~Web, mobile, e-commerce; career page (Frontend Dev) |
| Syscomatic Technologies | WordPress, PERN, MERN, AI/ML, IoT | https://syscomatic.com/ | ~Offices: USA, Dubai, Dhaka |
| Suffix IT Limited | React, HCM/HR/Payroll, ERP, E-commerce, FFMS | https://suffixit.com/ | ~Real dev co |
| StaticMania | Next.js, Hugo, Astro, headless CMS | https://staticmania.com/ | ~Static site specialists |
| The ICT Hub | Next.js, custom software, web/mobile apps, AI, ERP | https://theicthub.com/career | ~Global clients; real software company |
| The Tork Incorporation | React, Vue, Angular, Go, Laravel, Python, Node, AI/ML | https://thetork.com/career | ~Full-stack dev; UK+BD offices |
| Tirzok Private Limited | DevOps, Cloud, ERP, software dev, IT consultancy | https://tirzok.com/ | ~ISO certified; clients: M&S, Optasia |
| Truck Lagbe Limited | Mobile apps, logistics platform | https://trucklagbe.com/career/ | ~$4M Series A; funded startup; active career page |
| Traideas | React, Next.js, Node, Python, Flutter, Shopify, AI/ML | https://traideas.com/careers | ~Active hiring (BE dev, SWE intern) |
| Trends Bird Limited | WordPress, software/web/mobile dev | https://trendsbird.com/career/ | ~Digital agency; active openings |
| Trillion Bits Ltd | React, RN, Angular, Vue, Python, Node, Laravel, .NET | https://trillionbits.com/ | ~US/BD presence; broad tech stack |
| Velwire Ltd | Real-time payment, financial infrastructure | https://velwire.com/careers | ~BD fintech; partners: Microsoft, BCG; Singapore office |
| Webb Fontaine | AI/ML, Customs & Trade platforms | https://webbfontaine.com/careers | ~Global co; AI-powered trade facilitation |
| WINBRIDGETECH LTD | PHP (CodeIgniter), Web/App/BPO/UI-UX/QA | https://winbridgetech.com/career-view | ~BASIS member; Dhaka + NY offices |
| WPDeveloper | WordPress/PHP, SaaS (Essential Addons, NotificationX) | https://wpdeveloper.com/jobs | ~100+ team; 6M+ users; Startise group |
| WPXPO | WordPress/WooCommerce plugins (PostX, WowStore) | https://wpxpo.com/career | ~30+ team; 65K+ users; 9+ products; founded 2020 |
| Wafi Solutions | .NET Core, ABP.IO, Python, Django, AWS/Azure, AI | https://wafisolutions.com/career | ~12+ yrs; 150+ projects; Mohakhali DOHS; career page |
| XUBISOFT LTD | Software dev, web, mobile, ERP, e-Health, Edu Mgmt | https://xubisoft.com/career | ~Uttara; full-stack; career page |
| XpeedStudio | PHP, Elementor, React (Gutenberg), AI (GetGenie) | https://xpeedstudio.com/career | ~WP plugin/theme shop; hiring |
| XpertLab BD Ltd | ASP.NET Core, Blazor, MVC, Web API, Node, Android/iOS | https://xpertlabbd.com/ | ~Custom enterprise software |
| YetFix Limited | Web, Mobile, AI SaaS, UI/UX | https://yetfix.com/ | ~50+ startups; 110+ projects |
| ZCORP Solutions | Full-stack, cloud, DevOps, IT training | https://zcorpsolutions.com/ | ~Enterprise IT; 7 countries |
| Zaag Systems Ltd | AI, Next.js/react, custom commerce, embedded teams | https://zaagsys.com/ | ~AI Product Engineering Lab |
| Zantrik Limited | Mobile app + web, car maintenance platform | https://zantrik.com/ | ~150K+ customers; 2000+ partner garages |
| Zaynax Limited | Web, App, Cloud, DevOps | https://zaynax.com/ | ~Parent of Zaynax Health |
| i-Mesh Ltd | PHP/WordPress, custom software (HRMS, VMS, AMS) | https://imeshbd.com/ | ~BASIS/ECAB member; since 2006; custom dev |
| iHelpBD | React/Angular, CRM, call center, omnichannel, IVR, AI | https://ihelpbd.com/career/ | ~500+ clients; BPO/software; since 2019 |
| bitBirds Solutions | Web/app dev, hosting, IT support, custom software | https://bitbirds.com/ | ~BASIS member; since 2012 |
 
## Bulk BASIS & BD Company Reference (unresearched)
> All 111 SAAS directory pages fully extracted and all ~1,920 entries individually researched via website access.
> Companies below remain in bulk as they were found to be non-software, WordPress-only, dead/unreachable, or unverifiable.
> ~220 real software dev companies from this list have been researched and added to the main table above (an entry may appear in both places).
> 
> **Research breakdown of 1,920 bulk entries:**
> | Category | Count | Description |
> |---|---|---|
> | Moved to main table (real SW dev co) | ~220 | Has career pages, tech stacks, employees >5 |
> | WordPress-only / CMS shop | ~100-150 | Only does WP/CMS, not custom software dev |
> | Non-IT business | ~250-350 | Retail, construction, training, media, logistics, etc. |
> | Freelancer / individual consultant | ~50-70 | Single-person operations, Upwork-style |
> | Dead / unreachable / parked / expired | ~1,100-1,300 | Domain dead, timeout, parked for sale, DNS error |
> 
> **Total BD companies tracked in this file: ~2,500+** (500 researched + 2,000+ bulk reference)
| Company Name | Source | Notes |
|---|---|---|
| BizMotion Limited | BASIS SAAS | Field Force Automation |
| Rokkhi IT Solutions Limited | BASIS SAAS | Rokkhi Home product |
| Unisource Technology | BASIS SAAS | Billing Master ERP/POS |
| Swosti Limited | BASIS SAAS | CoopBank247, MFI software |
| RITE Solutions Limited | BASIS SAAS | ritebooks |
| Mazedatech Ltd. | BASIS SAAS | MTechERP |
| KICHAI IT SERVICES LTD | BASIS SAAS | HisabPotro, ERP2ALL |
| TOGETHER INITIATIVES (Pvt) LIMITED | BASIS SAAS | e-BPM, xSale, eRPA |
| TMSS ICT LIMITED | BASIS SAAS | Comprehensive Accounts |
| Intelligent Business Solutions Limited | BASIS SAAS | Biometric Attendance |
| ZUNOKS Consulting | BASIS SAAS | Gamified Recruitment |
| e-World Ltd. | BASIS SAAS | Hisab Khata |
| NITS Service (Pvt) Ltd | BASIS SAAS | NTRACK |
| Prime Tech Solutions Ltd. | BASIS SAAS | Trincome |
| Mediasoft Data Systems Ltd. | BASIS SAAS | Smart Sense |
| Computer Ease Limited | BASIS SAAS | Distributor & Sales Force Mgmt |
| Netsoft Solution Ltd. | BASIS SAAS | NSS ERP |
| shurjoMukhi Limited | BASIS SAAS | shurjoPay Payment Gateway |
| Anupam Infotek Limited | BASIS SAAS | IT solutions |
| Comjagat Technologies Limited | BASIS SAAS | Tech solutions |
| Macro Softwares Limited | BASIS SAAS | Software products |
| Softway IT | BASIS SAAS | IT services |
| RTC Hubs Limited | BASIS SAAS | Tech services |
| Impel Service & Solutions Limited | BASIS SAAS | IT services |
| Wintel Limited | BASIS SAAS | IT/Tech |
| Green and Red Technologies Limited | BASIS SAAS | Payment tech |
| NNS Solution Ltd. | BASIS SAAS | IT solutions |
| Beyond Innovations & Technologies Limited | BASIS SAAS | Innovation/tech |
| Radisson Digital Technologies Limited | BASIS SAAS | Digital solutions |
| WEBTECHSOFT.COM | BASIS SAAS | Web/software |
| Solution 9 Ltd. | BASIS SAAS | Software solutions |
| Confidence Software Limited | BASIS SAAS | Software products |
| Mango Teleservices Limited | BASIS SAAS | Telecom services |
| M2M Communications Ltd. | BASIS SAAS | Telecom/communication |
| Opus Technology Limited | BASIS SAAS | Technology solutions |
| My Outsourcing Ltd. | BASIS SAAS | IT outsourcing |
| MIEC Lab Ltd. | BASIS SAAS | Lab/tech services |
| XOR Geek | BASIS SAAS | Tech solutions |
| KS Network Limited | BASIS SAAS | Networking |
| UQEEL.COM Limited | BASIS SAAS | E-commerce platform |
| Race IT Solution BD | BASIS SAAS | IT solutions |
| Anymotion Studio | BASIS SAAS | Animation/design |
| Thrilltons | BASIS SAAS | Tech/entertainment |
| Quant FinTech Ltd. | BASIS SAAS | Fintech |
| Service Hub Limited | BASIS SAAS | Service platform |
| Teamexus Solutions Ltd. | BASIS SAAS | Collaboration/tech |
| Easital Technologies Ltd. | BASIS SAAS | Tech solutions |
| Winky Tech Limited | BASIS SAAS | Tech solutions |
| Sarker Trade International Limited | BASIS SAAS | Trade/IT |
| Cambrian Technologies Limited | BASIS SAAS | Tech solutions |
| Renaissance Technology BD | BASIS SAAS | Tech solutions |
| Vcube Soft and Tech Limited | BASIS SAAS | Software/tech |
| TaxHouse Bangladesh Limited | BASIS SAAS | Tax software |
| Tech Analytica Limited | BASIS SAAS | Analytics/tech |
| Tech Point BPO | BASIS SAAS | BPO services |
| Wizard Software & Technology Bangladesh Ltd. | BASIS SAAS | Software/tech |
| Touch & Solve Technologies Limited | BASIS SAAS | Tech solutions |
| Softifybd Limited | BASIS SAAS | Software |
| THE IPAGE GLOBAL LTD. | BASIS SAAS | Web/IT services |
| TELEAUS Bangladesh Ltd | BASIS SAAS | Telecom |
| REDQ TECHNOLOGIES LTD. | BASIS SAAS | Tech solutions |
| Leadcraft IT Solutions | BASIS SAAS | IT solutions |
| Eon infosys Technology | BASIS SAAS | IT services |
| Gamma Innovation Ltd. | BASIS SAAS | Innovation/tech |
| CTrends Software & Services Ltd. | BASIS PDF Catalog | Software & services |
| ACME AI LTD | BASIS PDF Catalog | AI solutions |
| Beetles Cyber Security Ltd | BASIS PDF Catalog | Cyber security |
| Right Time Limited | BASIS PDF Catalog | IT services |
| Nitto Digital Service and Analytics Ltd. | BASIS PDF Catalog | Digital/analytics |
| Reverie Corporation Limited | BASIS PDF Catalog | IT services |
| Desktop IT | BASIS PDF Catalog | IT services |
| Infosoft Valley Ltd | BASIS PDF Catalog | Software/dev |
| E-Medical Solution Limited | BASIS PDF Catalog | Hospital mgmt SW |
| Excellence ICT | BASIS PDF Catalog | Hospital mgmt SW |
| MerinaSoft | BASIS PDF Catalog | Hospital mgmt SW |
| Pro-edge Associates Limited | BASIS PDF Catalog | HR software |
| ReCom Consulting Ltd. | BASIS PDF Catalog | HR/consulting |
| Sweet iTech Tech & Business Solutions Ltd | BASIS PDF Catalog | HR/software |
| Amar Bebsha Limited | BASIS PDF Catalog | ERP/business |
| Business Automation Ltd. | BASIS PDF Catalog | ERP/automation |
| DOT BD SOLUTIONS | BASIS PDF Catalog | ERP solutions |
| PC Link IT Palli Ltd. | BASIS PDF Catalog | IT/palli services |
| Proficient Information Systems | BASIS PDF Catalog | ERP/software |
| Square InformatiX Limited | BASIS PDF Catalog | ERP/software |
| CoLoCity Limited | BASIS PDF Catalog | Data center/cloud |
| OBHAI Solutions Ltd. | BASIS PDF Catalog | IT enabled services |
| Grameen Communications | BASIS PDF Catalog | MFI/banking SW |
| Solution Art Ltd. | BASIS PDF Catalog | IT solutions |
| Debug BD | BASIS PDF Catalog | Mobile apps/games |
| Infobahn Realm IT Solution | BASIS PDF Catalog | GIS/tech |
| Link Vision Software Solution Ltd | BASIS SAAS | HRIS, Elearning Portal |
| Databiz Software Limited | GitHub list | Software company |
| 10MS Limited | BASIS SAAS | |
| 22 Info Tech | BASIS SAAS | |
| 24/7 Virtual Assistants | BASIS SAAS | |
| 35mm studio | BASIS SAAS | |
| 3R ENTERPRISE | BASIS SAAS | |
| 4 Sight Technology Limited | BASIS SAAS | |
| 4Beats Ltd. | BASIS SAAS | |
| 4K Engineering | BASIS SAAS | |
| 4S Technologies Limited | BASIS SAAS | |
| 6amTech | BASIS SAAS | |
| 7Digital Ton Ltd. | BASIS SAAS | |
| 88 Innovations | BASIS SAAS | |
| 88 Innovations Engineering Ltd. | BASIS SAAS | |
| A & A Consulting Limited | BASIS SAAS | |
| A. K. Khan Telecom Limited | BASIS SAAS | |
| A.Wahab & Co. | BASIS SAAS | |
| A2ARENA ltd | BASIS SAAS | |
| AA Technology Limited | BASIS SAAS | |
| ABG Datafication Limited | BASIS SAAS | |
| ABG TECHNOLOGIES LIMITED | BASIS SAAS | |
| ABIR IT LIMITED | BASIS SAAS | |
| ACCFINTAX | BASIS SAAS | |
| ADA Trading Bangladesh Co.Ltd | BASIS SAAS | |
| ADN DIGINET LIMITED | BASIS SAAS | |
| ADN Eduservices Limited | BASIS SAAS | |
| ADN Media Limited | BASIS SAAS | |
| ADON COMMUNICATIONS LIMITED | BASIS SAAS | |
| AGAMI Limited | BASIS SAAS | |
| AGS Quality Action Limited | BASIS SAAS | |
| AHSAN TECHNOLOGIES LTD | BASIS SAAS | |
| AI PROJUKTI LIMITED | BASIS SAAS | |
| AIIM Global Limited | BASIS SAAS | |
| AKIJ ONLINE LIMITED | BASIS SAAS | |
| ALLIED INFORMATION TECHNOLOGY LIMITED | BASIS SAAS | |
| ALPHA POTATO LTD. | BASIS SAAS | |
| ALTRUIST TECHNOLOGIES LIMITED | BASIS SAAS | |
| AMAR AGRO-TECH LTD | BASIS SAAS | |
| ANAM Research & Development Solutions | BASIS SAAS | |
| AND IT | BASIS SAAS | |
| ANDnet Solutions Limited | BASIS SAAS | |
| ANS MUSIC OPC | BASIS SAAS | |
| ANWAR ENTERPRISE SYSTEMS LIMITED | BASIS SAAS | |
| APPAREL ONLINE | BASIS SAAS | |
| ARA TECHNOLOGIES LTD. | BASIS SAAS | |
| ARHAM Techpro Ltd | BASIS SAAS | |
| ARITS Limited | BASIS SAAS | |
| ARMR TECH | BASIS SAAS | |
| ARN TECH | BASIS SAAS | |
| AROSH FREELANCER | BASIS SAAS | |
| ARRA Technologies Limited | BASIS SAAS | |
| ASK Telecom Limited | BASIS SAAS | |
| ASL Systems LTD. | BASIS SAAS | |
| AST International Limited | BASIS SAAS | |
| ATB Lab Ltd. | BASIS SAAS | |
| ATC TECH LIMITED | BASIS SAAS | |
| ATTRITO LIMITED | BASIS SAAS | |
| AUSPICIOUS | BASIS SAAS | |
| AVENTRACONSULTANT LTD. | BASIS SAAS | |
| AZIFA ICT LIMITED | BASIS SAAS | |
| AZTech Systemz Limited | BASIS SAAS | |
| Aalpin Digital | BASIS SAAS | |
| Aamar Digital Solutions Ltd. | BASIS SAAS | |
| Aamartech Limited | BASIS SAAS | |
| Aan-Nahl | BASIS SAAS | |
| Abelling | BASIS SAAS | |
| Academy of Business Professionals (ABP) | BASIS SAAS | |
| AccenTech Limited | BASIS SAAS | |
| Accord Tech Solutions | BASIS SAAS | |
| Accord Technologies Limited | BASIS SAAS | |
| Acote Limited | BASIS SAAS | |
| ActiveXT Limited | BASIS SAAS | |
| Adbox Bangladesh | BASIS SAAS | |
| Adeffi Limited | BASIS SAAS | |
| Adplay Technology Limited | BASIS SAAS | |
| AdroitSSD | BASIS SAAS | |
| Advanced Equipment Limited | BASIS SAAS | |
| Advanced IT | BASIS SAAS | |
| Advancing Business Professionals Limited (ABPL) | BASIS SAAS | |
| Adventure Dhaka Limited | BASIS SAAS | |
| Advert Limited | BASIS SAAS | |
| Aesthetic Eurasia | BASIS SAAS | |
| Aftab Nagar Online Service (ANOS) | BASIS SAAS | |
| Again Software Solutions | BASIS SAAS | |
| Agemark Technology | BASIS SAAS | |
| Agile Bytes | BASIS SAAS | |
| Agriventure Limited | BASIS SAAS | |
| AinoviQ IT LTD. | BASIS SAAS | |
| Aipro Engineering & Consultancy Service | BASIS SAAS | |
| Airways Office | BASIS SAAS | |
| Akaar IT Ltd. | BASIS SAAS | |
| Al-Hiyal Automation Limited | BASIS SAAS | |
| Alchemy Software Limited | BASIS SAAS | |
| Algo Bit Technology Ltd. | BASIS SAAS | |
| Algorithm Generation Ltd | BASIS SAAS | |
| Alice Labs Pte. Ltd. | BASIS SAAS | |
| Alien Technology Ltd. | BASIS SAAS | |
| All Next Ver | BASIS SAAS | |
| Allone Softtech Limited | BASIS SAAS | |
| Alo Communications Ltd | BASIS SAAS | |
| Alo It Consultants | BASIS SAAS | |
| Alpha Commerz LTD. | BASIS SAAS | |
| Alpha-i Studios Ltd. | BASIS SAAS | |
| Alphabyte Technology Ltd. | BASIS SAAS | |
| AlterYouth Limited | BASIS SAAS | |
| Amader Academy Ltd | BASIS SAAS | |
| AmarStock Limited | BASIS SAAS | |
| Amarlab Limited | BASIS SAAS | |
| Amazing Soft | BASIS SAAS | |
| Ambala IT | BASIS SAAS | |
| Amber Software Solutions Limited | BASIS SAAS | |
| Ami Probashi Limited | BASIS SAAS | |
| Amreen Info Tech Limited | BASIS SAAS | |
| AnZa Corporation Ltd. | BASIS SAAS | |
| Anandasoftbd | BASIS SAAS | |
| Anchorblock Technology Limited | BASIS SAAS | |
| Angular Esports Ltd | BASIS SAAS | |
| Anirban Soft | BASIS SAAS | |
| Annanovas IT LTD. | BASIS SAAS | |
| Antaranga Dot Com Ltd. | BASIS SAAS | |
| Anupam Recording Media | BASIS SAAS | |
| AnyConnect Bangladesh Limited | BASIS SAAS | |
| Aplectrum Solutions Ltd. | BASIS SAAS | |
| AponTech Ltd | BASIS SAAS | |
| AppDevs | BASIS SAAS | |
| Appinion BD Limited | BASIS SAAS | |
| Apple soft IT | BASIS SAAS | |
| Application Mentors Limited | BASIS SAAS | |
| Applied Business Initiatives Ltd | BASIS SAAS | |
| Appnap Technologies Limited | BASIS SAAS | |
| AppsCode Ltd. | BASIS SAAS | |
| Aqualink Bangladesh Limited | BASIS SAAS | |
| Araf Tech Point Ltd. | BASIS SAAS | |
| Arafin Media | BASIS SAAS | |
| Arbree Limited | BASIS SAAS | |
| Arcturus Technology | BASIS SAAS | |
| Arena Excellence Limited | BASIS SAAS | |
| AriSaf Tech | BASIS SAAS | |
| Arknetics Ltd. | BASIS SAAS | |
| Armor Bangladesh Limited | BASIS SAAS | |
| Arogga Limited | BASIS SAAS | |
| ArrowLink Soft | BASIS SAAS | |
| Arthor Limited | BASIS SAAS | |
| Artificial Soft | BASIS SAAS | |
| Artology | BASIS SAAS | |
| Ascend Technology Ltd. | BASIS SAAS | |
| Asian Technologies Limited | BASIS SAAS | |
| Asiatic Marketing Communications Ltd | BASIS SAAS | |
| Aspire Tech Services and Solutions Limited | BASIS SAAS | |
| Asterisk Digital OPC | BASIS SAAS | |
| Atova Technology | BASIS SAAS | |
| Attrabit ICT Solution | BASIS SAAS | |
| Augmedix BD Ltd. | BASIS SAAS | |
| Aurko Technologies Ltd. | BASIS SAAS | |
| Aus-Bangla Communications Ltd. | BASIS SAAS | |
| Auth Lab | BASIS SAAS | |
| Authentic Four Technology | BASIS SAAS | |
| Automation Services Ltd. | BASIS SAAS | |
| Automation Solutionz Bangladesh | BASIS SAAS | |
| Autonemo Limited | BASIS SAAS | |
| Avalon Hosting Services Ltd. | BASIS SAAS | |
| Avant Technological Solution | BASIS SAAS | |
| Avian BPO & IT | BASIS SAAS | |
| Avid Tech Solutions Ltd. | BASIS SAAS | |
| Avro Digital Enterprise | BASIS SAAS | |
| AxEnTec PLC | BASIS SAAS | |
| Axilweb Limited | BASIS SAAS | |
| Ayaan Tech Limited | BASIS SAAS | |
| Ayesha Outsourcing Solutions Ltd. | BASIS SAAS | |
| AyyKori Digital Limited | BASIS SAAS | |
| Azmi Studio | BASIS SAAS | |
| Azoka Limited | BASIS SAAS | |
| Azoncode Ltd. | BASIS SAAS | |
| B Technologies | BASIS SAAS | |
| B-Trac Solutions Ltd. | BASIS SAAS | |
| B-Trac Technologies Limited | BASIS SAAS | |
| BAARTA TECHNOLOGIES LIMITED | BASIS SAAS | |
| BACKDOOR PRIVATE LTD. | BASIS SAAS | |
| BAKTIER AHMED RONY AND ASSOCIATES LIMITED | BASIS SAAS | |
| BANGLA TRAC LIMITED | BASIS SAAS | |
| BANGLADESH SOFTWARE SOLUTION | BASIS SAAS | |
| BANGLAMARK Fintech Ltd. | BASIS SAAS | |
| BARASIA International | BASIS SAAS | |
| BCI Technosys Limited | BASIS SAAS | |
| BD Fare Bangladesh Limited | BASIS SAAS | |
| BD Software & Security System Ltd. | BASIS SAAS | |
| BD Tax Technology Ltd. | BASIS SAAS | |
| BDCRICTEAM.COM | BASIS SAAS | |
| BDECOM IT LTD. | BASIS SAAS | |
| BDGAME STUDIO LTD | BASIS SAAS | |
| BDIT | BASIS SAAS | |
| BEATNIK DIGITAL LIMITED | BASIS SAAS | |
| BGD Online Limited | BASIS SAAS | |
| BIGM Resources Limited | BASIS SAAS | |
| BIKE BD | BASIS SAAS | |
| BINARYCLOTH Ltd | BASIS SAAS | |
| BINDU IT LIMITED | BASIS SAAS | |
| BIPO Service (Bangladesh) Limited | BASIS SAAS | |
| BITS AND BYTES | BASIS SAAS | |
| BITxx Technologies Ltd. | BASIS SAAS | |
| BLUWEBZ | BASIS SAAS | |
| BMIT Solutions Ltd. | BASIS SAAS | |
| BMS TECH LOGISTICS LTD. | BASIS SAAS | |
| BONGO TECHNOLOGY LTD. | BASIS SAAS | |
| BRIGHT-i SYSTEMS LTD. | BASIS SAAS | |
| BTE Infotech Pvt. Ltd. | BASIS SAAS | |
| BULLBD DOT COM | BASIS SAAS | |
| BZM Graphics Limited | BASIS SAAS | |
| Backspace International Limited | BASIS SAAS | |
| Bangla Insider Limited | BASIS SAAS | |
| Bangla Puzzle Limited | BASIS SAAS | |
| Bangladesh Associate of IT Solution | BASIS SAAS | |
| Bangladesh Consulting Limited | BASIS SAAS | |
| Bangladesh IT Institute | BASIS SAAS | |
| Bangladesh RACE Management Private Co. Ltd. | BASIS SAAS | |
| Bangladesh SME Corporation Ltd. | BASIS SAAS | |
| Bangladevs Technologies | BASIS SAAS | |
| Bangladhol Limited | BASIS SAAS | |
| Barikoi Technologies Limited | BASIS SAAS | |
| Basumati IT Solutions Ltd. | BASIS SAAS | |
| Battery Low Interactive Ltd. | BASIS SAAS | |
| Bay Information Technologies and Systems Ltd. | BASIS SAAS | |
| Bdtask Limited | BASIS SAAS | |
| Be Data Solutions Limited | BASIS SAAS | |
| Beatnik Technology Limited | BASIS SAAS | |
| Bee Technology & Research Hub | BASIS SAAS | |
| Benet Tech | BASIS SAAS | |
| Bengal Creative Media Ltd. | BASIS SAAS | |
| Bengal Software Limited | BASIS SAAS | |
| Bepresent IT Limited | BASIS SAAS | |
| Berger Tech Consulting Limited | BASIS SAAS | |
| Best Bazar BD | BASIS SAAS | |
| Betafore | BASIS SAAS | |
| BetonBook Pvt. Ltd. | BASIS SAAS | |
| Beyond Bracket Limited | BASIS SAAS | |
| Bhalo Ventures Limited | BASIS SAAS | |
| Big Bang Computer Limited | BASIS SAAS | |
| Bijoy Informatics Ltd. | BASIS SAAS | |
| Bijoy wifi Private Limited | BASIS SAAS | |
| Bikolpo Computer | BASIS SAAS | |
| Billing Master Software Ltd. | BASIS SAAS | |
| Bimafy Ltd. | BASIS SAAS | |
| Binate Solutions Ltd. | BASIS SAAS | |
| Bindulogic Limited | BASIS SAAS | |
| Bit Byte Technology Limited | BASIS SAAS | |
| Bit Code Technologies Limited | BASIS SAAS | |
| Bite Hive Solutions Limited | BASIS SAAS | |
| Bitec Software | BASIS SAAS | |
| Bitlab Technology Solutions Ltd. | BASIS SAAS | |
| Bitmorpher | BASIS SAAS | |
| Bitspearhead Limited | BASIS SAAS | |
| Bitsy Technologies Limited | BASIS SAAS | |
| BizMappers Ltd. | BASIS SAAS | |
| Bizz Solutions PLC. | BASIS SAAS | |
| Bizzntek Ltd | BASIS SAAS | |
| BlocKnots Limited | BASIS SAAS | |
| Blue Automation | BASIS SAAS | |
| Blue Pill Limited | BASIS SAAS | |
| Blue Solutions Limited | BASIS SAAS | |
| Bluebees Limited | BASIS SAAS | |
| Bluedot Technology Ltd | BASIS SAAS | |
| Bohubrihi Technologies Ltd. | BASIS SAAS | |
| Boibazar.com | BASIS SAAS | |
| Bongo IT Limited | BASIS SAAS | |
| Bongtech Limited | BASIS SAAS | |
| Borak services limited | BASIS SAAS | |
| Bot-tola Cyber Net | BASIS SAAS | |
| Brain Craft Ltd. | BASIS SAAS | |
| Brain Wave IT Solution | BASIS SAAS | |
| Brainify Bangladesh | BASIS SAAS | |
| Braintree | BASIS SAAS | |
| BrainyZat Digital Limited | BASIS SAAS | |
| Bright River Bangladesh limited | BASIS SAAS | |
| Bright Solutions | BASIS SAAS | |
| Brillmark Technologies Bangladesh Private Limited | BASIS SAAS | |
| British Bangla Travel Limited | BASIS SAAS | |
| Bug Finder | BASIS SAAS | |
| Bug Resistance | BASIS SAAS | |
| BugsBD Limited | BASIS SAAS | |
| Buildcon Consultancies Limited | BASIS SAAS | |
| Bullet Platforms Limited | BASIS SAAS | |
| Business Information Technology Limited | BASIS SAAS | |
| Business Network | BASIS SAAS | |
| Business Novelty Ltd. | BASIS SAAS | |
| Business Software Solutions Limited | BASIS SAAS | |
| Business Solution | BASIS SAAS | |
| Buyonia Bangladesh Limited | BASIS SAAS | |
| Buzzuuka Communications | BASIS SAAS | |
| Byte Care Limited | BASIS SAAS | |
| Byte Trek Limited | BASIS SAAS | |
| ByteCode Limited | BASIS SAAS | |
| C 3 Sourcing | BASIS SAAS | |
| CAD One Limited | BASIS SAAS | |
| CADD CORE TRAINING & IT SERVICES | BASIS SAAS | |
| CASHe Alliance Limited | BASIS SAAS | |
| CD Choice | BASIS SAAS | |
| CDIP IT SERVICES LTD | BASIS SAAS | |
| CHAYA APP LIMITED | BASIS SAAS | |
| CIMPEX International | BASIS SAAS | |
| CIPHER ANALYTICA LIMITED | BASIS SAAS | |
| CIS Tech Ltd. | BASIS SAAS | |
| CLAP Services Ltd. | BASIS SAAS | |
| CLAREx Limited | BASIS SAAS | |
| CLICK ART BD LIMITED | BASIS SAAS | |
| CM Work Solutions | BASIS SAAS | |
| CMED Health Limited | BASIS SAAS | |
| COBAIT Bangladesh Limited | BASIS SAAS | |
| COLORS OF BANGLADESH | BASIS SAAS | |
| COORDINATES | BASIS SAAS | |
| COUNTRY'S LARGEST AUDIENCE NETWORK LIMITED | BASIS SAAS | |
| COdesign | BASIS SAAS | |
| CSL Training | BASIS SAAS | |
| CSM BANGLADESH LTD | BASIS SAAS | |
| CTMT Solutions | BASIS SAAS | |
| CURSOR LIMITED | BASIS SAAS | |
| CUTTING EDGER | BASIS SAAS | |
| Camel Waves Digital | BASIS SAAS | |
| Care-Box Limited | BASIS SAAS | |
| Caretutors Technologies Limited | BASIS SAAS | |
| Carnival Assure Limited | BASIS SAAS | |
| Carrot Comm Limited | BASIS SAAS | |
| Catch Bangladesh Limited | BASIS SAAS | |
| Celebration | BASIS SAAS | |
| Celestial Tech Limited | BASIS SAAS | |
| Central Music and Video (CMV) | BASIS SAAS | |
| Centranix Limited | BASIS SAAS | |
| Centureon IT | BASIS SAAS | |
| Challen Beel Communication | BASIS SAAS | |
| Chhaya Technologies Limited | BASIS SAAS | |
| Cholpori Technologies Ltd. | BASIS SAAS | |
| Circle Data Processing & Research Center | BASIS SAAS | |
| Circle FinTech Ltd. | BASIS SAAS | |
| City IT Limited | BASIS SAAS | |
| Classic IT & Sky Mart Ltd. | BASIS SAAS | |
| Clavis Fintech Solutions | BASIS SAAS | |
| Clear Edge Technologies Limited | BASIS SAAS | |
| Clementine Data Solutions Ltd. | BASIS SAAS | |
| CliqPack LTD | BASIS SAAS | |
| Cloud 7 Limited | BASIS SAAS | |
| Cloud Coder Limited | BASIS SAAS | |
| Cloud Connect Limited | BASIS SAAS | |
| Cloud Experts Ltd. | BASIS SAAS | |
| Cloud Institute | BASIS SAAS | |
| Cloud Japan International (BD) Ltd. | BASIS SAAS | |
| CloudNinja Technologies | BASIS SAAS | |
| CloudWell Digital Services Limited | BASIS SAAS | |
| Cloudbina web services | BASIS SAAS | |
| Cloudware Systems | BASIS SAAS | |
| Cloudy Camp Limited | BASIS SAAS | |
| Cluster International Limited | BASIS SAAS | |
| Co-Solution Ltd | BASIS SAAS | |
| Code For Host Inc Ltd. | BASIS SAAS | |
| Code Spiders Limited | BASIS SAAS | |
| CodeMarshal IT Systems Ltd. | BASIS SAAS | |
| CodeRex | BASIS SAAS | |
| CodeSmith Tech Ltd. | BASIS SAAS | |
| Codeboxr | BASIS SAAS | |
| CodemanBD | BASIS SAAS | |
| Coder71 Limited | BASIS SAAS | |
| CodersBucket Ltd. | BASIS SAAS | |
| CodersTrust Bangladesh Ltd. | BASIS SAAS | |
| Codes Break Ltd. | BASIS SAAS | |
| Codeshaper Corporation | BASIS SAAS | |
| Codeware Limited | BASIS SAAS | |
| Codexplorer Technologies | BASIS SAAS | |
| Coloasia Limited | BASIS SAAS | |
| Color Clipping Limited | BASIS SAAS | |
| Comet IT & Communication Ltd. | BASIS SAAS | |
| Commjuncture | BASIS SAAS | |
| Communication Systems Limited | BASIS SAAS | |
| Comptech Cloud Solutions Ltd. | BASIS SAAS | |
| Computing and Information Services Ltd. | BASIS SAAS | |
| Connect Bangla Limited | BASIS SAAS | |
| Content Matters Ltd. | BASIS SAAS | |
| ContentPro Interactive Limited | BASIS SAAS | |
| Continental Technologies (BD) Ltd | BASIS SAAS | |
| Convergence Technologies Ltd | BASIS SAAS | |
| Coppanet Limited | BASIS SAAS | |
| Core Devs ltd | BASIS SAAS | |
| Core3Lab Limited | BASIS SAAS | |
| Corexlab Limited | BASIS SAAS | |
| Corporate Projukti Limited | BASIS SAAS | |
| Cosmopolitan Communications Ltd. | BASIS SAAS | |
| CrackTech Limited | BASIS SAAS | |
| Craftsmen Ltd. | BASIS SAAS | |
| Crashedeal Limited | BASIS SAAS | |
| Creative Clipping Path Ltd. | BASIS SAAS | |
| Creative Digital Store | BASIS SAAS | |
| Creative IT Soft | BASIS SAAS | |
| Creative Soft Technology Ltd. | BASIS SAAS | |
| Creative Tech Park | BASIS SAAS | |
| Creativitix Software Ltd. | BASIS SAAS | |
| Creato Design research lab ltd. | BASIS SAAS | |
| Creatrix Soft Tech Ltd. | BASIS SAAS | |
| Crosswalk Communications Ltd. | BASIS SAAS | |
| Crown CompTech | BASIS SAAS | |
| Crypto Tech | BASIS SAAS | |
| Crystal Vision Solutions | BASIS SAAS | |
| CtgShop.com Limited | BASIS SAAS | |
| Cubic Global Limited | BASIS SAAS | |
| Cultive8 Technologies Limited | BASIS SAAS | |
| Cyber 32 | BASIS SAAS | |
| Cyber Aeronautycs Ltd. | BASIS SAAS | |
| Cyber World IT | BASIS SAAS | |
| Cyberdyne Technology Ltd | BASIS SAAS | |
| Cybergate Limited | BASIS SAAS | |
| Cye Retail Tech Ltd. | BASIS SAAS | |
| D Global V Limited | BASIS SAAS | |
| D Money Bangladesh Limited | BASIS SAAS | |
| DAINIK SARABANGLA | BASIS SAAS | |
| DAPCO Ventures Limited | BASIS SAAS | |
| DARCO Technologies Limited | BASIS SAAS | |
| DATA INSIGHT SOLUTIONS | BASIS SAAS | |
| DATAWARE LIMITED | BASIS SAAS | |
| DBL Digital Ltd | BASIS SAAS | |
| DCiCON Limited | BASIS SAAS | |
| DESHLINK LIMITED | BASIS SAAS | |
| DHANSHIRI DIGITAL LTD | BASIS SAAS | |
| DIGI JADOO BROADBAND LIMITED | BASIS SAAS | |
| DIGITECH COMPUTERS | BASIS SAAS | |
| DISB Solution (Pvt.) Ltd. | BASIS SAAS | |
| DIST TTC | BASIS SAAS | |
| DIVO Solutions Limited | BASIS SAAS | |
| DOPPCALL | BASIS SAAS | |
| DTCL-Fututre Tech | BASIS SAAS | |
| Daisen Technologies Limited | BASIS SAAS | |
| Dakatiya | BASIS SAAS | |
| Dana Fintech Ltd. | BASIS SAAS | |
| Daraz Bangladesh Limited | BASIS SAAS | |
| Data Aid BD | BASIS SAAS | |
| Data Exchange | BASIS SAAS | |
| DataCrunch Limited | BASIS SAAS | |
| DataFort Limited | BASIS SAAS | |
| DataHub Asia DC First Limited | BASIS SAAS | |
| DataMart BD Limited | BASIS SAAS | |
| DataQuest Tech Limited | BASIS SAAS | |
| DataSoft Next International Ltd. | BASIS SAAS | |
| Datacanvas Solutions Limited | BASIS SAAS | |
| Datacom Solution Limited | BASIS SAAS | |
| Datafluent Analytics | BASIS SAAS | |
| Datascape IT Limited | BASIS SAAS | |
| Datasoft Manufacturing & Assembly Inc. Ltd. | BASIS SAAS | |
| Datasource Software Ltd | BASIS SAAS | |
| Datavanced Bangladesh | BASIS SAAS | |
| Dataworks Ltd | BASIS SAAS | |
| Dcrowd IT Ltd. | BASIS SAAS | |
| Ddesk IT Limited | BASIS SAAS | |
| De Tempete Limited | BASIS SAAS | |
| Debug BD Ltd. | BASIS SAAS | |
| Decent Act International | BASIS SAAS | |
| Decodes Lab Limited | BASIS SAAS | |
| Decor Interior Ltd. | BASIS SAAS | |
| Deft Technologies Limited | BASIS SAAS | |
| Deftyled | BASIS SAAS | |
| Dekko ISHO Technologies Limited | BASIS SAAS | |
| Department S Consulting | BASIS SAAS | |
| Desh Cyber Limited | BASIS SAAS | |
| Desh Soft Ltd. | BASIS SAAS | |
| Deshi Systems Ltd. | BASIS SAAS | |
| DeshiCommerce | BASIS SAAS | |
| Deshifarmer Limited | BASIS SAAS | |
| Devs Core | BASIS SAAS | |
| DevsCred | BASIS SAAS | |
| DevsNest OPC | BASIS SAAS | |
| DevsStream Limited | BASIS SAAS | |
| DevsZone | BASIS SAAS | |
| Dewan ICT | BASIS SAAS | |
| Deys Tech Solution | BASIS SAAS | |
| Dgency | BASIS SAAS | |
| Dhaka Distributions | BASIS SAAS | |
| Dhaka Host IT | BASIS SAAS | |
| Dhaka Stock Exchange Ltd. | BASIS SAAS | |
| Dhaka Web Host Ltd. | BASIS SAAS | |
| DhakaColo Pvt. Limited | BASIS SAAS | |
| Dhakatech iT Ltd | BASIS SAAS | |
| Dhorola Soft Future Technologies Ltd. | BASIS SAAS | |
| Dhorony Limited | BASIS SAAS | |
| Dhrubo Networks Limited | BASIS SAAS | |
| Dhrubok Infotech Services Ltd. | BASIS SAAS | |
| Dial 2 Support | BASIS SAAS | |
| Diana Host Ltd. | BASIS SAAS | |
| Digerati | BASIS SAAS | |
| DigiFea | BASIS SAAS | |
| DigiPro Solutions Limited | BASIS SAAS | |
| Digicon Technologies PLC | BASIS SAAS | |
| Digicon Telecommunication Ltd | BASIS SAAS | |
| Digidot Ltd. | BASIS SAAS | |
| Digital Bridge Limited | BASIS SAAS | |
| Digital Expressions Ltd. | BASIS SAAS | |
| Digital Graphic Studio | BASIS SAAS | |
| Digital Lab | BASIS SAAS | |
| Digital Payments Limited | BASIS SAAS | |
| Digital Run Limited | BASIS SAAS | |
| Digital Security Solutions | BASIS SAAS | |
| Digital Technology Solution Limited | BASIS SAAS | |
| Dikkha Online Limited | BASIS SAAS | |
| Dingi Technologies Ltd. | BASIS SAAS | |
| Dipon Consultancy Services | BASIS SAAS | |
| Discovery Internet | BASIS SAAS | |
| Discovery One Limited | BASIS SAAS | |
| Disrupt Technologies Limited | BASIS SAAS | |
| Divergent Technologies Limited | BASIS SAAS | |
| Diverzent Ltd. | BASIS SAAS | |
| Divine Force Solutions Ltd. | BASIS SAAS | |
| Dnet | BASIS SAAS | |
| Doctime Limited | BASIS SAAS | |
| Doel e-Services | BASIS SAAS | |
| Dolphin IT Solutions | BASIS SAAS | |
| Doodle Incorporation | BASIS SAAS | |
| Dot Birth Limited | BASIS SAAS | |
| Dot Com Systems Ltd. | BASIS SAAS | |
| Dotlines Bangladesh Limited | BASIS SAAS | |
| Dotpot iT | BASIS SAAS | |
| Dream Line IT Solution | BASIS SAAS | |
| Dream Tec | BASIS SAAS | |
| DreamLight Digital Ltd. | BASIS SAAS | |
| DreamOnline Limited | BASIS SAAS | |
| Dreamerz Lab Ltd. | BASIS SAAS | |
| Drobal InnovaTech Corporation | BASIS SAAS | |
| Druto Fintech limited | BASIS SAAS | |
| Dtech Online Limited | BASIS SAAS | |
| Dun & Bradstreet Data & Analytics Private Limited | BASIS SAAS | |
| Dupno International Limited | BASIS SAAS | |
| Durbar Technologies Ltd. | BASIS SAAS | |
| Durbin Labs Limited | BASIS SAAS | |
| Durjoy Rides Limited | BASIS SAAS | |
| E Soft Limited | BASIS SAAS | |
| E-Desk Limited | BASIS SAAS | |
| E-Learning and Earning Limited | BASIS SAAS | |
| E-Medical Software Limited | BASIS SAAS | |
| E-Medical Solution Ltd. | BASIS SAAS | |
| E-Palli Limited | BASIS SAAS | |
| ECB Technologies | BASIS SAAS | |
| EFG Tech | BASIS SAAS | |
| EFOLI | BASIS SAAS | |
| EGO Digital Ltd. | BASIS SAAS | |
| ELEKTRONIX IT TECH SOLUTIONS | BASIS SAAS | |
| ELEVATE Solutions Limited | BASIS SAAS | |
| EMERALD TECHNO LIMITED | BASIS SAAS | |
| ENGINEERING MATRIX | BASIS SAAS | |
| ERECTORS | BASIS SAAS | |
| ERP.com.bd | BASIS SAAS | |
| ET Tech Limited | BASIS SAAS | |
| EUPHORIA INFOTECH BANGLADESH PRIVATE LIMITED | BASIS SAAS | |
| EWN Bangladesh Limited | BASIS SAAS | |
| EXOTICO SOLUTIONS | BASIS SAAS | |
| EYE ELECTRONICS | BASIS SAAS | |
| EagleX Robotics | BASIS SAAS | |
| Earth Telecommunication Pvt. Ltd. | BASIS SAAS | |
| Easytrax World | BASIS SAAS | |
| EchoaSoft Limited | BASIS SAAS | |
| Echologyx Ltd | BASIS SAAS | |
| Eclat IT | BASIS SAAS | |
| Eclipse Enterprise Limited | BASIS SAAS | |
| Eclipse Intellitech Limited | BASIS SAAS | |
| Eco-Dev Solutions & Technologies Bangladesh Limited | BASIS SAAS | |
| EcoSoftBD IT Ltd. | BASIS SAAS | |
| Ecom Solutions | BASIS SAAS | |
| Econ Consulting | BASIS SAAS | |
| Edumaker | BASIS SAAS | |
| Edusoft Consultants Ltd | BASIS SAAS | |
| Effervescent | BASIS SAAS | |
| Efficient Software Solutions Ltd. | BASIS SAAS | |
| Einstech Studio | BASIS SAAS | |
| Eitekh ERP Limited | BASIS SAAS | |
| Ejogajog Limited | BASIS SAAS | |
| EkkBaz Bangladesh Pvt. Ltd. | BASIS SAAS | |
| Electra IT | BASIS SAAS | |
| Electro Soft | BASIS SAAS | |
| Elegance IT Bangladesh | BASIS SAAS | |
| Elegant IT Limited | BASIS SAAS | |
| Elitbuzz Technologies Ltd. | BASIS SAAS | |
| Emerald IT | BASIS SAAS | |
| Emerging Technologies | BASIS SAAS | |
| EnTech Solutions BD | BASIS SAAS | |
| Enamel BD | BASIS SAAS | |
| Encoders Infotech Ltd. | BASIS SAAS | |
| Enigma Multimedia Limited | BASIS SAAS | |
| Enkaizen | BASIS SAAS | |
| Enlight Solutions | BASIS SAAS | |
| Enosis Solutions | BASIS SAAS | |
| Enterprise Info Solutions Ltd. | BASIS SAAS | |
| Equal & Co. Consulting Limited | BASIS SAAS | |
| Ered Technologies Limited | BASIS SAAS | |
| Esquire Technology Limited | BASIS SAAS | |
| Essential Infotech | BASIS SAAS | |
| Ether Technologies Limited | BASIS SAAS | |
| European IT Solutions Bangladesh | BASIS SAAS | |
| Eurosia Limited | BASIS SAAS | |
| Eurosia Technologies Limited | BASIS SAAS | |
| Eutech Systems Ltd. | BASIS SAAS | |
| Excel IT AI LTD. | BASIS SAAS | |
| Excel Intelligent Solutions Ltd. | BASIS SAAS | |
| Excel Technologies Limited | BASIS SAAS | |
| Exes Tech Ltd. | BASIS SAAS | |
| ExonHost | BASIS SAAS | |
| Expert Consortium Ltd | BASIS SAAS | |
| Expo Technologies Ltd. | BASIS SAAS | |
| Expotech Solutions Ltd | BASIS SAAS | |
| Exprocoder IT | BASIS SAAS | |
| Extent Technologies Limited | BASIS SAAS | |
| EyHost Ltd. | BASIS SAAS | |
| Eye Information Communication Technology Limited | BASIS SAAS | |
| Eyevary Limited | BASIS SAAS | |
| F-Z Technologies Limited | BASIS SAAS | |
| F. A. Creative Firm Limited | BASIS SAAS | |
| FABRIC LAGBE LIMITED | BASIS SAAS | |
| FAQ Private Limited | BASIS SAAS | |
| FDS Bangladesh Limited | BASIS SAAS | |
| FEBD Ltd | BASIS SAAS | |
| FIFOTech | BASIS SAAS | |
| FLEX InfoTech Limited | BASIS SAAS | |
| FLUX IT | BASIS SAAS | |
| FLYinfoSoft Technologies Limited | BASIS SAAS | |
| FORT INTERNATIONAL LTD. | BASIS SAAS | |
| FOXPRO LTD | BASIS SAAS | |
| FUTURE TECH | BASIS SAAS | |
| Fair IT Solutions Ltd. | BASIS SAAS | |
| Fair Pattern LTD | BASIS SAAS | |
| Fakir Technologies Limited | BASIS SAAS | |
| Falcons | BASIS SAAS | |
| Famous Creation (Pvt.) Ltd. | BASIS SAAS | |
| Far-East IT Solutions Limited | BASIS SAAS | |
| Fara IT Fusion Ltd. | BASIS SAAS | |
| Fast Clipping Path | BASIS SAAS | |
| Feather IT Limited | BASIS SAAS | |
| Feenix Lab | BASIS SAAS | |
| Fiber Flow Technologies BD Ltd. | BASIS SAAS | |
| FinCoach Bangladesh Limited | BASIS SAAS | |
| FinTale Ltd. | BASIS SAAS | |
| Finest Web Geek | BASIS SAAS | |
| Fingerprint Information Technology Limited | BASIS SAAS | |
| Fingertips Innovations Limited | BASIS SAAS | |
| Finva Soft Limited | BASIS SAAS | |
| Firewall Technologies Limited | BASIS SAAS | |
| First Technology | BASIS SAAS | |
| FirstTrip Limited | BASIS SAAS | |
| Flame Alpha Enterprise | BASIS SAAS | |
| Fleet Bangladesh | BASIS SAAS | |
| Fly Far International | BASIS SAAS | |
| Foqas | BASIS SAAS | |
| Foresight IT | BASIS SAAS | |
| Fort Media | BASIS SAAS | |
| Foxcatcher IT Solutions | BASIS SAAS | |
| Fred Intelligence Ltd. | BASIS SAAS | |
| Free Lancer Information Technology | BASIS SAAS | |
| Free Pixel Games Ltd. | BASIS SAAS | |
| Freedom Soft | BASIS SAAS | |
| Freelancers HUB | BASIS SAAS | |
| FronTech Limited | BASIS SAAS | |
| Furnitex Limited | BASIS SAAS | |
| Fusion Technology | BASIS SAAS | |
| Future Cloud Bangladesh Limited | BASIS SAAS | |
| G Technologies | BASIS SAAS | |
| G10 Infotech Limited | BASIS SAAS | |
| GAZI COMMUNICATIONS | BASIS SAAS | |
| GB Technology | BASIS SAAS | |
| GBL FINTECH LIMITED | BASIS SAAS | |
| GCTL Infosys | BASIS SAAS | |
| GD Assist Limited | BASIS SAAS | |
| GFGG IT Solutions Limited | BASIS SAAS | |
| GHURI EXPRESS LTD. | BASIS SAAS | |
| GIGA TECH5 | BASIS SAAS | |
| GLASCUTR LIMITED | BASIS SAAS | |
| GLOCAL TECHNOLOGY LIMITED | BASIS SAAS | |
| GM TECHNOLOGY | BASIS SAAS | |
| GMGI Solutions Limited | BASIS SAAS | |
| GPOSTING | BASIS SAAS | |
| GROWTH TECHNOLOGY LIMITED | BASIS SAAS | |
| Gain Solutions Ltd | BASIS SAAS | |
| Galaxy Motion | BASIS SAAS | |
| Game On | BASIS SAAS | |
| Geek Picker Limited | BASIS SAAS | |
| GenNext Technologies Limited | BASIS SAAS | |
| Generic Software | BASIS SAAS | |
| Genese Solutions Ltd. | BASIS SAAS | |
| Genex Infrastructure Limited | BASIS SAAS | |
| Genie InfoTech | BASIS SAAS | |
| Geo-Planning for Advanced Development Ltd | BASIS SAAS | |
| Get-Aid Ltd. | BASIS SAAS | |
| Gifty Platform Limited | BASIS SAAS | |
| Giga Tech Ltd. | BASIS SAAS | |
| Gigalogy Ltd | BASIS SAAS | |
| Gingham Services Ltd | BASIS SAAS | |
| Global Brand Pvt. Ltd. | BASIS SAAS | |
| Global IT & Language Institute Ltd. | BASIS SAAS | |
| Global Info-Tech Systems Ltd. | BASIS SAAS | |
| Global Informatics Limited | BASIS SAAS | |
| Global Skills Development Agency | BASIS SAAS | |
| Global Soft Tech | BASIS SAAS | |
| GlobalTech Information Systems | BASIS SAAS | |
| Glocal Learning Management  Limited | BASIS SAAS | |
| Gloria Tech Limited | BASIS SAAS | |
| Glossy IT | BASIS SAAS | |
| GoBangla Solutions | BASIS SAAS | |
| GoZayaan Limited | BASIS SAAS | |
| Goinnovior Limited | BASIS SAAS | |
| Gold Kinen Technologies Limited | BASIS SAAS | |
| Golden Info Systems Limited | BASIS SAAS | |
| Golden Trade International BD. | BASIS SAAS | |
| GoodHope Insure Ltd. | BASIS SAAS | |
| Gpit (global professional IT) | BASIS SAAS | |
| Graaho Ltd. | BASIS SAAS | |
| Grameen Telecom Trust- Digital Healthcare Solutions | BASIS SAAS | |
| Grant Thornton Consulting Bangladesh Limited | BASIS SAAS | |
| Graphics Home | BASIS SAAS | |
| Graphics View | BASIS SAAS | |
| Green Agrotech Grocery Pvt. Ltd. | BASIS SAAS | |
| Green Data Limited | BASIS SAAS | |
| Green Feather Technologies Ltd. | BASIS SAAS | |
| Green Leaf Technology | BASIS SAAS | |
| Grey Meta Solutions | BASIS SAAS | |
| Grit Technologies Limited | BASIS SAAS | |
| Grow More Gaze | BASIS SAAS | |
| Growing Rank | BASIS SAAS | |
| Guardvision Monitoring BD Ltd | BASIS SAAS | |
| Gulshan IT and Infrastructure Limited | BASIS SAAS | |
| HABRO SYSTEMS LIMITED | BASIS SAAS | |
| HAJ Corporation | BASIS SAAS | |
| HAMKO ICT LTD. | BASIS SAAS | |
| HATIL IT | BASIS SAAS | |
| HOSPITALITY AND RETAIL SOLUTIONS (BD) LTD. | BASIS SAAS | |
| HR Bangladesh Limited | BASIS SAAS | |
| HR Reco | BASIS SAAS | |
| HS Traders | BASIS SAAS | |
| HSD Dream71 Ltd. | BASIS SAAS | |
| HSENID MOBILE SOLUTIONS BANGLADESH PVT LTD | BASIS SAAS | |
| HUAWEI TECHNOLOGIES (BANGLADESH) LTD. | BASIS SAAS | |
| HUMAYRA | BASIS SAAS | |
| Happihub Platform Ltd. | BASIS SAAS | |
| Harris Web Works Dhaka Limited | BASIS SAAS | |
| HasTech IT Limited | BASIS SAAS | |
| Hasan IT | BASIS SAAS | |
| Hasan Khan IT Limited | BASIS SAAS | |
| HawarIT Data Services Ltd. | BASIS SAAS | |
| Hawk Eye Digital Limited | BASIS SAAS | |
| HawkEyes Digital Monitoring Limited | BASIS SAAS | |
| Hayati Soft Corporation | BASIS SAAS | |
| Headless Technologies Limited | BASIS SAAS | |
| Headroom InfoTech Limited | BASIS SAAS | |
| HealthOS Limited | BASIS SAAS | |
| Helinix Limited | BASIS SAAS | |
| Hello World Communications Ltd. | BASIS SAAS | |
| Hellotask Platform Ltd | BASIS SAAS | |
| Helper Platform Limited | BASIS SAAS | |
| Hesper IT Solution | BASIS SAAS | |
| Hishab Technologies Ltd | BASIS SAAS | |
| Hishabee Technologies Limited | BASIS SAAS | |
| Hoichoi Technologies Bangladesh Limited | BASIS SAAS | |
| Honest Traders Ltd. | BASIS SAAS | |
| Honeycom IT & Automation Pvt. Ltd. | BASIS SAAS | |
| Hoolo Technologies Limited | BASIS SAAS | |
| Hope IT Solutions | BASIS SAAS | |
| HostsCheap Limited | BASIS SAAS | |
| Hubar Tech Limited | BASIS SAAS | |
| Human Development Research Centre | BASIS SAAS | |
| Hydrus Digital BD (Pvt) Ltd. | BASIS SAAS | |
| Hype Technology Ltd | BASIS SAAS | |
| Hyper Helios | BASIS SAAS | |
| Hyper Systems Ltd. | BASIS SAAS | |
| Hyperlapse BD Ltd. | BASIS SAAS | |
| I-CLIQUE SOLUTIONS LIMITED | BASIS SAAS | |
| I-Infomedia Limited | BASIS SAAS | |
| I-Soft Communication Ltd. | BASIS SAAS | |
| I-Venture Limited | BASIS SAAS | |
| I360 Bangladesh Ltd. | BASIS SAAS | |
| IAK Global Consulting | BASIS SAAS | |
| IBR Software Services and Solutions | BASIS SAAS | |
| IFAD Information & Technology Limited | BASIS SAAS | |
| IGNITE TECHNOLOGY | BASIS SAAS | |
| IGROOTT LIMITED | BASIS SAAS | |
| IMBD Agency Ltd | BASIS SAAS | |
| IMPIT LIMITED | BASIS SAAS | |
| IN-Technology Ltd. | BASIS SAAS | |
| INFONET ASSOCIATES | BASIS SAAS | |
| INFORMAX TECHNOLOGY LIMITED | BASIS SAAS | |
| INFOSYSTEM DEVELOPMENT LTD | BASIS SAAS | |
| INTELLEX LIMITED | BASIS SAAS | |
| INTELLIGENT ERP LTD. | BASIS SAAS | |
| INovex Idea Solution Limited | BASIS SAAS | |
| IONIC Corporation | BASIS SAAS | |
| IOTA INFOTECH LIMITED | BASIS SAAS | |
| IQRA TECHNOLOGIES LTD | BASIS SAAS | |
| IRINFOSYS LIMITED | BASIS SAAS | |
| IT Bangla Limited | BASIS SAAS | |
| IT Craft Ltd. | BASIS SAAS | |
| IT EXPERT BD | BASIS SAAS | |
| IT MEDIA LTD. | BASIS SAAS | |
| IT Magnet | BASIS SAAS | |
| IT Nut Hosting | BASIS SAAS | |
| IT Q Solutions | BASIS SAAS | |
| IT SHEBA 24 DOT COM | BASIS SAAS | |
| IT WAY BD | BASIS SAAS | |
| IT'S Global Bangla Ltd. | BASIS SAAS | |
| ITLogiko | BASIS SAAS | |
| ITX Limited | BASIS SAAS | |
| ITclan BD | BASIS SAAS | |
| ITengine Software Limited. | BASIS SAAS | |
| ITmedicus Solutions | BASIS SAAS | |
| IYLMA Innovation Ltd. | BASIS SAAS | |
| Icicle Corporation | BASIS SAAS | |
| Icon Information Systems Ltd. | BASIS SAAS | |
| Idea Tec Ltd. | BASIS SAAS | |
| IdeaScale Bangladesh | BASIS SAAS | |
| IdeaScale Bangladesh Limited | BASIS SAAS | |
| Ideal Clipping | BASIS SAAS | |
| Ideaxen | BASIS SAAS | |
| Idlewild Digital | BASIS SAAS | |
| Image Retouching Lab | BASIS SAAS | |
| Impact Runway Bangladesh Limited | BASIS SAAS | |
| Impressive Security Ltd. | BASIS SAAS | |
| InResource International Ltd. | BASIS SAAS | |
| Increments Inc. | BASIS SAAS | |
| IncubeX IT Ltd. | BASIS SAAS | |
| Ind Innovation Pvt. Limited | BASIS SAAS | |
| Indrojal | BASIS SAAS | |
| Inferno Technologies Pvt Ltd | BASIS SAAS | |
| Infinity infotech Ltd | BASIS SAAS | |
| Inflack Limited | BASIS SAAS | |
| Inflame Cloud | BASIS SAAS | |
| Inflame Solutions Ltd | BASIS SAAS | |
| Info Bangla Limited | BASIS SAAS | |
| Info Station (Pvt) Limited | BASIS SAAS | |
| Infolady Social Enterprise Limited | BASIS SAAS | |
| Information Technology Solutions and Services | BASIS SAAS | |
| Infosoftbd Solutions | BASIS SAAS | |
| Infosonik Systems Limited | BASIS SAAS | |
| Infosystem Technology Limited | BASIS SAAS | |
| Infosystems Eng Ltd. | BASIS SAAS | |
| Infozillion Teletech BD Limited | BASIS SAAS | |
| Ingenuiti Technologies BD Limited | BASIS SAAS | |
| Inkam Limited | BASIS SAAS | |
| Inland Networks | BASIS SAAS | |
| Inleads IT | BASIS SAAS | |
| Inneed Cloud BD Pvt. Ltd. | BASIS SAAS | |
| InnoWeb Limited | BASIS SAAS | |
| Innova Soft Ltd | BASIS SAAS | |
| Innovation Garage Limited | BASIS SAAS | |
| Innovative Minds Consulting Ltd. | BASIS SAAS | |
| Innovative Online Limited | BASIS SAAS | |
| Innovative Technology & Engineering | BASIS SAAS | |
| InnoverTech Ltd. | BASIS SAAS | |
| Innoversal | BASIS SAAS | |
| Inovace Technologies Limited | BASIS SAAS | |
| Inovi Solutions Ltd. | BASIS SAAS | |
| Insights Automata | BASIS SAAS | |
| Inspira Advisory & Consulting Ltd. | BASIS SAAS | |
| Instalogic | BASIS SAAS | |
| Instantwebb | BASIS SAAS | |
| Instasure Limited | BASIS SAAS | |
| Instructory | BASIS SAAS | |
| Intech Limited | BASIS SAAS | |
| Integrated Business Systems & Solutions pvt Ltd. | BASIS SAAS | |
| Integrated Software and Technologies Ltd. | BASIS SAAS | |
| IntelEdge Corporation | BASIS SAAS | |
| Intellier Ltd. | BASIS SAAS | |
| Intelligent Business Solutions Ltd. | BASIS SAAS | |
| Intelligent Machines Limited | BASIS SAAS | |
| Intelligent Resources International Ltd. | BASIS SAAS | |
| Intelligent Systems & Solutions Ltd | BASIS SAAS | |
| Intercloud Limited | BASIS SAAS | |
| Interface Solutions Limited | BASIS SAAS | |
| Intimacy Computer & Solutions | BASIS SAAS | |
| Intuisys Ltd | BASIS SAAS | |
| Inument Solutions Limited | BASIS SAAS | |
| Invento Software Limited | BASIS SAAS | |
| Invert Emo Tech | BASIS SAAS | |
| Invicta Solutions Ltd. | BASIS SAAS | |
| Invictus Global IT Solutions | BASIS SAAS | |
| IoT Lab BD Ltd. | BASIS SAAS | |
| Ipsita Computers Pte Ltd | BASIS SAAS | |
| Iqrasys Solutions Limited | BASIS SAAS | |
| Isharify Limited | BASIS SAAS | |
| Ishraak Solutions Limited | BASIS SAAS | |
| Itech Soft Solutions | BASIS SAAS | |
| JA Station | BASIS SAAS | |
| JAAN IT BD | BASIS SAAS | |
| JABA IT Ltd. | BASIS SAAS | |
| JADROO IT (BD) Limited | BASIS SAAS | |
| JATRA.COM LTD. | BASIS SAAS | |
| JB CODERS LTD. | BASIS SAAS | |
| JMC Technology Ltd. | BASIS SAAS | |
| JMJ CODE | BASIS SAAS | |
| JOBGHOR24.COM LTD. | BASIS SAAS | |
| JR Recycling Solutions Ltd | BASIS SAAS | |
| Jachai.com Ltd. | BASIS SAAS | |
| Jackal IT | BASIS SAAS | |
| JadeWits Technologies Limited | BASIS SAAS | |
| Jagori Technologies Ltd. | BASIS SAAS | |
| Jahaji Ltd | BASIS SAAS | |
| Jaka International Ltd. | BASIS SAAS | |
| Jamuna Tech | BASIS SAAS | |
| Janata Wifi Ltd. | BASIS SAAS | |
| Jarvis Digital Limited | BASIS SAAS | |
| Jatra International Pvt. Limited | BASIS SAAS | |
| Jatri Services Ltd | BASIS SAAS | |
| Jeeon Bangladesh Ltd. | BASIS SAAS | |
| Jets Next | BASIS SAAS | |
| Jibika Intelligic Ltd. | BASIS SAAS | |
| Jibontory Technology Limited | BASIS SAAS | |
| Jielian Technologies Ltd. | BASIS SAAS | |
| Joha IT | BASIS SAAS | |
| JoomShaper | BASIS SAAS | |
| JoulesLabs | BASIS SAAS | |
| JustGo Technologies Limited | BASIS SAAS | |
| KAR COMMUNICATIONS | BASIS SAAS | |
| KATAHIRA & ENGINEERS INTERNATIONAL | BASIS SAAS | |
| KHAN IT | BASIS SAAS | |
| KITE GAMES STUDIO LTD. | BASIS SAAS | |
| KMR ENTERPRISE BD | BASIS SAAS | |
| KMS SOFTWARE SOLUTIONS | BASIS SAAS | |
| KPMG Advisory Services Limited | BASIS SAAS | |
| Kaff Limited | BASIS SAAS | |
| Kaharba IT | BASIS SAAS | |
| Kaicom Solutions | BASIS SAAS | |
| Kaicom Solutions Japan BD Co. Ltd. | BASIS SAAS | |
| Kaizen IT Ltd. | BASIS SAAS | |
| Kamal Paterson Ltd | BASIS SAAS | |
| Kawaii Advanced Technology & Solution Limited | BASIS SAAS | |
| Kazla Technologies Ltd. | BASIS SAAS | |
| Khaas Food Limited | BASIS SAAS | |
| Khan IT Host | BASIS SAAS | |
| Khan Soft Limited | BASIS SAAS | |
| Kholabazaar International Limited | BASIS SAAS | |
| Kichai Business Solutions Ltd | BASIS SAAS | |
| Kite & Dart Limited | BASIS SAAS | |
| Klouder Limited | BASIS SAAS | |
| KloverCloud BD Ltd | BASIS SAAS | |
| Kolpolok Limited | BASIS SAAS | |
| Kotha Apps & Technologies Ltd. | BASIS SAAS | |
| Kovair Software Bangladesh Limited | BASIS SAAS | |
| Kreatech | BASIS SAAS | |
| L3 Ventures Limited | BASIS SAAS | |
| LCBS Dhaka Ltd | BASIS SAAS | |
| LCT Solution Center | BASIS SAAS | |
| LEADS Enterprise Solutions Limited | BASIS SAAS | |
| LEVERnGEAR LIMITED | BASIS SAAS | |
| LS Communications | BASIS SAAS | |
| LUMINALOGIK | BASIS SAAS | |
| LYNKTO LIMITED | BASIS SAAS | |
| Lalamove Bangladesh Limited | BASIS SAAS | |
| Lamda Telecom | BASIS SAAS | |
| Laser Vision Ltd. | BASIS SAAS | |
| Lausn Technology Bangladesh | BASIS SAAS | |
| Lead Academy Limited | BASIS SAAS | |
| Leading Edge Technology | BASIS SAAS | |
| Leads Training  and Consulting Ltd. | BASIS SAAS | |
| Leadswin Limited | BASIS SAAS | |
| Learn with Sumit LWS | BASIS SAAS | |
| Lebus Family Ltd | BASIS SAAS | |
| Legalized Education Bangladesh Ltd. | BASIS SAAS | |
| Lenden (BD) Ltd. | BASIS SAAS | |
| Leotech | BASIS SAAS | |
| Level3 Carrier Limited | BASIS SAAS | |
| Libanza Limited | BASIS SAAS | |
| LifePlus Bangladesh Ltd. | BASIS SAAS | |
| LifeSpring Tech Limited | BASIS SAAS | |
| Light Technologies | BASIS SAAS | |
| Light of Hope Ltd. | BASIS SAAS | |
| Limda Host | BASIS SAAS | |
| Limerick Resources Ltd | BASIS SAAS | |
| Line Reflection Ltd | BASIS SAAS | |
| Link-Up Technology Ltd | BASIS SAAS | |
| LinkTech IT | BASIS SAAS | |
| Live Entertainment Limited | BASIS SAAS | |
| Live Media Ltd. | BASIS SAAS | |
| Lobdhi | BASIS SAAS | |
| Logic & Thoughts | BASIS SAAS | |
| Logic Forum Limited | BASIS SAAS | |
| Login Technologies BD Ltd. | BASIS SAAS | |
| Loginex Ltd. | BASIS SAAS | |
| Logistech LTD | BASIS SAAS | |
| Looks Bangladesh | BASIS SAAS | |
| Lowkia Limited | BASIS SAAS | |
| LuminousLabs | BASIS SAAS | |
| Lynx International | BASIS SAAS | |
| M&T IT Tech Solutions | BASIS SAAS | |
| M/S . J.M.Corporation | BASIS SAAS | |
| M/S 2PI-BD | BASIS SAAS | |
| M/S Aalaadin.com | BASIS SAAS | |
| M/S Brandmyth Digital | BASIS SAAS | |
| M/S CLOUD STORAGE SOLUTIONS | BASIS SAAS | |
| M/S Chickadee | BASIS SAAS | |
| M/S Cloudly Solutions | BASIS SAAS | |
| M/S DIGITAL SCAN | BASIS SAAS | |
| M/S DataBind Technology | BASIS SAAS | |
| M/S Digital Decoder | BASIS SAAS | |
| M/S Electrohome | BASIS SAAS | |
| M/S F S Corporation | BASIS SAAS | |
| M/S Hamba Games | BASIS SAAS | |
| M/S Intelzaa | BASIS SAAS | |
| M/S MITALI INTERNATIONAL | BASIS SAAS | |
| M/S Northern Tech Bd | BASIS SAAS | |
| M/S Reliance Traders | BASIS SAAS | |
| M/S TechNickel | BASIS SAAS | |
| M/S. CCL IT | BASIS SAAS | |
| M/S. MSR Enterprise | BASIS SAAS | |
| M/s TechTrioZ Solutions | BASIS SAAS | |
| M/s. BUSPRO IT SOLUTIONS | BASIS SAAS | |
| M/s. Finalytics | BASIS SAAS | |
| M/s. MINDS AT WORK GLOBAL | BASIS SAAS | |
| M/s. Thunder Games | BASIS SAAS | |
| MA Network Service | BASIS SAAS | |
| MACRO SOLUTIONS LTD. | BASIS SAAS | |
| MADD Technology | BASIS SAAS | |
| MAK Tech Solution | BASIS SAAS | |
| MAPLE IT SOLUTIONS | BASIS SAAS | |
| MARK 1 Software | BASIS SAAS | |
| MARKSPHERE LIMITED | BASIS SAAS | |
| MB Software | BASIS SAAS | |
| MD Infotech | BASIS SAAS | |
| MDassist Bangladesh | BASIS SAAS | |
| ME SOLSHARE LIMITED | BASIS SAAS | |
| MH Technologies | BASIS SAAS | |
| MI2 Technology | BASIS SAAS | |
| MIAKI MEDIA LIMITED | BASIS SAAS | |
| MIM Technologies Limited | BASIS SAAS | |
| MIND CRAFT LIMITED | BASIS SAAS | |
| MINISOFT PARK | BASIS SAAS | |
| MIT ESP Bangladesh Private Ltd. | BASIS SAAS | |
| MM IT SOFT LTD | BASIS SAAS | |
| MR-Accountants | BASIS SAAS | |
| MRZ International | BASIS SAAS | |
| MSTUDIO Limited | BASIS SAAS | |
| MUSA Technologies Ltd. | BASIS SAAS | |
| MWT Informatics Limited. | BASIS SAAS | |
| MYEG(BD)LTD. | BASIS SAAS | |
| Maacc Media Ltd. | BASIS SAAS | |
| Machine Xtreme | BASIS SAAS | |
| Madly Ltd. | BASIS SAAS | |
| Madmen Digital Limited | BASIS SAAS | |
| Madvertancy IT | BASIS SAAS | |
| Maestro Solutions Ltd | BASIS SAAS | |
| Magnetism Tech Limited | BASIS SAAS | |
| Magnus Corporation Ltd. | BASIS SAAS | |
| Magnus Software Works | BASIS SAAS | |
| Maktro Electronics | BASIS SAAS | |
| Management and Training International Ltd | BASIS SAAS | |
| Mansha Negocis | BASIS SAAS | |
| Mantis A.I.R | BASIS SAAS | |
| Maple BPO | BASIS SAAS | |
| March Robotics & IT Solution Ltd. | BASIS SAAS | |
| Market Access Analytics & Consulting Limited | BASIS SAAS | |
| Marketever | BASIS SAAS | |
| Marlax Technologies Bangladesh | BASIS SAAS | |
| Marn IT Solutions | BASIS SAAS | |
| Match Wheel Ltd. | BASIS SAAS | |
| Mavengers Limited | BASIS SAAS | |
| Maverick Enterprise Limited | BASIS SAAS | |
| Max InfoTech Ltd. | BASIS SAAS | |
| Mayalogy Limited | BASIS SAAS | |
| MazeGeek Technologies BD Ltd. | BASIS SAAS | |
| Medical System Company Limited | BASIS SAAS | |
| Medina Tech Limited | BASIS SAAS | |
| Mediusware Ltd | BASIS SAAS | |
| Meenaclick Limited | BASIS SAAS | |
| Megatech GNBD Dhaka | BASIS SAAS | |
| MeghOps Limited | BASIS SAAS | |
| Mensa Digiworld | BASIS SAAS | |
| Meraki Innovations Limited | BASIS SAAS | |
| Meraki Technologies Limited | BASIS SAAS | |
| Merchant Bay Limited | BASIS SAAS | |
| Mercury IT International Limited | BASIS SAAS | |
| Mesh Technologies Limited | BASIS SAAS | |
| MetroSoft Bangladesh Limited | BASIS SAAS | |
| Metroonn Limited | BASIS SAAS | |
| Micro Parts USA Incorporation | BASIS SAAS | |
| Micro Solutions Limited | BASIS SAAS | |
| Microsec International Ltd | BASIS SAAS | |
| Microtech Interactive Ltd. | BASIS SAAS | |
| Microtech(BD)Systems | BASIS SAAS | |
| Microters | BASIS SAAS | |
| Microxen Technology | BASIS SAAS | |
| Milvik Bangladesh Ltd. | BASIS SAAS | |
| Mini Game Lab Limited | BASIS SAAS | |
| Misfit Technologies Limited | BASIS SAAS | |
| Mitisol Ltd. | BASIS SAAS | |
| Mitro Fintech Limited | BASIS SAAS | |
| MoMagic Bangladesh Ltd. | BASIS SAAS | |
| Modhumoti Tech | BASIS SAAS | |
| Moner Khabor | BASIS SAAS | |
| Mother Services Limited | BASIS SAAS | |
| Motion View | BASIS SAAS | |
| Mtech Bangladesh | BASIS SAAS | |
| Muktodhara Technology Limited | BASIS SAAS | |
| Mulytic Energy Solutions Ltd. | BASIS SAAS | |
| Munshe IT | BASIS SAAS | |
| Munshi HR Solutions Limited | BASIS SAAS | |
| Munshi IT Services | BASIS SAAS | |
| Musemind Digital Agency Ltd. | BASIS SAAS | |
| Musketeers Idea Ltd. | BASIS SAAS | |
| Mustache | BASIS SAAS | |
| Muttaqwi Incorporation | BASIS SAAS | |
| My Fuel Pump Limited | BASIS SAAS | |
| MyHealthbd.com | BASIS SAAS | |
| Mymensingh It Solutions | BASIS SAAS | |
| NAZIHAR IT SOLUTION LIMITED | BASIS SAAS | |
| NCSL | BASIS SAAS | |
| NDE Technology Services Ltd | BASIS SAAS | |
| NETWORLD TECHNOLOGY LTD. | BASIS SAAS | |
| NEXCET LTD | BASIS SAAS | |
| NG WAVE | BASIS SAAS | |
| NGAGE 360 LIMITED | BASIS SAAS | |
| NGen IT Limited | BASIS SAAS | |
| NIMBLE Code Execution System Ltd. | BASIS SAAS | |
| NITEX Solutions Ltd. | BASIS SAAS | |
| NITS service (Pvt.) Ltd. | BASIS SAAS | |
| NIramoy Healthtech Limited | BASIS SAAS | |
| NK Solutions Limited | BASIS SAAS | |
| NRB Solutions Limited | BASIS SAAS | |
| NRB Telecom Ltd. | BASIS SAAS | |
| NRD Bangladesh Limited | BASIS SAAS | |
| NSM Limited | BASIS SAAS | |
| NXGIT Soft | BASIS SAAS | |
| NZTECH | BASIS SAAS | |
| Nagad Ltd. | BASIS SAAS | |
| Nagadhat Bangladesh Limited | BASIS SAAS | |
| Nagorik Technologies Ltd. | BASIS SAAS | |
| Nanosoft System | BASIS SAAS | |
| National Institute of Engineering & Technology (NIET) Ltd. | BASIS SAAS | |
| National Institute of Fashion & Technology (NIFT) Ltd. | BASIS SAAS | |
| Native Digital Technologies Limited | BASIS SAAS | |
| Natty Com (Pvt) Ltd | BASIS SAAS | |
| Navigation BD Limited | BASIS SAAS | |
| Navigator Technologies | BASIS SAAS | |
| Nazabi | BASIS SAAS | |
| Nazihar Tech Limited | BASIS SAAS | |
| Neeramoy Digital Services Ltd | BASIS SAAS | |
| Nelsis Limited | BASIS SAAS | |
| Nerddevs Ltd. | BASIS SAAS | |
| Nessbit Technologies Limited | BASIS SAAS | |
| Net Planet Soft & Engineering | BASIS SAAS | |
| NetCoden | BASIS SAAS | |
| Netconnect Ltd. | BASIS SAAS | |
| Netvent Dhaka Limited | BASIS SAAS | |
| Neural Semiconductor Limited | BASIS SAAS | |
| Neuron33 Ltd. | BASIS SAAS | |
| Nevronus Systems | BASIS SAAS | |
| New Eagle Video and VCD Centre | BASIS SAAS | |
| New Horizons Software Development Center | BASIS SAAS | |
| New Trizons IT | BASIS SAAS | |
| NewVision Solutions Ltd. | BASIS SAAS | |
| Newroz Technologies Limited | BASIS SAAS | |
| News Bangla Media Ltd | BASIS SAAS | |
| NexKraft Limited | BASIS SAAS | |
| Nexalinx | BASIS SAAS | |
| Nexel Research Ltd. | BASIS SAAS | |
| Nexo Technologies Ltd | BASIS SAAS | |
| Next Generation Information Technology | BASIS SAAS | |
| Next Solution Lab | BASIS SAAS | |
| Next Tel Communication | BASIS SAAS | |
| NextGen Bangladesh | BASIS SAAS | |
| NextGen Data Systems LTD. | BASIS SAAS | |
| NextGen Software & Solutions Ltd. | BASIS SAAS | |
| NextLab | BASIS SAAS | |
| Nextbangla Limited | BASIS SAAS | |
| Nextive Solution | BASIS SAAS | |
| Nextzen Limited | BASIS SAAS | |
| Niama International | BASIS SAAS | |
| Nifty Coders Pvt. LTD. | BASIS SAAS | |
| Nifty IT Solution LTD. | BASIS SAAS | |
| Nifty Informatics Limited | BASIS SAAS | |
| Nirupon Limited | BASIS SAAS | |
| Nitsol Bangladesh Ltd | BASIS SAAS | |
| Noble IT Solution | BASIS SAAS | |
| Nodes Digital Limited | BASIS SAAS | |
| Nongmin Consultancy Services Ltd. | BASIS SAAS | |
| Notionhive Bangladesh Limited | BASIS SAAS | |
| Nova Labs Limited | BASIS SAAS | |
| Nreach-Net (Pvt.) Limited | BASIS SAAS | |
| Nuport Industrial Automation Ltd. | BASIS SAAS | |
| Nusratech Pte Ltd. | BASIS SAAS | |
| Nvisio Solutions Limited | BASIS SAAS | |
| NybSys (Pvt) Ltd. | BASIS SAAS | |
| OFFSHORE IT | BASIS SAAS | |
| OITIJJHYA | BASIS SAAS | |
| OMEXPRESS | BASIS SAAS | |
| ON TRACK LINK | BASIS SAAS | |
| ORANGE IT LTD. | BASIS SAAS | |
| ORANGE SOLUTIONS LTD. | BASIS SAAS | |
| OS CLiCKS | BASIS SAAS | |
| OS IT Solutions Ltd | BASIS SAAS | |
| OSINT Tech Limited | BASIS SAAS | |
| OSTAD LIMITED | BASIS SAAS | |
| OSV Bangladesh Limited | BASIS SAAS | |
| OTAE Bangladesh Ltd. | BASIS SAAS | |
| OTOMATIC | BASIS SAAS | |
| Obhai Solutions Limited | BASIS SAAS | |
| Object Canvas Technology | BASIS SAAS | |
| Oblivion Solutions Limited | BASIS SAAS | |
| Oceanize Lab | BASIS SAAS | |
| Octaglory Limited | BASIS SAAS | |
| Octaglory Retail Technology Limited | BASIS SAAS | |
| Octavia Digital | BASIS SAAS | |
| Octopi Digital Ltd. | BASIS SAAS | |
| Octopi Technology Limited | BASIS SAAS | |
| Octopus Communications Limited | BASIS SAAS | |
| Oculin Networks Limited | BASIS SAAS | |
| Oculin Tech BD Ltd. | BASIS SAAS | |
| Odhikar Media Ltd | BASIS SAAS | |
| Odin Outsourcing | BASIS SAAS | |
| Odyssey Apps Ltd. | BASIS SAAS | |
| Ogroni Informatix Limited | BASIS SAAS | |
| Omega Tech Limited | BASIS SAAS | |
| Omni Solutions Ltd | BASIS SAAS | |
| Omnitech Solutions Ltd. | BASIS SAAS | |
| Omnixima | BASIS SAAS | |
| On The Way | BASIS SAAS | |
| One Sky Communications Limited | BASIS SAAS | |
| OneLittleWeb Ltd | BASIS SAAS | |
| OneiTech | BASIS SAAS | |
| Oneixchange Ltd. | BASIS SAAS | |
| Oner Systems Limited | BASIS SAAS | |
| Online Marketing Service | BASIS SAAS | |
| Online Tech Academy | BASIS SAAS | |
| Onnow Limited | BASIS SAAS | |
| Opedia Technologies Limited | BASIS SAAS | |
| Open Communication Ltd. | BASIS SAAS | |
| OpenRefactory Bangladesh Limited | BASIS SAAS | |
| Optimal Technology (Pvt.) Ltd. | BASIS SAAS | |
| Optimum Services Ltd. | BASIS SAAS | |
| Optimum Soft | BASIS SAAS | |
| Optimum Software and Services Development Network Ltd | BASIS SAAS | |
| Optimum Solution and Services Ltd. | BASIS SAAS | |
| Orbit Digital Solutions Ltd. | BASIS SAAS | |
| Orbit IT Limited | BASIS SAAS | |
| Orboroi Bangladesh Ltd | BASIS SAAS | |
| Org-Quest Research Limited | BASIS SAAS | |
| Orient Computers | BASIS SAAS | |
| Orko Health Limited | BASIS SAAS | |
| Oshudghor | BASIS SAAS | |
| Otix Technologies | BASIS SAAS | |
| Outsourcing Institute | BASIS SAAS | |
| P Tune Studio | BASIS SAAS | |
| P.I. Ocean Soft Tech | BASIS SAAS | |
| PANTOMIME LIMITED | BASIS SAAS | |
| PAP International Ltd. | BASIS SAAS | |
| PARKWAY TECHNOLOGY LIMITED | BASIS SAAS | |
| PAYMENTSAVE BD LIMITED | BASIS SAAS | |
| PBS Limited | BASIS SAAS | |
| PEARS GLOBAL LIMITED | BASIS SAAS | |
| PENTA GLOBAL LIMITED | BASIS SAAS | |
| PHOENIX SOFTWARE | BASIS SAAS | |
| PI Software Ltd. | BASIS SAAS | |
| PIXELS BD | BASIS SAAS | |
| PLEXUS | BASIS SAAS | |
| PM Expert Limited | BASIS SAAS | |
| PMaspire Technologies | BASIS SAAS | |
| PORTBLISS LIMITED | BASIS SAAS | |
| PRACHURJO ENGINEERING | BASIS SAAS | |
| PRIME NET LTD. | BASIS SAAS | |
| PRINK | BASIS SAAS | |
| PUNDIT | BASIS SAAS | |
| PURPLE IT LIMITED | BASIS SAAS | |
| Pakiza Software Limited | BASIS SAAS | |
| Pakiza Technovation Ltd. | BASIS SAAS | |
| Pallabi Business Services | BASIS SAAS | |
| Panorama Management Advisory Services Limited | BASIS SAAS | |
| Paperfly Pvt. Ltd. | BASIS SAAS | |
| Parallaxlogic Infotech | BASIS SAAS | |
| Paribahan.com Limited | BASIS SAAS | |
| ParonSoft Solutions Limited | BASIS SAAS | |
| Pathao Limited | BASIS SAAS | |
| Paul & Paul Consultants Limited | BASIS SAAS | |
| Pearl Consultant Ltd. | BASIS SAAS | |
| Pentanik IT Solution Park | BASIS SAAS | |
| Peoples Information and Technology Incorporation | BASIS SAAS | |
| Periscope Labs Limited | BASIS SAAS | |
| Perky Rabbit Corporation Limited | BASIS SAAS | |
| Picasa Limited | BASIS SAAS | |
| Picredo Software Limited | BASIS SAAS | |
| Piistech Limited | BASIS SAAS | |
| Ping BD | BASIS SAAS | |
| Pinkwhale Technologies | BASIS SAAS | |
| Pinnacle Crest | BASIS SAAS | |
| Pinovation Tech Ltd. | BASIS SAAS | |
| Pipeline Bangladesh Ltd | BASIS SAAS | |
| Pipilika Soft | BASIS SAAS | |
| Pirthe Limited | BASIS SAAS | |
| Pixamatics Technology Ltd | BASIS SAAS | |
| PixelVega Limited | BASIS SAAS | |
| Pixency | BASIS SAAS | |
| Planet Hack Limited | BASIS SAAS | |
| Planex Technologies Ltd. | BASIS SAAS | |
| PlayOn 24 | BASIS SAAS | |
| Playnoob | BASIS SAAS | |
| Plutus Consulting | BASIS SAAS | |
| PolicyHuT Bangladesh Limited | BASIS SAAS | |
| Pollux Technology Solutions | BASIS SAAS | |
| Polygon Information and Technology Limited | BASIS SAAS | |
| Polyuno BD | BASIS SAAS | |
| Popular IT | BASIS SAAS | |
| Poshora Services Limited | BASIS SAAS | |
| Powerbits Ltd. | BASIS SAAS | |
| Pranon Global Ltd. | BASIS SAAS | |
| Prediction Infotech Limited | BASIS SAAS | |
| Prefeex Limited | BASIS SAAS | |
| Prem IT | BASIS SAAS | |
| PricewaterhouseCoopers Bangladesh Private Limited | BASIS SAAS | |
| Primacy Infotech Ltd. | BASIS SAAS | |
| Prime Resource Solutions Ltd. | BASIS SAAS | |
| Primex information Systems Limited | BASIS SAAS | |
| Privilege Engineering Ltd | BASIS SAAS | |
| Privilege Technologies Ltd | BASIS SAAS | |
| PriyoShop.com Ltd. | BASIS SAAS | |
| PriyoSys Ltd. | BASIS SAAS | |
| Pro Technology Solution | BASIS SAAS | |
| ProAms | BASIS SAAS | |
| ProSystem Limited | BASIS SAAS | |
| Probha Aurora Ltd. | BASIS SAAS | |
| Prodata Ltd. | BASIS SAAS | |
| Progeny Technologies Ltd | BASIS SAAS | |
| Programming Hero | BASIS SAAS | |
| Progress Tech Limited. | BASIS SAAS | |
| Project2Morrow Consulting Services | BASIS SAAS | |
| Provati Courier Limited | BASIS SAAS | |
| Publix Metro Ltd | BASIS SAAS | |
| Pulse Tech Ltd. | BASIS SAAS | |
| Purple Patch | BASIS SAAS | |
| Putul Host | BASIS SAAS | |
| QA Harbor Limited | BASIS SAAS | |
| QA Pro Limited | BASIS SAAS | |
| QYS Networking & Solutions Ltd. | BASIS SAAS | |
| Qtec Solution Limited | BASIS SAAS | |
| Quadque Technologies Pvt. Limited | BASIS SAAS | |
| Quantanite Bangladesh Limited | BASIS SAAS | |
| Quantum Vault International | BASIS SAAS | |
| Qubits Ltd. | BASIS SAAS | |
| Quest BDC Limited | BASIS SAAS | |
| Quintet Alliance Pvt. Ltd | BASIS SAAS | |
| R&H Business Solution | BASIS SAAS | |
| RAAZ IT CENTER | BASIS SAAS | |
| RAIDA-IT | BASIS SAAS | |
| RBD SOFTWARE & TECHNOLOGY LIMITED | BASIS SAAS | |
| RD Services Limited | BASIS SAAS | |
| REBING TECH | BASIS SAAS | |
| RECENT TOUCH BANGLADESH LIMITED | BASIS SAAS | |
| RED IT INTERNATIONAL LTD. | BASIS SAAS | |
| REIT LIMITED | BASIS SAAS | |
| RENSSOFT SOLUTIONS LIMITED | BASIS SAAS | |
| REPLIQ Limited | BASIS SAAS | |
| RESDA | BASIS SAAS | |
| REVINNS LIMITED | BASIS SAAS | |
| RILO IT & Software Ltd. | BASIS SAAS | |
| RODRIGO.exe | BASIS SAAS | |
| RONS TECH | BASIS SAAS | |
| ROYAL IT LIMITED | BASIS SAAS | |
| RPSI SERVICES LTD | BASIS SAAS | |
| RS Information and Technology | BASIS SAAS | |
| Rabbi It Firm | BASIS SAAS | |
| Rabbit Code | BASIS SAAS | |
| Race Online Ltd. | BASIS SAAS | |
| Racssoft | BASIS SAAS | |
| Raif Technology Ltd | BASIS SAAS | |
| Raindrops Tech Ltd. | BASIS SAAS | |
| Rancom Trading (PVT) Ltd. | BASIS SAAS | |
| Rankmylist Bangladesh Ltd. | BASIS SAAS | |
| Ranks ITT Limited | BASIS SAAS | |
| Rankwis | BASIS SAAS | |
| Rational Technologies Ltd. | BASIS SAAS | |
| Recall (BD) Ltd. | BASIS SAAS | |
| Recom Consulting Limited | BASIS SAAS | |
| RedDot Digital Limited | BASIS SAAS | |
| Redington Bangladesh Limited | BASIS SAAS | |
| Redviolet Digital Limited | BASIS SAAS | |
| ReformedTech | BASIS SAAS | |
| Regency Tech City Limited | BASIS SAAS | |
| Regnum Resource Ltd. | BASIS SAAS | |
| Reliance IT | BASIS SAAS | |
| Relief Validation Limited | BASIS SAAS | |
| Renegades Art | BASIS SAAS | |
| Renessa Info Systems Limited | BASIS SAAS | |
| ReplyMind AI Limited | BASIS SAAS | |
| Retina Soft | BASIS SAAS | |
| Revo Interactive | BASIS SAAS | |
| Ridmik Labs Limited | BASIS SAAS | |
| RightClick Solutions Limited | BASIS SAAS | |
| Ringer Soft Limited | BASIS SAAS | |
| Risda Institute of technology LTD | BASIS SAAS | |
| RoBenDevs | BASIS SAAS | |
| Robust Research And Development Ltd. | BASIS SAAS | |
| Rocketman Limited | BASIS SAAS | |
| Romoni Services Limited | BASIS SAAS | |
| RootNext Solutions | BASIS SAAS | |
| RoseTech Solutions Limited | BASIS SAAS | |
| Royal Soft Limited | BASIS SAAS | |
| Rubytech | BASIS SAAS | |
| Runway Tech Ltd. | BASIS SAAS | |
| S-Tech Limited | BASIS SAAS | |
| SA Tech & Consultancy | BASIS SAAS | |
| SAM IT PARK | BASIS SAAS | |
| SAM Online | BASIS SAAS | |
| SAMSUNG R&D INSTITUTE BANGLADESH LTD. | BASIS SAAS | |
| SANBJ LIMITED | BASIS SAAS | |
| SARTECH INNOVATION & SERVICES LTD. | BASIS SAAS | |
| SAVVY TECHMART LIMITED | BASIS SAAS | |
| SBS CORPORATION | BASIS SAAS | |
| SCHOPE Infotech Limited | BASIS SAAS | |
| SCT-Bangla Limited | BASIS SAAS | |
| SELISE Bangladesh Limited | BASIS SAAS | |
| SEO EXPATE BANGLADESH LTD | BASIS SAAS | |
| SERVIFY TECH LTD | BASIS SAAS | |
| SHEBA XEN TECH LIMITED | BASIS SAAS | |
| SHUVO IT | BASIS SAAS | |
| SI2 Limited | BASIS SAAS | |
| SIGMIND.ai | BASIS SAAS | |
| SILICON ORCHARD LTD. | BASIS SAAS | |
| SKYDO | BASIS SAAS | |
| SM FINTECH LTD | BASIS SAAS | |
| SMAC IT LIMITED | BASIS SAAS | |
| SMART INNOVATIONS LIMITED | BASIS SAAS | |
| SMART-trend Digital | BASIS SAAS | |
| SMARTMATRIX PTE. LTD. | BASIS SAAS | |
| SME Informatics Ltd. | BASIS SAAS | |
| SMG SOFTECH LTD. | BASIS SAAS | |
| SNEHO Digital Limited | BASIS SAAS | |
| SOFT HOST IT | BASIS SAAS | |
| SOFTAVION LIMITED | BASIS SAAS | |
| SOFTEKO | BASIS SAAS | |
| SOFTIC OPC | BASIS SAAS | |
| SOLVERS | BASIS SAAS | |
| SOTbizz IT Firm | BASIS SAAS | |
| SOUTH POINT TECHNOLOGY | BASIS SAAS | |
| SPEEDWAY SOLUTIONS LTD. | BASIS SAAS | |
| SPONDON | BASIS SAAS | |
| SPRING RAIN PRIVATE LIMITED | BASIS SAAS | |
| SR Solutions | BASIS SAAS | |
| SRRK IT Limited | BASIS SAAS | |
| SRS Idea Limited | BASIS SAAS | |
| STARTISE LIMITED | BASIS SAAS | |
| STATA IT Limited | BASIS SAAS | |
| STELLAR DIGITAL LIMITED | BASIS SAAS | |
| STR IT SOLUTION | BASIS SAAS | |
| STUDIO IMAGINE | BASIS SAAS | |
| SUNCROPS Ltd. | BASIS SAAS | |
| SUSUSOFT Ltd. | BASIS SAAS | |
| SVAM BANGLADESH PRIVATE LIMITED | BASIS SAAS | |
| SWISS SOFT | BASIS SAAS | |
| SYSSOLUTION | BASIS SAAS | |
| Sab Tech | BASIS SAAS | |
| Saic Institute of Management & Technology (SIMT) | BASIS SAAS | |
| Salaam Network Solutions Ltd. | BASIS SAAS | |
| Samadhan Solution PTY Ltd. | BASIS SAAS | |
| Samaira Skill Development Institute (SSDI) | BASIS SAAS | |
| Samurai System Limited | BASIS SAAS | |
| Sanaz Corporation | BASIS SAAS | |
| Satej Ltd | BASIS SAAS | |
| Sayburgh Solution Limited | BASIS SAAS | |
| Sazim Tech Limited | BASIS SAAS | |
| ScITech Consulting and Solutions Limited | BASIS SAAS | |
| Scoppa Technologies Ltd | BASIS SAAS | |
| Scube Technologies Ltd | BASIS SAAS | |
| SecureMetrics Systems | BASIS SAAS | |
| Selgus Technology Inc | BASIS SAAS | |
| Selopia | BASIS SAAS | |
| Semicolon IT Solutions | BASIS SAAS | |
| Semion Limited | BASIS SAAS | |
| Sentinel Technologies Limited | BASIS SAAS | |
| ServiPro Solutions Ltd | BASIS SAAS | |
| Shadhin Fintech Solutions Limited | BASIS SAAS | |
| Shadhin Music Limited | BASIS SAAS | |
| Shadhin Technologies Limited | BASIS SAAS | |
| Shadowhite Animators Limited | BASIS SAAS | |
| Shahjalal Software Pvt. Ltd. | BASIS SAAS | |
| Shajao | BASIS SAAS | |
| Shajgoj Limited | BASIS SAAS | |
| Shampan IT Solution | BASIS SAAS | |
| Sharabir.com | BASIS SAAS | |
| ShareTrip Ltd. | BASIS SAAS | |
| Sharoz international limited | BASIS SAAS | |
| Shataj Soft | BASIS SAAS | |
| Sheam Aviation Services Ltd. | BASIS SAAS | |
| Sheba Fintech Limited | BASIS SAAS | |
| Sheba Technologies Limited | BASIS SAAS | |
| Sheba.xyz Services Limited | BASIS SAAS | |
| Shell Technologies | BASIS SAAS | |
| Shikhbe Shobai Solutions | BASIS SAAS | |
| Shikho Technologies Bangladesh Limited | BASIS SAAS | |
| Shohagh Paribahan Pvt. Ltd. | BASIS SAAS | |
| Shohay Technologies Bangladesh Ltd. | BASIS SAAS | |
| Shohoj Limited | BASIS SAAS | |
| Shomvob Technologies Limited | BASIS SAAS | |
| Shonod | BASIS SAAS | |
| Shopfront Limited | BASIS SAAS | |
| Shorborno Holdings Limited | BASIS SAAS | |
| Shorobor IT | BASIS SAAS | |
| ShuktaraSoft | BASIS SAAS | |
| Shunno Ek Limited | BASIS SAAS | |
| Shunno Tech & Innovation | BASIS SAAS | |
| Shuttle Technologies BD Limited | BASIS SAAS | |
| Siara Solutions | BASIS SAAS | |
| Siddiqui Perl Tech Incorporated | BASIS SAAS | |
| Sigma Solutions | BASIS SAAS | |
| Silicon Computing Ltd | BASIS SAAS | |
| Silver Water Technologies Bangladesh Ltd | BASIS SAAS | |
| Singularity Limited | BASIS SAAS | |
| Six Generation IT Limited | BASIS SAAS | |
| Skies Engineering & Technologies Ltd | BASIS SAAS | |
| Skill Service Limited | BASIS SAAS | |
| Skillers Zone | BASIS SAAS | |
| Sky Digital (BD) Limited | BASIS SAAS | |
| SkyTech Solutions | BASIS SAAS | |
| Skycon Solutions | BASIS SAAS | |
| Skylark Soft Limited | BASIS SAAS | |
| Smart Card IT Solutions Bangladesh Limited | BASIS SAAS | |
| Smart Field Service | BASIS SAAS | |
| Smart Lab | BASIS SAAS | |
| Smart Software Solution | BASIS SAAS | |
| Smart Solution for Software | BASIS SAAS | |
| Smart Technologies (BD) Ltd. | BASIS SAAS | |
| Smart Toll Solution BD | BASIS SAAS | |
| Smart Voice Limited | BASIS SAAS | |
| Smart Web Source | BASIS SAAS | |
| SmartDataSoft | BASIS SAAS | |
| SmartGo Solutions Limited | BASIS SAAS | |
| Soft Code | BASIS SAAS | |
| Soft IT Security | BASIS SAAS | |
| Soft Park | BASIS SAAS | |
| Soft Ratio | BASIS SAAS | |
| Soft Tech Innovation Ltd | BASIS SAAS | |
| Soft Valley | BASIS SAAS | |
| SoftCare IT | BASIS SAAS | |
| SoftHut Ltd. | BASIS SAAS | |
| SoftShore Technology | BASIS SAAS | |
| Softalogy Limited | BASIS SAAS | |
| Softify Technologies | BASIS SAAS | |
| Softin Technology Ltd. | BASIS SAAS | |
| Softnet BD | BASIS SAAS | |
| Softnmart Limited | BASIS SAAS | |
| Softograph Ltd. | BASIS SAAS | |
| Softopark IT Ltd | BASIS SAAS | |
| Softrobotics Bangladesh Ltd. | BASIS SAAS | |
| Softtech Solution | BASIS SAAS | |
| Softtech71 | BASIS SAAS | |
| Software Bazar Bangladesh | BASIS SAAS | |
| Software Global Consultancy PVT LTD | BASIS SAAS | |
| Software Lighthouse | BASIS SAAS | |
| Software Shell | BASIS SAAS | |
| Software Solutions And Logistics Enterprise Limited | BASIS SAAS | |
| Softwrd Ltd | BASIS SAAS | |
| Softzino Technologies | BASIS SAAS | |
| Solution Hub Technologies | BASIS SAAS | |
| SolutionSpin Limited | BASIS SAAS | |
| Solutya Private Limited | BASIS SAAS | |
| Somikoron IT Ltd. | BASIS SAAS | |
| Somoy Media Limited | BASIS SAAS | |
| Sonali IT | BASIS SAAS | |
| Sonali Intellect Ltd | BASIS SAAS | |
| Soppiya Innovation Limited | BASIS SAAS | |
| South Asian Software & Engineering Corporation | BASIS SAAS | |
| SpaGreen Creative | BASIS SAAS | |
| Spark IT Solution | BASIS SAAS | |
| Spate Initiative Limited | BASIS SAAS | |
| Spectra International Ltd. | BASIS SAAS | |
| Spectrum IT Solutions Ltd. | BASIS SAAS | |
| Speed Tech Online | BASIS SAAS | |
| Spellbound Communications Limited | BASIS SAAS | |
| Spider Digital Security | BASIS SAAS | |
| Spotter Private Limited | BASIS SAAS | |
| Squad Innovators | BASIS SAAS | |
| Star Infotech Limited | BASIS SAAS | |
| Star Tech & Engineering Ltd. | BASIS SAAS | |
| Stargate Communications Ltd. | BASIS SAAS | |
| Starlink Engineering Ltd. | BASIS SAAS | |
| Startup Tech BD Limited | BASIS SAAS | |
| StaticMania | BASIS SAAS | |
| Steinwerk OPC | BASIS SAAS | |
| Stockwell International | BASIS SAAS | |
| Strategic BD Lead Corporation | BASIS SAAS | |
| Strategic Transformation Consultants | BASIS SAAS | |
| Strativ BD Limited | BASIS SAAS | |
| Studio Mason Ltd. | BASIS SAAS | |
| Studio Metrodesk | BASIS SAAS | |
| Suffix IT Limited | BASIS SAAS | |
| Sumations Bangladesh | BASIS SAAS | |
| Suncity Biz | BASIS SAAS | |
| Sunshine It | BASIS SAAS | |
| Suranjali | BASIS SAAS | |
| Surat | BASIS SAAS | |
| Swapnoloke | BASIS SAAS | |
| Switch Com Ltd. | BASIS SAAS | |
| Symbiosis IT | BASIS SAAS | |
| Synnova Pty Ltd. | BASIS SAAS | |
| Sys Dev Ltd. | BASIS SAAS | |
| Syscomatic Technologies | BASIS SAAS | |
| Syscon Solution Limited | BASIS SAAS | |
| Sysnest Limited | BASIS SAAS | |
| System Netware | BASIS SAAS | |
| SystemEye Technologies Ltd. | BASIS SAAS | |
| Systems & Services Limited | BASIS SAAS | |
| T3 Communications Limited | BASIS SAAS | |
| TALENT PRO | BASIS SAAS | |
| TBN BD Ltd | BASIS SAAS | |
| TBZ ENGINEERING | BASIS SAAS | |
| TECHGATE SOFTWARE LIMITED | BASIS SAAS | |
| TECHLAND | BASIS SAAS | |
| TECHLOGICIANS SOLUTIONS | BASIS SAAS | |
| TECHNOBD LIMITED | BASIS SAAS | |
| TECHNOMETRICS LIMITED | BASIS SAAS | |
| TECHSOCO | BASIS SAAS | |
| TECHSOL Technologies Bangladesh Limited | BASIS SAAS | |
| TEXXIT BD | BASIS SAAS | |
| THE GREEN HELPERS | BASIS SAAS | |
| THE KOW COMPANY LIMITED | BASIS SAAS | |
| THEMATIC LTD. | BASIS SAAS | |
| THESOFTKING LIMITED | BASIS SAAS | |
| TIME RESEARCH & INNOVATION LTD | BASIS SAAS | |
| TMAS - Crafting Agility | BASIS SAAS | |
| TMSS ICT Ltd. | BASIS SAAS | |
| TOS Technology Ltd. | BASIS SAAS | |
| TOTALOFFTEC | BASIS SAAS | |
| TR Systems Ltd. | BASIS SAAS | |
| TRI Digital Technologies Ltd | BASIS SAAS | |
| TS4U Limited | BASIS SAAS | |
| TULIPTECH LTD. | BASIS SAAS | |
| TUUO SOLUTIONS LIMITED | BASIS SAAS | |
| TWINPEAK Business Corporation Limited | BASIS SAAS | |
| Tactsoft Ltd | BASIS SAAS | |
| Tafuri Technologies Limited | BASIS SAAS | |
| TagIT Solutions Limited | BASIS SAAS | |
| Taham Express | BASIS SAAS | |
| Takshal .Com | BASIS SAAS | |
| Talvette Limited | BASIS SAAS | |
| Tangail Digital It Firm | BASIS SAAS | |
| Tangram Tech Solutions Limited | BASIS SAAS | |
| Tanjid's Studio | BASIS SAAS | |
| Taqwa Enterprise | BASIS SAAS | |
| Tara Tech Limited | BASIS SAAS | |
| Tarun Soft (PVT) Limited | BASIS SAAS | |
| Team Platform Ltd. | BASIS SAAS | |
| Tech Aroma Ltd | BASIS SAAS | |
| Tech Bhai | BASIS SAAS | |
| Tech Blue Ocean Pvt. Ltd. | BASIS SAAS | |
| Tech Built Ltd | BASIS SAAS | |
| Tech Hive Limited | BASIS SAAS | |
| Tech Hub Bangladesh | BASIS SAAS | |
| Tech Intelligence Limited | BASIS SAAS | |
| Tech Lab Pro | BASIS SAAS | |
| Tech Lab33 Limited | BASIS SAAS | |
| Tech Solution Factory | BASIS SAAS | |
| Tech Solution IT Ltd | BASIS SAAS | |
| Tech Terrain IT Limited | BASIS SAAS | |
| Tech Valley Networks Limited | BASIS SAAS | |
| Tech Village ITES Ltd. | BASIS SAAS | |
| Tech Vision | BASIS SAAS | |
| Tech for Biz Limited | BASIS SAAS | |
| TechBPO Pro | BASIS SAAS | |
| TechBrigades LTD | BASIS SAAS | |
| TechCare Technologies Limited | BASIS SAAS | |
| TechForing Ltd | BASIS SAAS | |
| TechGarlic Limited | BASIS SAAS | |
| TechKnowGram Limited | BASIS SAAS | |
| TechMellow | BASIS SAAS | |
| TechMinds Ltd | BASIS SAAS | |
| TechMonstar Limited | BASIS SAAS | |
| TechOptions | BASIS SAAS | |
| TechSparkIT Limited | BASIS SAAS | |
| Techabyte Solutions | BASIS SAAS | |
| Techbee Solutions Limited | BASIS SAAS | |
| Techdyno BD Ltd | BASIS SAAS | |
| Techetron Ventures Ltd | BASIS SAAS | |
| Techgenix | BASIS SAAS | |
| Technext Limited | BASIS SAAS | |
| Techniche Consulting Services Bangladesh | BASIS SAAS | |
| Techno Mole Creations Ltd. | BASIS SAAS | |
| Techno Safety Limited | BASIS SAAS | |
| Techno Solutions & Services Limited | BASIS SAAS | |
| TechnoArt Software | BASIS SAAS | |
| TechnoMarine Solutions Limited | BASIS SAAS | |
| TechnoPx Digital Ltd. | BASIS SAAS | |
| Technocore Bangladesh Limited | BASIS SAAS | |
| Technofair IT Limited | BASIS SAAS | |
| Technomedia Ltd. | BASIS SAAS | |
| Technosoft Integration | BASIS SAAS | |
| Techntalents | BASIS SAAS | |
| Tecognize Solutions Ltd. | BASIS SAAS | |
| Tedfo Bangladesh Limited | BASIS SAAS | |
| Teknovus Limited | BASIS SAAS | |
| Telcobright Limited | BASIS SAAS | |
| Telecontran Limited | BASIS SAAS | |
| Telerad Bangladesh Ltd. | BASIS SAAS | |
| Tenbyte Limited | BASIS SAAS | |
| Teton Private Ltd. | BASIS SAAS | |
| TetraHost Bangladesh | BASIS SAAS | |
| Thakral One Private Limited | BASIS SAAS | |
| Thane Systems | BASIS SAAS | |
| The Arcade Bangladesh Limited | BASIS SAAS | |
| The Design Park | BASIS SAAS | |
| The Everest IT | BASIS SAAS | |
| The ICT Hub | BASIS SAAS | |
| The Mighty Byte Ltd | BASIS SAAS | |
| The Sygnius Limited | BASIS SAAS | |
| The Tork Incorporation | BASIS SAAS | |
| The waresun Limited | BASIS SAAS | |
| ThemeXpert | BASIS SAAS | |
| Themefisher | BASIS SAAS | |
| Themeperch ltd | BASIS SAAS | |
| Themewinter | BASIS SAAS | |
| Think & Sync Limited | BASIS SAAS | |
| Think Limited | BASIS SAAS | |
| ThinkBig Solutions Ltd. | BASIS SAAS | |
| Thriving Skills Limited | BASIS SAAS | |
| Tiger Park Limited | BASIS SAAS | |
| Tiger Soft BD | BASIS SAAS | |
| Tiller | BASIS SAAS | |
| Times Innovation | BASIS SAAS | |
| Tinkers Technologies Limited | BASIS SAAS | |
| Tirzok Private Limited | BASIS SAAS | |
| Titan Technologies Ltd | BASIS SAAS | |
| Tix Ninja | BASIS SAAS | |
| Tlntrip | BASIS SAAS | |
| Toggi Services Limited | BASIS SAAS | |
| ToguMogu Pvt. Limited | BASIS SAAS | |
| Total Digital Solutions Soft Link | BASIS SAAS | |
| Trademajestic Limited | BASIS SAAS | |
| Traideas | BASIS SAAS | |
| Traveller Global Ltd. | BASIS SAAS | |
| TraydCom Technology Ltd. | BASIS SAAS | |
| Trends Bird Limited | BASIS SAAS | |
| Tri-Vision Limited | BASIS SAAS | |
| Trillion Bits Ltd | BASIS SAAS | |
| Trimatric AI | BASIS SAAS | |
| TripeGate | BASIS SAAS | |
| Truck Lagbe Limited | BASIS SAAS | |
| Trust Innovation Limited | BASIS SAAS | |
| Trust It | BASIS SAAS | |
| Trustaira Limited | BASIS SAAS | |
| Turnago IT & Technical Training Center | BASIS SAAS | |
| Turtle Solutions Limited | BASIS SAAS | |
| Tutor Club Site | BASIS SAAS | |
| TutorsInc Ltd. | BASIS SAAS | |
| Twinforce Solutions Limited | BASIS SAAS | |
| UCB Fintech Company Ltd. | BASIS SAAS | |
| UDC CONSTRUCTION LTD. | BASIS SAAS | |
| UFO Interactive Ltd. | BASIS SAAS | |
| UK Bangla IT LIMITED | BASIS SAAS | |
| ULTRA - X BD LIMITED | BASIS SAAS | |
| UMRLabs | BASIS SAAS | |
| UNICOM BANGLADESH | BASIS SAAS | |
| UNILABEL CORPORATION | BASIS SAAS | |
| UNION-MULTITECH CORPORATION | BASIS SAAS | |
| UNISHOP | BASIS SAAS | |
| UPSTRA Communications Ltd. | BASIS SAAS | |
| UUMOO LIMITED | BASIS SAAS | |
| UY Lab | BASIS SAAS | |
| Uddom Business Services Ltd | BASIS SAAS | |
| Udvash-Unmesh Online Care | BASIS SAAS | |
| UhuruTek Solutions | BASIS SAAS | |
| Ui Barn Limited | BASIS SAAS | |
| Ulka Games Limited | BASIS SAAS | |
| Ultimate IT Solution Limited | BASIS SAAS | |
| Unified Core Ltd. | BASIS SAAS | |
| Unifon Limited | BASIS SAAS | |
| Unigo Solutions | BASIS SAAS | |
| Unimation Infrastructures | BASIS SAAS | |
| Unipro software bd ltd | BASIS SAAS | |
| Unique Consortium Limited | BASIS SAAS | |
| Unisoft Business Solutions Ltd | BASIS SAAS | |
| UnivaHost | BASIS SAAS | |
| Universal Trading & Services | BASIS SAAS | |
| UnlockLive IT Limited | BASIS SAAS | |
| Update Solutions Technologies Ltd. | BASIS SAAS | |
| Upgrade U initiative Ltd | BASIS SAAS | |
| Uptech Solution Limited | BASIS SAAS | |
| Utopia Private Ltd. | BASIS SAAS | |
| Utshab Technology Ltd. | BASIS SAAS | |
| V2 Technologies Ltd. | BASIS SAAS | |
| VC World | BASIS SAAS | |
| VENUS IT LIMITED | BASIS SAAS | |
| VEOSTR Ltd. | BASIS SAAS | |
| VISA WORLDWIDE SINGAPORE PTE LIMITED | BASIS SAAS | |
| VISER X LIMITED | BASIS SAAS | |
| VISUAL MONITORING SOLUTIONS | BASIS SAAS | |
| VIVASOFT LIMITED | BASIS SAAS | |
| VROMOR | BASIS SAAS | |
| VS ONE Bangladesh Ltd | BASIS SAAS | |
| Valere Enterprise | BASIS SAAS | |
| Vantage Technologies Ltd. | BASIS SAAS | |
| Vasttek bangladesh | BASIS SAAS | |
| Vector360 BD | BASIS SAAS | |
| Velocity Internet | BASIS SAAS | |
| Velwire Ltd. | BASIS SAAS | |
| Vertical Innovations Limited | BASIS SAAS | |
| ViaTech Limited | BASIS SAAS | |
| Virtual Market Solution Ltd. | BASIS SAAS | |
| Visual I Ltd. | BASIS SAAS | |
| Visual Systems Limited | BASIS SAAS | |
| Vobon | BASIS SAAS | |
| Voltsmith Technology Limited | BASIS SAAS | |
| Vroom Services Limited | BASIS SAAS | |
| WAGELY BANGLADESH LIMITED | BASIS SAAS | |
| WEBB FONTAINE BANGLADESH LIMITED | BASIS SAAS | |
| WEBNS Technology Ltd. | BASIS SAAS | |
| WHITELION Technologies Limited | BASIS SAAS | |
| WINBRIDGETECH LTD | BASIS SAAS | |
| WORLD IT EXPRESS | BASIS SAAS | |
| WPDeveloper | BASIS SAAS | |
| WPXPO | BASIS SAAS | |
| WW Tech Ltd. | BASIS SAAS | |
| Waadaa Ltd. | BASIS SAAS | |
| Wafi Solutions | BASIS SAAS | |
| Walton Digi-Tech Industries Limited | BASIS SAAS | |
| Wardan Tech Ltd. | BASIS SAAS | |
| Wazdi Solutions Ltd. | BASIS SAAS | |
| WeGro Technologies Limited | BASIS SAAS | |
| WeNexus | BASIS SAAS | |
| Web Impression Technology | BASIS SAAS | |
| Web Soft BD | BASIS SAAS | |
| Webcoder-IT Institute | BASIS SAAS | |
| Weblink Communications Limited | BASIS SAAS | |
| WebnWell | BASIS SAAS | |
| Webtricker Web Design & Development Agency | BASIS SAAS | |
| Well It & Consultancy Ltd | BASIS SAAS | |
| WellDev Bangladesh Ltd. | BASIS SAAS | |
| WellsTech Solutions Ltd. | BASIS SAAS | |
| Western Management Ltd. | BASIS SAAS | |
| Wezapps Limited | BASIS SAAS | |
| White Services Technology Limited | BASIS SAAS | |
| Win Miaki Limited | BASIS SAAS | |
| Wintech Engineers Ltd. | BASIS SAAS | |
| Wintel Digital Ltd. | BASIS SAAS | |
| Wipro IT Services Bangladesh Limited | BASIS SAAS | |
| Wolast Technologies | BASIS SAAS | |
| Women in Digital | BASIS SAAS | |
| Wondersoft Solution | BASIS SAAS | |
| WorkSpace Infotech Ltd. | BASIS SAAS | |
| Workstation Communication | BASIS SAAS | |
| World of Technology | BASIS SAAS | |
| X Solutions Ltd. | BASIS SAAS | |
| XCEED Bangladesh Ltd. | BASIS SAAS | |
| XUBISOFT LTD. | BASIS SAAS | |
| Xactidea Ltd. | BASIS SAAS | |
| Xeon Technology Limited | BASIS SAAS | |
| XeonBD | BASIS SAAS | |
| XerOne IT | BASIS SAAS | |
| XpeedLab | BASIS SAAS | |
| XpeedStudio | BASIS SAAS | |
| Xpert Fintech Ltd. | BASIS SAAS | |
| XpertLab BD Ltd. | BASIS SAAS | |
| Xposure soft solution | BASIS SAAS | |
| Xpress In Town Ltd. | BASIS SAAS | |
| Xsellence Bangladesh Limited | BASIS SAAS | |
| YO TECH LIMITED | BASIS SAAS | |
| YSP Technology | BASIS SAAS | |
| YUJYO IT | BASIS SAAS | |
| YetFix Limited | BASIS SAAS | |
| Your net | BASIS SAAS | |
| Youth Opportunities Ltd. | BASIS SAAS | |
| Z Tech PLC | BASIS SAAS | |
| ZAMANIZ | BASIS SAAS | |
| ZAYAN TECHNOLOGY LIMITED | BASIS SAAS | |
| ZAYNAX HEALTH LIMITED | BASIS SAAS | |
| ZCORP SOLUTIONS | BASIS SAAS | |
| ZEN IT Services | BASIS SAAS | |
| ZIT Solutions Limited | BASIS SAAS | |
| ZaChai Ltd. | BASIS SAAS | |
| Zaag Systems Ltd. | BASIS SAAS | |
| ZamZamIT | BASIS SAAS | |
| Zantrik Limited | BASIS SAAS | |
| Zara Zaman Technology Ltd. | BASIS SAAS | |
| Zaria Engineering Limited | BASIS SAAS | |
| Zaynax Limited | BASIS SAAS | |
| Zeal International Limited | BASIS SAAS | |
| Zecodeek IT Ltd. | BASIS SAAS | |
| Zend IT Solution Limited | BASIS SAAS | |
| Zenetic Esports | BASIS SAAS | |
| Zeppelin Limited | BASIS SAAS | |
| ZeroGround | BASIS SAAS | |
| Zeteq Systems | BASIS SAAS | |
| Zia U | BASIS SAAS | |
| Zolpie Limited | BASIS SAAS | |
| Zoo Travel Technology | BASIS SAAS | |
| adorsho praniSheba Limited | BASIS SAAS | |
| bdCalling IT Ltd. | BASIS SAAS | |
| bitBirds Solutions | BASIS SAAS | |
| comptech Network System (Pvt. ) Limited | BASIS SAAS | |
| d-logiK Limited | BASIS SAAS | |
| e-Business Soft Solution Limited | BASIS SAAS | |
| eSaviour Limited | BASIS SAAS | |
| eSecureSoft Technologies Limited | BASIS SAAS | |
| eShikhon | BASIS SAAS | |
| eTech Solution Limited | BASIS SAAS | |
| epsilon solutions bd limited | BASIS SAAS | |
| graph-ai | BASIS SAAS | |
| i-Bangla Limited | BASIS SAAS | |
| i-Farmer Ltd | BASIS SAAS | |
| i-Mesh Limited | BASIS SAAS | |
| i2 Technologies Limited | BASIS SAAS | |
| iBOS Limited | BASIS SAAS | |
| iCircles USA Bangladesh Limited | BASIS SAAS | |
| iEatery Limited | BASIS SAAS | |
| iGen Solutions Limited | BASIS SAAS | |
| iHealthScreen Bangladesh Limited | BASIS SAAS | |
| iHelpBD | BASIS SAAS | |
| iKitchen Ltd. | BASIS SAAS | |
| iPro Technologies Limited | BASIS SAAS | |
| iQra Systems & Software | BASIS SAAS | |
| iQuantile | BASIS SAAS | |
| iShop Trading | BASIS SAAS | |
| iTech Unlimited | BASIS SAAS | |
| iTest Bangladesh Limited | BASIS SAAS | |
| inizio Limited | BASIS SAAS | |
| inqube Bangladesh Limited | BASIS SAAS | |
| iota Consulting BD | BASIS SAAS | |
| izoom Limited | BASIS SAAS | |
| jobdesk Ltd | BASIS SAAS | |
| lenosoft | BASIS SAAS | |
| mediMate Ltd | BASIS SAAS | |
| multibrand INFOTECH Ltd. | BASIS SAAS | |
| naztech Inc. Limited | BASIS SAAS | |
| plaas Tech Industries Ltd. | BASIS SAAS | |
| r ventures PLC | BASIS SAAS | |
| safetaka.com Ltd | BASIS SAAS | |
| shurjomukhi Solutions Limited | BASIS SAAS | |
| tecno bz | BASIS SAAS | |
| toyghor | BASIS SAAS | |
| v-Generation Limited | BASIS SAAS | |
| w3xplorers Bangladesh | BASIS SAAS | |
| zDrop Bangladesh Limited | BASIS SAAS | |
| zooFamily | BASIS SAAS | |
