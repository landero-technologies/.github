# LANDERO GitHub Organization Agent Instructions

This file defines repository-specific AI guidance for `landero-technologies/.github`.
It does not impose repository-specific development workflows on LANDERO teams.

## Repository responsibility

This repository owns shared GitHub organization configuration, including:

- organization-wide default Issue Forms;
- default Issue template configuration;
- shared community health files;
- GitHub configuration intentionally inherited by LANDERO repositories.

It does not own:

- product documentation;
- system architecture;
- repository-specific implementation rules;
- repository-specific development workflows.

## Required context

Before changing organization-wide GitHub configuration, read the applicable documents in:

- `../landero-foundation/docs/standards/work-management.md`;
- `../landero-foundation/docs/standards/documentation.md`;
- `../landero-foundation/docs/standards/repositories.md`.

Keep organization-wide configuration compatible with those standards.

## Issue Forms

Default Issue Forms are maintained in:

- `.github/ISSUE_TEMPLATE/`

The shared forms support:

- Epic;
- Feature;
- Story;
- Task;
- Spike;
- Bug.

When modifying Issue Forms:

- preserve the LANDERO Work Management Standard;
- keep forms generic enough for organization-wide use;
- keep required fields limited to broadly useful information;
- do not add repository-specific implementation requirements;
- do not introduce team-specific development workflow requirements.

Repository-specific forms may exist when justified, but must not redefine organization-wide work-management semantics.

## Repository boundaries

Treat `landero-technologies/.github` as the default mutation boundary.

Sibling repositories may be read for context.
Do not modify them unless the user explicitly approves a cross-repository change.

Before changing organization-wide configuration, verify that the target belongs to this repository.

## Git and safety

Inspect Git state before changing files or performing Git operations.
Do not commit or push without explicit approval.
Before committing, verify the diff, intended files, secrets, and working-tree state.

Do not:

- change organization-wide Issue semantics without checking the Work Management Standard;
- introduce repository-specific rules into organization-wide forms;
- remove shared organization configuration without explicit instruction;
- create or modify Issues without approval;
- commit secrets or sensitive configuration;
- impose team-specific workflows through shared defaults.

The repository standardizes the common LANDERO GitHub interface while preserving team autonomy over implementation and delivery.
