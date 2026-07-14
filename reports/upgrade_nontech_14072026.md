# VidyaSetu Non-Tech Repo Upgrade Report — 14 July 2026

## Repo Understanding

VidyaSetu is a personal, single-maintainer content repo (not code): a playbook-in-progress for
helping mid-career professionals, homemakers, retirees, and others transition into academic
teaching in India. It contains a vision README, a working ToDos/tracking log, a 4-stakeholder
Playbook (students, colleges, professionals, facilitators), reference notes, and a personal-project
"Admin" folder (surveys, assessment notes, insights). At review time it was an early-stage, honest
work-in-progress rather than a polished public resource — this review focused on making that stage
easy to trust and navigate for a first-time visitor, without touching the substance of the content.

## Completed This Session

### Critical Issues
- Cleaned up em dashes in `Admin/DoNew_VidyaSetu_Insights.md` (line 28) and `References/Notes.md` (line 15).
- Resolved third-party redistribution risk: moved 9 copyrighted academic PDFs and a scanned
  newspaper clipping from `References/` to a sibling folder outside the repo
  (`VidyaSetu_removed_thirdparty/References/`); moved a third-party "DoNew" framework screenshot
  from `Admin/` to `VidyaSetu_removed_thirdparty/Admin/`. `References/Notes.md` (which already had
  proper citation links to several of these sources) was left in place. The now-broken image
  reference in `Admin/DoNew_VidyaSetu_NinjaSkills.md` was replaced with a text description.

### Structural Changes
- Added `LaTeX/README.md` clarifying that folder is a personal presentation-template toolkit,
  unrelated to the VidyaSetu playbook content.
- Linked `References/Notes.md` from the root README under "Information Gathering".
- Rendered `Admin/VidyaSetuMindMap.pdf` to `Admin/VidyaSetuMindMap.png` (spot-checked for rendering
  defects) and embedded it in the README under a new "Project at a Glance" heading.
- Extracted the inline "How to Contribute" section from `Playbook/Playbook.md` into a standalone
  `CONTRIBUTING.md` at the repo root.

### Clutter & Redundancy
- Removed commented-out `-- OLD --` draft blocks from all four Playbook files (students, colleges,
  professionals, facilitators) — each file's current version was confirmed final first.
- Removed the commented-out "Appendix: Development Plan" from `ToDos.md`.
- Trimmed `LaTeX/about_me.tex` down to the active bio slide, removing ~90% of the file that was
  commented-out, unrelated old NLP/ML talking points and references to a defunct venture.

### Improvement Suggestions & Documentation Gaps
- Added License, Last Commit, and Contributors badges to the README (dynamic shields.io badges).
- Added a one-line "who this is for" summary near the top of the README.
- Added `CODE_OF_CONDUCT.md` (standard Contributor Covenant v2.1).
- Added `.github/ISSUE_TEMPLATE/content_suggestion.md` and `.github/PULL_REQUEST_TEMPLATE.md`
  (plain markdown templates — no automation or workflows).
- Added a root-level `CONTENTS.md` catalog indexing every folder (Root, Playbook/, Admin/,
  References/, LaTeX/); every link in it was verified programmatically to resolve. Linked from the
  README.

No GitHub Actions or CI/CD were added or proposed at any point, per standing preference.

## Still Open — Tracked as a Checklist

### Manual (maintainer-only, cannot be done by an agent)
- [ ] Set the GitHub repo Description and Topics: go to `https://github.com/yogeshhk/VidyaSetu`,
      click the gear icon next to "About" (top-right of the repo page), add a short description
      (e.g. "A playbook for professionals transitioning into academic teaching careers in India")
      and topics (e.g. `education`, `career-transition`, `teaching`, `india`, `playbook`).
- [ ] Optionally set a social preview image via Settings → General → Social preview.

### Personal & Sensitive Information — decided (2026-07-14, follow-up session)
- [x] Phone number in `LaTeX/about_me.tex` — turned out to already be resolved: it was inside the
      commented-out block removed during the earlier clutter cleanup.
- [x] Third-party names/relations table (one entry labeled "(son)") in a commented-out block in
      `Admin/DoNew_VidyaSetu_Insights.md` — deleted entirely per maintainer decision (it was
      outdated, mostly "Awaiting response" tracking data).
- [x] Maintainer's own psychometric self-assessment in `Admin/DoNew_Assessment_Summary_Yogesh.md`
      — kept as-is per maintainer decision; it intentionally documents the project's origin story.

### Follow-up note (not an action item, just a fact)
Moving the third-party PDFs, newspaper clipping, and DoNew screenshot out of the working tree does
**not** remove them from git history, since they were already committed. If the redistribution risk
needs to be fully closed, that requires a git history rewrite (e.g. `git filter-repo`) and a
force-push — a deliberate, destructive operation that is yours to decide on and perform, not
something done as part of this review.
