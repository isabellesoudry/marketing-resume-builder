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

## The problem this solves

If you've ever applied to multiple jobs and ended up with 10, 15, or 20 slightly different versions of your CV — each one tweaked for a different company or role — this skill is for you. Instead of maintaining dozens of versions, you create one master document with *everything* in it. Every time you apply somewhere new, Claude reads the job description, picks the most relevant parts of your experience, rewrites the bullets in the company's language, and produces a tailored CV ready to open in Google Docs.

---

## IF YOU HAVE NO IDEA HOW TO USE THIS AND DON'T EVEN KNOW WHAT GITHUB IS, READ THESE INSTRUCTIONS

### Step 1 — Download this skill to your computer
- Click the green **Code** button at the top of this page → **Download ZIP**

### Step 2 — Create your CV bank
You have two options depending on how much setup you want:

  **Option 1 (quickest/easiest):** Skip this step entirely (don't create a CV bank). In Step 3, just paste your most recent CV text directly into the chat when you use the skill and ask it to update based on the JD.

  **Option 2 (set it up once, never paste your CV again):**
- 👉 **[Open the all experience template](https://docs.google.com/document/d/1vPrf6UYjHTMNTXAnbkXQ2h7PuOaA-KEcsM6J1eCk1pg/edit?tab=t.0)** → File → Make a copy
- Fill in every job, metric, and tool across your whole career. If you have multiple CV versions, copy bullet points from all of them into the relevant sections. More content = better output.
- When done: **File → Download → Plain Text (.txt)**
- Rename the file to `all-experience.md`
- Unzip the "marketing-resume-builder-public" folder you donwloaded in step 1 → drop your file into `context/` folder → re-zip (select the entire "marketing-resume-builder-public" folder, right click, and select compress)

### Step 3 — Install the skill in Claude
- Go to [claude.ai](https://claude.ai) → profile icon → **Settings → Customize → Skills**
- Click **Upload skill** → select the ZIP file you either downloaded in step 1 or just compressed in step 2 → toggle the skill **on**


### Step 3 — Tailor your CV
Start a new chat in Claude and say:

> "Use my marketing-resume-builder-public skill. Here's a job I'm applying to: [paste job description or URL]. Tailor my CV for this role."

Claude will produce a `.docx` file named after the company and role, ready to open and make final edits.

---

## Tips
- **Include everything in your all-experience doc** — don't cut it down yourself. The AI decides what to cut, not you
- **Paste the full job description** — the more detail Claude has, the better the language matching
- **Always review the output** — the AI won't fabricate anything, but read through before sending

---

## Requirements
- A [Claude.ai](https://claude.ai) account (free, Pro, or Team)
- Code execution enabled in Claude settings (required for .docx output)

---

## License
MIT — use it, adapt it, share it.
