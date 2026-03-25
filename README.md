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
