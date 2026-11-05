# career-kit

Three Claude skills for job hunting, for any profession or industry. They ask about your field first and adapt their questions, CV conventions and interview prep to it. Used in order:

| Skill | What it does | Output |
|-------|--------------|--------|
| `grill-me-for-my-cv` | Interviews you to build or update your master CV | `master-cv.md` |
| `gen-me-a-cv` | Tailors a CV (and optional cover letter) to one job ad | CV per job |
| `get-me-that-job` | Research, interview prep and a day-by-day plan for one job | Prep plan per job |

```
grill-me-for-my-cv  ->  master-cv.md  ->  gen-me-a-cv  ->  get-me-that-job
   (once, update            (the one          (per job)       (per job)
    as you go)             source of truth)
```

## Using them

**Claude Code:** clone this repo and run `claude` inside it. Skills in `.claude/skills/` are picked up automatically for this project. To have them in every project, copy the folders into `~/.claude/skills/`.

**Claude app (claude.ai, desktop, mobile):** zip each skill folder (the folder itself, with `SKILL.md` inside) and upload it in the Skills section of your settings. Uploaded skills belong to your account only.

## Other AI tools

These follow the open Agent Skills (`SKILL.md`) format, so they also work in tools such as OpenAI Codex CLI (`.agents/skills/`), GitHub Copilot (reads `.claude/skills/` as-is) and Gemini CLI. In chat apps without skills support, paste a `SKILL.md` in as instructions.

## Privacy

The skills themselves contain no personal data, so this repo can be public.
Your actual CV data must never be committed. Keep it in `data/`, which is git-ignored:

```
data/
  master-cv.md
  jobs/
    {company}-{role}/
      ad.md
      cv.md
      prep.md
```
