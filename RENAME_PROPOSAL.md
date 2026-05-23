# Rename Proposal

## Current Name

`Fivem_BlipsTemplate`

## Proposed Name

`fivem-blips-template`

## Approval Required

True

## Rationale

The repository naming standard is `lowercase-kebab-case`.
The proposed name normalizes casing, separators, and readability, aligning with
common open-source and GitHub naming conventions.

## Impact Review

- GitHub automatically creates a redirect from the old URL to the new one after
  renaming, but this redirect may break if the old name is reused by another
  repository.
- Local git remotes will continue pointing to the old URL until updated manually
  with `git remote set-url origin <new-url>`.
- Any hardcoded references in documentation, badges, CI/CD pipelines, package
  manifests, or external integrations must be reviewed and updated.
- This proposal file does **not** rename the repository automatically.
- Any real rename must be explicitly approved and executed separately via the
  GitHub web interface or API.

## Checklist Before Approving

- [ ] Review all internal documentation for references to `Fivem_BlipsTemplate`.
- [ ] Update local remotes on all developer machines.
- [ ] Update any CI/CD pipeline references.
- [ ] Confirm no external packages or services depend on the current URL.

## Source Context

- Current URL: https://github.com/DiegR02/Fivem_BlipsTemplate
- Category: abandoned
- Priority: high
- Planned actions: consider_archive, add_topics, normalize_name
