# upsweep

An agent skill (`skills/upsweep/SKILL.md`, plus `connect.md` for each agent's MCP setup). It searches Upwork with the user's own filters, lists the matches and summarises what those clients ask for, through Upwork's official MCP. This file is public, so keep it publication-safe.

- **Upwork's API & MCP Terms are the hard boundary.** The skill runs on demand only, uses the user's own criteria with no ranking of its own, stores no job data, only reads, and writes drafts only. Any change must keep all of that. The clauses are cited in SKILL.md.
- **Install:** `npx skills add dave8172/upsweep`
- **Test like a new user:** use an empty folder with `.claude/skills/upsweep` symlinked to `skills/upsweep`, a fresh `UPSWEEP_DIR`, and every Upwork write tool in `--disallowedTools`. Say "upsweep", then "ok". Afterwards, check that nothing except `profile.md` was written.
