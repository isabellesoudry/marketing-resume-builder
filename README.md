# Marketing Resume Builder — Claude Skill

A custom skill for [Claude](https://claude.ai) that automatically tailors your CV to any job description — matching language, emphasizing the right experience, and outputting a formatted document ready to open in Google Docs or Word.

Built by a growth marketing professional to solve a real problem: applying to 20+ roles across fintech, retail, and growth companies requires a different CV emphasis each time. This skill makes that process fast, consistent, and high-quality.

---

## What it does

1. **Reads the job description** — extracts key language, required skills, tools, and metrics the role cares about
2. **Runs a gap analysis** — compares the job requirements against your master CV and identifies what to surface, reframe, or cut
3. **Rewrites your CV** — mirrors the job's language, leads with the most relevant metrics, and applies lifecycle marketing best practices throughout
4. **Outputs a formatted .docx file** — named `[Your Name]_[Company]_[Role].docx`, ready to open and make final edits

---

## Folder structure

```
marketing-resume-builder/
├── SKILL.md                          ← skill instructions (the brain)
├── context/
│   ├── 1-all-merged-cv-bank.md       ← your master CV with all experience
│   ├── 2-past-projects-bank.md       ← supplementary project details
│   └── 3-formatted-cv-template-DO-NOT-UPDATE.md  ← formatting reference
└── LICENSE
```

---

## How to use it

### Step 1 — Add your own content

Replace the placeholder files in the `context/` folder with your own:

- **`1-all-merged-cv-bank.md`** — your master CV containing every role, every bullet point variation, and every metric across your career. The more complete, the better. See the placeholder for the recommended structure.
- **`2-past-projects-bank.md`** — a log of supplementary achievements, projects, and results that don't fit neatly into a CV but are useful context. One entry per project, with dates and impact.
- **`3-formatted-cv-template-DO-NOT-UPDATE.md`** — a markdown version of a CV you like the look of. The skill uses this as a formatting reference. Replace with your own preferred layout — but don't change the filename.

### Step 2 — Install the skill in Claude

1. Zip the `marketing-resume-builder` folder
2. Go to [claude.ai](https://claude.ai) → Settings → Customize → Skills
3. Click **Upload skill** and select the zip file
4. Toggle the skill on

### Step 3 — Use it

Start a new conversation in Claude and say:

> "Use my marketing-resume-builder skill. Here's a job I'm applying to: [paste job description or URL]. Tailor my CV for this role."

Claude will read your master CV, analyse the job, and produce a tailored `.docx` file named after the company and role.

---

## Writing principles baked in

Every CV this skill produces follows these rules:

- **Metric-first bullets** — every point leads with a hard number or percentage
- **Language mirroring** — uses the exact terminology from the job description for ATS and human readers
- **Strong action verbs** — Architected, Spearheaded, Engineered, Scaled
- **Concise** — no bullet longer than two lines; most impressive data point comes first
- **Never fabricates** — only reframes real experience in stronger language

---
## Quick start for non-technical users

No coding required. If you can use Google Docs, you can use this skill.

---

### The problem this solves

If you've ever applied to multiple jobs and ended up with 10, 15, or 20 slightly different versions of your CV — each one tweaked for a different company or role — this skill is for you.

Instead of maintaining dozens of versions, you create one master document with *everything* in it. Then every time you apply somewhere new, Claude reads the job description, picks the most relevant parts of your experience, rewrites the bullets in the company's language, and produces a tailored CV ready to open in Google Docs.

---

### Step 1 — Copy the master CV template into Google Docs

👉 **[Click here to open the Master CV Template](#)** *(https://docs.google.com/document/d/1vPrf6UYjHTMNTXAnbkXQ2h7PuOaA-KEcsM6J1eCk1pg/edit?tab=t.0)*

- Go to **File → Make a copy** to get your own editable version
- Fill in every section with your experience — include every job, every metric, every tool you've used
- If you have multiple versions of the same CV, go through each one and copy the bullet points into the relevant job section. More content = better tailored CVs
- When done: **File → Download → Plain Text (.txt)**
- Find the downloaded file on your computer and rename it from `master-cv.txt` to `master-cv.md`

---

### Step 2 — Download the skill

- Click the green **Code** button at the top of this page → **Download ZIP**
- Unzip the folder on your computer
- Replace the file `context/1-all-merged-cv-bank.md` with your own `master-cv.md`

---

### Step 3 — Upload the skill to Claude

- Go to [claude.ai](https://claude.ai) and sign in
- Click your profile icon → **Settings** → **Customize** → **Skills**
- Click **Upload skill** → select the zipped skill folder
- Toggle the skill **on**

---

### Step 4 — Tailor your CV

Start a new chat in Claude and paste this:

> "Use my marketing-resume-builder skill. Here's a job I'm applying to: [paste the job description or URL]. Tailor my CV for this role."

Claude will read your master CV, analyse the job description, and produce a tailored CV as a Word document named after the company and role.

---

### Tips for getting the best results

- **Include everything in your master CV** — don't edit yourself. The AI decides what to cut, not you.
- **Paste the full job description** — the more detail Claude has, the better the language matching
- **Review the output** — the AI won't fabricate anything, but you should always read through and make sure the framing feels accurate before sending
- **Update your master CV over time** — add new projects, metrics, and achievements as you go


## Industry framing

The master CV template includes framing notes for four role types:

| Role type | Examples |
|-----------|----------|
| Fintech / Payments | Stripe, Robinhood, Ramp, Cash App |
| Luxury / Retail | Reformation, Versace, Zappos, AMEX |
| Growth / Platform | Meta, TikTok, Pinterest, DoorDash |
| AI-forward | xAI, Ramp AI, Blend |

---

## Requirements

- A [Claude.ai](https://claude.ai) account (free, Pro, or Team)
- Code execution enabled in Claude settings (required for .docx output)

---

## License

MIT — use it, adapt it, share it.
