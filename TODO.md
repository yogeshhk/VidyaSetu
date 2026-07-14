# TODO: Discoverability Upgrade

Working checklist from the non-tech repo review (see `reports/upgrade_nontech_*.md` once written for the full plan). Items are worked one at a time; each is confirmed individually before execution. Checked off immediately as completed.

## Structural Changes
- [x] Add a short README to `LaTeX/` explaining it's a personal presentation-template toolkit
- [x] Link `References/Notes.md` from the root README (the PDFs themselves were moved out in the redistribution-risk step above)
- [x] Surface the VidyaSetu mind map from the root README — rendered `Admin/VidyaSetuMindMap.pdf` to `Admin/VidyaSetuMindMap.png` and embedded it under a new "Project at a Glance" heading
- [x] Extract the "How to Contribute" section from `Playbook/Playbook.md` into a standalone `CONTRIBUTING.md` at the repo root

## Critical Issues
- [x] Clean up em dash in `Admin/DoNew_VidyaSetu_Insights.md` (line 28)
- [x] Clean up em dash in `References/Notes.md` (line 15)
- [x] Decide handling of third-party redistribution risk: `References/*.pdf` (9 copyrighted journal articles) — moved to `VidyaSetu_removed_thirdparty/References/` outside the repo
- [x] Decide handling of third-party redistribution risk: `References/WhatsApp Image 2026-02-22 at 3.29.45 PM.jpeg` (scanned newspaper clipping) — moved to `VidyaSetu_removed_thirdparty/References/` outside the repo
- [x] Decide handling of third-party redistribution risk: `Admin/20DoNewNinjaSkills.png` (third-party "DoNew" framework screenshot) — moved to `VidyaSetu_removed_thirdparty/Admin/`; broken image reference in `Admin/DoNew_VidyaSetu_NinjaSkills.md` replaced with a text description

## Clutter & Redundancy
- [x] Remove commented-out `-- OLD --` blocks in `Playbook/students_playbook.md`, `colleges_playbook.md`, `professionals_playbook.md`, `facilitators_playbook.md`
- [x] Remove commented-out "Appendix: Development Plan" in `ToDos.md`
- [x] Trim commented-out unrelated NLP/ML and "Yati.io" content in `LaTeX/about_me.tex`

## Improvement Suggestions
- [x] Add license + last-commit/contributors badges to README (dynamic shields.io badges)
- [x] Embed `Admin/VidyaSetuMindMap.pdf` (as PNG) near the top of the README (done as part of Structural Changes above)
- [x] Add a one-line "who this is for" summary near the top of the README

## Documentation Gaps
- [x] Add `CONTRIBUTING.md` (done as part of Structural Changes above)
- [x] Add `CODE_OF_CONDUCT.md` (standard Contributor Covenant v2.1)
- [x] Add issue templates / PR template (`.github/ISSUE_TEMPLATE/content_suggestion.md`, `.github/PULL_REQUEST_TEMPLATE.md`)
- [x] Build a root-level catalog: `CONTENTS.md`, linked from the README, all links verified to resolve

## Manual (maintainer-only, cannot be done by the agent)
- [ ] Set GitHub repo Description and Topics (Settings gear next to "About")
- [ ] Optionally set a social preview image (Settings → General → Social preview)

## Personal & Sensitive Information — decided
- [x] Phone number in `LaTeX/about_me.tex` comment — already removed as a side effect of the earlier clutter trim (it was inside the deleted commented-out block)
- [x] Third-party names/relations table in `Admin/DoNew_VidyaSetu_Insights.md` comment — deleted entirely per maintainer decision
- [x] Maintainer's own psychometric summary in `Admin/DoNew_Assessment_Summary_Yogesh.md` — kept as-is per maintainer decision (intentional origin-story content)
