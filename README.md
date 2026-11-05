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

## How to install

### Claude app (claude.ai, desktop, mobile)

1. Go to the [latest release](https://github.com/Kurt-van-Reenen/career-kit/releases/latest) and download the three zip files:
   `grill-me-for-my-cv.zip`, `gen-me-a-cv.zip`, `get-me-that-job.zip`
2. In Claude, open the Skills section of your settings and upload each zip. Don't unzip them first.
3. Start a new chat and say **"grill me for my CV"**.

Uploaded skills belong to your account only.

### Claude Code

Install all three as a plugin with one command:

```
/plugin install career-kit --marketplace Kurt-van-Reenen/career-kit
```

On older versions of Claude Code, use two steps:

```
/plugin marketplace add Kurt-van-Reenen/career-kit
/plugin install career-kit@career-kit
```

To get updates later: `/plugin marketplace update career-kit`.

### Other AI tools

The skills follow the open Agent Skills (`SKILL.md`) format, so they work in other tools too. Copy the folders from `skills/` into the tool's skills folder, for example `.agents/skills/` for OpenAI Codex CLI or `.github/skills/` for GitHub Copilot. In chat apps without skills support, paste a `SKILL.md` in as instructions.

## Repo layout

```
.claude-plugin/
  plugin.json          plugin details
  marketplace.json     lets Claude Code install from this repo
skills/
  grill-me-for-my-cv/SKILL.md
  gen-me-a-cv/SKILL.md
  get-me-that-job/SKILL.md
```

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

## License

MIT. Use, change and share these freely.
