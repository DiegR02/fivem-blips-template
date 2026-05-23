# Repository Review

## Summary

This document records the findings and recommendations from an automated
repository maintenance review of `Fivem_BlipsTemplate`.

## Classification

| Field | Value |
|-------|-------|
| Category | abandoned |
| Priority | high |
| Reason | Repository has not been updated in over 1,000 days. Metadata (topics, normalized name) is missing or incomplete. |

## Findings

1. **Naming** — The repository name `Fivem_BlipsTemplate` uses mixed case and
   underscores. The recommended convention is `lowercase-kebab-case`.
2. **Topics** — No topics are currently set. Topics improve discoverability on
   GitHub search and the Explore page.
3. **Activity** — The repository has been inactive for approximately 1,182 days,
   which qualifies it as abandoned under current maintenance policy.
4. **License** — No license file was detected. This limits how others can legally
   use or contribute to the code.
5. **README** — A README exists but may lack installation, usage, and status
   information. See `README_PROPOSAL.md` for a suggested improvement.

## Recommendations

| Action | Rationale |
|--------|-----------|
| `add_topics` | Improves discoverability; zero topics currently set. |
| `consider_archive` | Repository is inactive; archiving signals its status clearly. |
| `normalize_name` | Aligns with `lowercase-kebab-case` naming standard. |

## Metadata Proposal

- **Suggested topics:** `fivem`, `lua`, `blips`, `gta5`, `fivem-script`, `blipstemplate`
- **Current description present:** Yes
- **Current topics present:** No
- **Proposed description:** See `repo_metadata_proposal.json`

## Files Generated

| File | Purpose |
|------|---------|
| `RENAME_PROPOSAL.md` | Documents the proposed repository rename with impact checklist. |
| `README_PROPOSAL.md` | Improved README draft for human review. |
| `REPOSITORY_REVIEW.md` | This review document. |
| `repo_metadata_proposal.json` | Machine-readable metadata update proposal. |

## Safety

All changes were prepared on a dedicated review branch
(`repo-cleanup-2026-05-24`) for human review. **None of these files should be
merged or published without explicit manual approval.** No source files have been
modified.
