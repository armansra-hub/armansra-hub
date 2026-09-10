## Arman Sra

Account executive who builds his own tools. I sell NetSuite; when the software I need for
the job doesn't exist, or exists badly, I build it. The repos below are **separate,
unrelated projects** — different problems, different stacks, different years. They have
nothing in common except that each one started with me being annoyed at something.

Mostly TypeScript / Next.js / Postgres, with Claude wired in where a model genuinely beats
a rule, and deterministic code everywhere else.

---

### 🛰️ [Stanley](https://github.com/armansra-hub/stanley) — territory intelligence for a solo AE
**Next.js · Supabase · Claude · scheduled agents** — [live](https://jarvis-arman44.vercel.app)

The largest of these. Stanley watches an entire NetSuite sales territory for ERP-readiness
trigger events and ranks the "call these now" worklist, so prospecting stops being a
guessing game about *timing*. Three modules on one app: **Headhunter** (TAM monitoring,
signal scoring with decay, CSV + NetSuite saved-search export), **Missions** (tasks and an
Outlook-calendar agent you talk to), and **Kill List** (a manual pipeline Kanban that the
AI is explicitly forbidden from inventing data in).

Pure monitoring, not discovery — it never scrapes a lead out of thin air. Every signal in
the roster was verified against the real base, and the ones that didn't predict anything
were deleted rather than kept for the demo.

---

### 📋 [Job-Search Accountability CRM](https://github.com/armansra-hub/job-search-crm) — a CRM that nags you
**Next.js · Supabase · Google Apps Script · Claude**

Job searches fail on follow-through, not tracking. So the tasks-with-deadlines are the
heartbeat and the CRM exists to give them something to point at. Applying auto-creates the
48-hour outreach task; a Gmail watcher on Google's infrastructure classifies replies every
15 minutes and moves the stage without you opening the app; an 8am digest surfaces what's
overdue.

Two decisions worth reading the code for: voice commands return a **structured diff you
confirm** before anything is written (speech recognition mishears company names, and a
voice UI that silently mutates data is worse than none), and the always-on half runs in
Apps Script precisely because a web page can't watch Gmail or fire at 8am.

---

### 🏔️ [Scroll-Driven Case Presentations](https://github.com/armansra-hub/scroll-case-presentations) — sales cases as websites
**Three.js · vanilla JS · single-file HTML** — [live demos](https://armansra-hub.github.io/scroll-case-presentations/)

Two live sales-case interviews where I built the presentation instead of decking it. One is
a 3D alpine descent — the deal from approval email to first draw, each analytical beat a
station you stop at on the way down. The other is an 8-bit pixel RPG climb where the
prospect's decision points are literal forks in the trail and the route changes with what
you choose.

Every word of case copy is verbatim from the source brief, and a Python checker in the repo
proves it on demand rather than on trust. No build step, no framework — each is one
self-contained HTML file that opens off a laptop in a room with bad wifi.

---

📫 armansra@gmail.com
