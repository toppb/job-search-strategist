# Job Search Strategist

A Claude skill that treats job searching as a research project — not a resume blast.

Instead of spray-and-pray applications, this skill runs a structured pipeline for each opportunity: analyze what the role *actually* needs, research the company and team, tailor every application artifact, track your pipeline, and prepare for interviews with concrete stories mapped to the role's requirements.

Works for any profession — designers, engineers, PMs, marketers, or anyone doing a targeted professional job search. The method is the same; the heuristics adapt to your domain.

---

## What it does

| Phase | What happens |
|-------|-------------|
| **0. Getting to Know You** | Lightweight intake on first use, then learns more about you with every application |
| **1. JD Analysis** | Reads between the lines of job descriptions — separating real requirements from wish lists |
| **2. Fit Assessment** | Honest evaluation of fit: Strong, Decent, Stretch, or Poor — with specifics, not encouragement |
| **3. Company Research** | Deep dive on product, team, hiring manager, culture, compensation, and red flags |
| **4. Application Tailoring** | Cover letters, referral notes, form responses, and experience summaries — all mapped to the specific role |
| **5. Tracking** | Structured application pipeline with status tracking and deduplication discipline |
| **6. Interview Prep** | Story mapping, behavioral question prep, portfolio/experience walkthrough rehearsal |
| **7. Follow-up** | Post-application and post-interview follow-up, negotiation framing |

The skill gets sharper over time. Each application teaches it more about your experience, your stories, your voice, and what positioning works — so the fifth application is significantly better than the first.

---

## Install

### Claude.ai

Upload the `.skill` file from [`dist/`](dist/) to your Claude.ai project under **Settings → Skills**.

### Claude Code — drop-in

```bash
cp -R job-search-strategist ~/.claude/skills/
```

### Claude Code — from repo

```bash
git clone https://github.com/toppb/job-search-strategist.git
cp -R job-search-strategist/job-search-strategist ~/.claude/skills/
```

---

## Usage

Once installed, the skill triggers automatically when you:

- Share a job posting URL or paste a JD
- Ask Claude to analyze a role, write a cover letter, or prep for an interview
- Say things like "help me apply", "is this a good fit", or "I have an interview at [company]"

**First time:** Claude will ask a few questions to understand your background — target roles, experience level, a couple of lead projects, and any known gaps. This takes a few minutes and makes everything downstream specific instead of generic.

**After that:** Just drop a job posting link and the skill handles the rest — analysis, fit assessment, tailoring, and prep. Each conversation builds on what Claude has learned about you.

### Example workflow

```
You:    "Here's a role I'm interested in: [URL]"
Claude: [Fetches JD, analyzes requirements, assesses fit, flags concerns]

You:    "Write me a cover letter"
Claude: [Drafts a letter leading with your strongest parallel to the role]

You:    "I got an interview — help me prep"
Claude: [Maps your experience to likely questions, builds story reference table]
```

---

## Tips

- **One conversation per opportunity** keeps all context (research, materials, prep) in one place.
- **Be honest about gaps.** The skill works best when it knows your real concerns — it'll help you address them, not hide them.
- **Correct it.** If Claude gets a detail wrong about your experience, say so. Corrections make future applications more accurate.
- **Use it for practice too.** General conversations for behavioral question practice or portfolio walkthrough rehearsal work well outside of specific opportunities.

---

## Origin

This skill was extracted from a real job search — dozens of applications across multiple industries and role types. The pipeline, heuristics, and tailoring patterns were refined through actual use, not theoretical design. Then generalized to work for any field.

---

## License

MIT — see [LICENSE](LICENSE).
