# Marketing Resume Builder — Claude Skill

A custom skill for [Claude](https://claude.ai) that automatically tailors your CV to any job description — matching language, emphasizing the right experience, and outputting a formatted document ready to open in Google Docs or Word.

Built by a growth marketing professional to solve a real problem: applying to 20+ roles across fintech, retail, and growth companies requires a different CV emphasis each time. This skill makes that process fast, consistent, and high-quality.

---

## What it does

1. **Reads the job description** — extracts key language, required skills, tools, and metrics the role cares about
2. **Runs a gap analysis** — compares the job requirements against your master CV and identifies what to surface, reframe, or cut
3. **Rewrites your CV** — mirrors the job's language, leads with the most relevant metrics, and applies best practices throughout
4. **Outputs a formatted .docx file** — named `[Your Name]_[Company]_[Role].docx`, ready to open and make final edits

---

## Writing principles baked in

- **Metric-first bullets** — every point leads with a hard number or percentage
- **Language mirroring** — uses the exact terminology from the job description for ATS and human readers
- **Strong action verbs** — Architected, Spearheaded, Engineered, Scaled
- **Concise** — no bullet longer than two lines; most impressive data point comes first
- **Never fabricates** — only reframes real experience in stronger language

---

## Folder structure

```
marketing-resume-builder/
├── SKILL.md                                        ← skill instructions (the brain)
├── context/
│   ├── 1-all-merged-cv-bank.md                     ← your master CV with all experience
│   ├── 2-past-projects-bank.md                     ← supplementary project details
│   └── 3-formatted-cv-template-DO-NOT-UPDATE.md    ← formatting reference
└── LICENSE
```

---

## Quick start — no coding required

If you can use Google Docs, you can use this skill.

### The problem this solves

If you've ever applied to multiple jobs and ended up with 10, 15, or 20 slightly different versions of your CV — each one tweaked for a different company or role — this skill is for you.

Instead of maintaining dozens of versions, you create one master document with *everything* in it. Every time you apply somewhere new, Claude reads the job description, picks the most relevant parts of your experience, rewrites the bullets in the company's language, and produces a tailored CV ready to open in Google Docs.

---

### Step 1 — Build your master CV in Google Docs

👉 **[Click here to open the Master CV Template](https://docs.google.com/document/d/1vPrf6UYjHTMNTXAnbkXQ2h7PuOaA-KEcsM6J1eCk1pg/edit?tab=t.0)**

- Go to **File → Make a copy** to get your own editable version
- Fill in every section with your experience — every job, every metric, every tool you've used
- If you have multiple CV versions, copy the bullet points from each one into the relevant job section. More content = better tailored CVs
- When done: **File → Download → Plain Text (.txt)**
- Rename the downloaded file from `master-cv.txt` to `master-cv.md`

### Step 2 — Download and set up the skill

- Click the green **Code** button at the top of this page → **Download ZIP**
- Unzip the folder
- Replace `context/1-all-merged-cv-bank.md` with your own `master-cv.md`
- Re-zip the folder

### Step 3 — Upload to Claude

- Go to [claude.ai](https://claude.ai) → profile icon → **Settings → Customize → Skills**
- Click **Upload skill** → select your zip file
- Toggle the skill **on**

### Step 4 — Tailor your CV

Start a new chat and say:

> "Use my marketing-resume-builder skill. Here's a job I'm applying to: [paste job description or URL]. Tailor my CV for this role."

Claude will produce a `.docx` file named after the company and role, ready to open and make final edits.

---

### Tips

- **Include everything in your master CV** — don't edit yourself. The AI decides what to cut, not you
- **Paste the full job description** — the more detail Claude has, the better the language matching
- **Always review the output** — the AI won't fabricate anything, but read through before sending
- **Update your master CV over time** — add new projects, metrics, and achievements as you grow

---

## Requirements

- A [Claude.ai](https://claude.ai) account (free, Pro, or Team)
- Code execution enabled in Claude settings (required for .docx output)

---

## License

MIT — use it, adapt it, share it.
