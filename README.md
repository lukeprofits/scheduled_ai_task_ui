# scheduled_ai_task_ui

Schedule recurring Grok Build & Claude Code tasks in a few clicks.

<br>

<div align="center">

[![Open the app](https://img.shields.io/badge/▶_Open_the_app-6366f1?style=for-the-badge&logoColor=white)](https://lukeprofits.github.io/scheduled_ai_task_ui/)

</div>

<br>

A single-file web UI that turns a plain-English task into a ready-to-paste
cron command — no cron syntax, no scripting.

## Why

Scheduling a recurring AI agent normally means hand-writing crontab lines,
escaping quotes, fixing cron's minimal `PATH`, and wiring up logs. This does
all of that: type what you want, pick a schedule, copy, paste in your terminal.

## What it does

- Pick a frequency (daily, weekdays, weekly, hourly) and describe the task.
- Generates the full one-liner: cron expression + `bash -lc` wrapper + `PATH`
  fix + dated log file in `~/agent-logs/` (or `<working-dir>/logs/`).
- For Claude Code, choose a work-safe tool allowlist (read / write / bash /
  web) — no permission bypass.
- Re-pasting updates the same task instead of duplicating it.

Runs entirely in the browser — nothing leaves your machine. Install the agent
CLI (`claude` or `grok`) and sign in once first; this tool only schedules.

## License

MIT
