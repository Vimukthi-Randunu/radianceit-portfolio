# Radiance IT Solution: Website Blueprint (v1)

Purpose: this is the specification for redesigning radianceits.com. It states the positioning, the page structure, the approved copy, what to remove from the current site, and what must NOT be claimed. Claude Code should treat it as the source of truth and should not invent positioning, services, statistics or client results.

---

## 0. Instructions for Claude Code

1. Read this whole file and the current site files before changing anything.
2. Before editing, reply with a short plan: which files you will change, the section order, and any conflicts you found between this file and the current code. Wait for approval.
3. Work on a new git branch (e.g. `redesign-v1`). Do not touch `main` until the owner approves the preview.
4. The site is hosted on GitHub Pages, so keep it static (HTML, CSS, vanilla JS). No build step or framework unless the owner approves one.
5. Use ONLY the copy in this file. If a section needs copy that is not here, write a draft, mark it `<!-- DRAFT: needs owner approval -->`, and list it at the end of your reply.
6. Never add statistics, client names, testimonials, certifications, logos or guarantees that are not in this file.
7. Keep the existing font style. Keep the existing blue as the main accent colour.
8. The site must work and look right on a phone (check around 390px wide) and on desktop.
9. Respect `prefers-reduced-motion`: disable animation for users who ask for it.
10. After finishing, give a list of every place where content is a placeholder.

---

## 1. Positioning

**Category:** Cloud Infrastructure & DevOps Engineering.

**Identity:** an infrastructure / cloud / DevOps / production engineering company. It is NOT a software agency that also does DevOps.

**Promise:** design, automate and operate reliable production infrastructure for modern software.

**Customer takeaway (10-second test):** "These people understand what happens after the developer says the application is finished."

**Voice:** calm, precise, engineering-led. Short sentences. Outcomes and situations, not hype. No "cutting-edge", "revolutionary", "world-class", "seamless".

**Scale honesty:** Radiance is a small, technically serious company. The site must never imply a large team. Write "we" sparingly. Never write "our team of engineers".

**What stays off the sales sections:** tool names, step-by-step fixes, or "how we diagnose". Sales sections describe situations and outcomes. Depth lives only in the Engineering Systems section, where it is proof of judgment.

**AI:** do not advertise AI on the site. It is an internal delivery advantage, not what the customer buys.

---

## 2. Navigation

Logo/wordmark "Radiance" (left). Links: Services, How we work, Engineering Systems, About, Contact. Right side: primary button **Request an assessment**.

---

## 3. Page structure (in this order)

1. Hero
2. Problem and "when teams come to us"
3. Services (seven, shown as a numbered lifecycle)
4. Working alongside your engineering team
5. Who we help
6. How we work (with the maturity ladder)
7. Engineering Systems
8. Technology
9. About
10. Assessment call-to-action band
11. Contact and footer

---

## 4. Section copy

### 4.1 Hero

- Small label above headline: **Cloud Infrastructure & DevOps Engineering**
- Headline: **Cloud infrastructure built for reliable production.**
- Subline: **We design, automate and operate the infrastructure behind modern software.**
- Supporting sentence: For agencies, product teams and growing businesses that need dependable production without building an infrastructure team.
- Primary button: **Discuss an infrastructure project** (scrolls to Contact)
- Secondary button: **Explore our services** (scrolls to Services)
- Visual: a clean architecture diagram (see section 6). No stock photos, no stats bar.

### 4.2 Problem and "when teams come to us" (one merged section)

- Headline: **Your application is only as reliable as the infrastructure running it.**
- Subline: We help teams move from "the application works" to "the application is ready for production."
- Lead-in: **When teams come to us**
  - Your cloud bill is growing faster than your usage.
  - A customer or auditor is asking about security, data location or recovery, and you can't answer with confidence.
  - Releases feel risky, and outages take too long to explain.
  - The platform you started on no longer fits what you're building.
  - The person who set up production has moved on, or is stretched thin.
  - You're about to scale and aren't sure what will break first.
- Closing line: If one of these sounds familiar, start with an infrastructure assessment.
- Button: **Request an assessment**

Rule: do not add tool names or fixes to this section.

### 4.3 Services (seven, numbered, in this order)

Section headline: **From first assessment to ongoing operations.**
Section subline: Seven services that follow the life of a production system.

Display as a vertical or connected numbered path (01 to 07), not a grid of unrelated cards. Each item: number, title, one-line outcome, 4 to 5 bullets, and (where available) a "See it in practice" link to the matching Engineering System.

**01 Infrastructure Assessment**
Outcome: Find out what's wrong before it costs you.
A focused review of your existing cloud and deployment environment, delivered as a written report.
- Reliability and failure risks
- Security configuration
- Deployment process
- Backup and recovery readiness
- Monitoring gaps
- Cloud cost
Deliverable line: Findings, severity, business impact and a prioritised roadmap.

**02 Cloud Architecture & Infrastructure**
Outcome: Design the foundation before you deploy.
- AWS environment design
- Private networking and isolation
- Access control (IAM)
- Compute, storage and databases
- DNS and TLS
- Separate staging and production environments

**03 Cloud Migration**
Outcome: Move from a starter setup to infrastructure you control.
- From starter hosting platforms to a structured AWS environment
- From single-server setups to separate staging and production
- Planned cutover with a rollback path
- Documentation of what was moved and how
Link: "See it in practice" to Operationalizing an Existing Application.

**04 DevOps & Deployment Automation**
Outcome: Turn deployment into a repeatable engineering process.
- Automated testing and deployment pipelines
- Containerised applications
- Staging and production with approval gates
- Health checks and automatic rollback
- Secrets kept out of code and images

**05 Reliability & Observability**
Outcome: Know what is happening in production.
- Metrics and dashboards
- Alerting on failures and error rates
- Health checks
- Service-level visibility across components

**06 Infrastructure Security**
Outcome: Secure the infrastructure your application depends on.
- Least-privilege access
- Network isolation between services
- Secrets management
- TLS everywhere
- No long-lived credentials in CI/CD

**07 Managed Infrastructure**
Outcome: Keep your production infrastructure running.
For teams that don't want to build an infrastructure function of their own. Defined monthly scope.
- Monitoring review
- Deployment support
- Maintenance and updates
- Cost reviews
- Incident assistance during agreed support hours

Footnote under the section (small text): We can also build custom applications and APIs when infrastructure and application engineering need to be delivered together. (This is the ONLY mention of software development. It is not a service card.)

### 4.4 Working alongside your engineering team

- Headline: **Work with your existing engineering team.**
- Text: Radiance doesn't replace your developers. We work alongside them on the infrastructure layer (design, automation and operations), so your engineers can stay focused on the product.
- No button; the page-level CTAs are enough.

### 4.5 Who we help (four cards, in this order)

1. **Software agencies.** An infrastructure partner for client projects that need cloud deployment, CI/CD, production environments or ongoing support.
2. **Product and SaaS teams.** Infrastructure and reliability support as your product moves from development into production and begins to scale.
3. **Founders and teams building with AI.** Applications built quickly with AI tools often work in a demo and strain under real users, real data and real security expectations. We take them from working to production-ready.
4. **Growing businesses.** Cloud infrastructure without the cost of a full internal infrastructure team.

### 4.6 How we work

- Headline: **A process, not a one-off setup.**
- Steps (numbered, horizontal on desktop, vertical on mobile):
  1. **Understand.** The application, the business requirements, the current infrastructure.
  2. **Assess.** Risks, constraints and opportunities.
  3. **Design.** The target architecture and an implementation plan.
  4. **Build.** Infrastructure, automation and operational tooling.
  5. **Validate.** Deployment, failure recovery, security and operational behaviour.
  6. **Operate.** Ongoing maintenance, monitoring and support where required.
- Line under the steps: Implementation is one step of six.

**Maturity ladder (small, directly under the steps):**
- Label: **Where is your infrastructure today?**
- Four steps shown as a rising ladder: **Working → Production-ready → Reliable → Optimised**
- One short line under each:
  - Working: the application runs.
  - Production-ready: deployment, security, backups and monitoring are in place.
  - Reliable: failures are visible, recoverable and rehearsed.
  - Optimised: cost, performance and operations are continuously improved.
- Closing line: An assessment tells you which step you are on and what it takes to reach the next one.
- Do NOT add a fifth "Platform / Kubernetes" step yet.

### 4.7 Engineering Systems

- Headline: **Engineering systems.**
- Subline: Reference systems built and documented by Radiance to demonstrate how we design and operate production infrastructure. Each one is public on GitHub.
- Each card uses this layout: Name, **Challenge**, **Approach**, **Infrastructure** (tags), **Outcome**, GitHub link.
- Outcomes describe capabilities demonstrated, never client results.
- Start from the existing project text on the current site (webhook delivery system, production waitlist API, operationalizing an existing application, staging and production separation, multi-container system, Docker-based CI/CD pipeline). Keep the technical depth: it is the proof. Reformat into the layout above.
- "Show more projects" stays.
- Do not call these "client work", "customers" or "case studies". A separate "Client results" section is added only when real client work exists.

### 4.8 Technology

Group, don't use a logo wall:
- Cloud: AWS (VPC, IAM, EC2, Route 53, Parameter Store)
- Infrastructure: Docker, Docker Compose, Linux, Nginx
- Delivery: GitHub Actions, CI/CD
- Observability: Prometheus, Grafana
- Data: PostgreSQL, Redis

Terraform and Kubernetes: **show only if the owner confirms real project use** (see section 8). Default: leave them out.

### 4.9 About

- Headline: **Built from first principles.**
- Text: keep the current about text with these changes: it is written in the first person plural sparingly; remove "scalable" as a promise; do not describe a team.
- Name and title: W.K.V.P Randunu, DevOps Engineer. Photo optional (owner decides).

### 4.10 Assessment call-to-action band

- Headline: **Not sure what's wrong with your infrastructure?**
- Subline: Start with an infrastructure assessment.
- Six short items: Security risks · Reliability gaps · Deployment problems · Cloud cost issues · Backup and recovery weaknesses · Operational blind spots
- Button: **Request an assessment** (opens email to wkvp.randunu@gmail.com with subject "Infrastructure assessment request")

### 4.11 Contact and footer

- Headline: **Let's talk about your infrastructure.**
- Text: Tell us what you're running and what's worrying you. We'll reply with an honest view of whether and how we can help.
- Email: wkvp.randunu@gmail.com (keep the existing address)
- Keep the X and LinkedIn links.
- Footer: © 2026 Radiance IT Solution · W.K.V.P Randunu · radianceits.com

---

## 5. Remove or correct from the current site

- **Remove the stats bar** ("9+ Production-ready systems built / 0 Manual deploys needed / 100% Automated rollback coverage"). It reads as client results and will damage trust when visitors find out these are reference projects.
- Replace the old hero label "DevOps & Deployment Automation" and the old headline.
- Change "Production-ready systems built" language anywhere: use "reference systems" or "engineering systems".
- Remove "Ready to automate your deployments?" from Contact.
- Remove any claim that implies customers, a team, uptime guarantees or response times.
- Remove "scalable" as a promise in the About text.
- Do not use any specific platform comparisons (limits of Vercel, Railway, Render etc.) anywhere on the site.

---

## 6. Visual direction

- Style: small, technically serious engineering company. Not a corporate consultancy, not a creative agency.
- Base: dark, but layered. Use two or three surface shades (page, raised surface, card) instead of one flat black. Subtle border lines.
- Accent: keep the current blue; add one lighter tint and one muted tone for secondary text. Use the accent sparingly for buttons, links, active states and diagram lines.
- Background: a very subtle grid or dot pattern in the hero only.
- Hero visual: an architecture diagram (users → load balancer/Nginx → application → database, with a monitoring path and a CI/CD path). Animate gently: flowing dashes along the connections. Respect reduced-motion.
- Services section: a connected numbered path with a thin line linking 01 to 07.
- Buttons: clear primary (filled accent) and secondary (outlined) styles, visible hover and focus states, a small transition.
- Cards: soft border, slight lift on hover.
- Code or terminal snippets: sparingly, only in Engineering Systems if at all.
- Do NOT use: stock photos, laptop photos, abstract blobs, AI-generated imagery, giant code screenshots, customer-logo walls.
- Accessibility: contrast must pass WCAG AA, visible keyboard focus, meaningful alt text and headings in order.

---

## 7. DO NOT CLAIM (yet)

- Clients, customers, testimonials, case studies, client logos
- Any statistic that cannot be verified from the repos
- 24/7 coverage, response-time guarantees, uptime or SLA guarantees
- On-premise to cloud migration, legacy modernisation, multi-cloud
- Kubernetes or platform engineering as a service (listed as a future direction only, if at all)
- SRE, tracing, SLOs, error budgets, automated remediation
- Cost optimisation as a headline service (it appears only as an item inside Assessment and Managed Infrastructure)
- Compliance certifications or frameworks (SOC 2, ISO 27001, HIPAA)
- Any comparison claiming a hosting platform "cannot" do something
- "AI-powered" or any mention of AI in delivery

---

## 8. Open items for the owner to confirm before launch

1. **Assessment offer:** what exactly is included, how long it takes, and the price (or "from" price). The button appears on every page, so this must exist before the site goes live. Copy on the site stays price-free until decided.
2. **Terraform and Kubernetes:** list them under Technology only if used in a real project. Otherwise leave them out.
3. **Backups and recovery:** the Assessment and Managed sections mention them. Confirm you can demonstrate backup and restore (a short documented test is enough).
4. **Migration proof:** build and document one small migration (an app on a starter platform moved to a structured AWS setup, with cutover and rollback notes) and add it as an Engineering System.
5. **Support hours** for Managed Infrastructure: decide the wording (for example "business hours, Sri Lanka time").
6. **Project count:** confirm the number of public reference systems before stating any number.
7. **About photo:** include or not.

---

## 9. Change log

- v1: initial blueprint. Seven services, migration as its own service (position 03), hero lines accepted, "Founders and teams building with AI" wording accepted, maturity ladder tied to the assessment.
