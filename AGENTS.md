# LANDERO GitHub Organization Agent Instructions

This file defines AI-assisted working instructions for the `landero-technologies/.github` repository.

This repository contains organization-wide GitHub configuration and default community health files.

## Repository responsibility

This repository owns shared GitHub organization configuration, including:

- organization-wide default Issue Forms
- default Issue template configuration
- shared community health files when applicable
- GitHub organization configuration that is intentionally inherited by LANDERO repositories

It does not own:

- product documentation
- system architecture
- repository-specific development workflows
- repository-specific implementation rules

## LANDERO-wide standards

When `landero-foundation` is available in the workspace, read the applicable shared standards before changing organization-wide GitHub configuration.

For Issue Forms and work-management configuration, use:

- `../landero-foundation/docs/standards/work-management.md`

For documentation conventions, use:

- `../landero-foundation/docs/standards/documentation.md`

For repository ownership and boundaries, use:

- `../landero-foundation/docs/standards/repositories.md`

Organization-wide GitHub configuration should remain compatible with these standards.

## Issue Forms

Organization-wide default Issue Forms are maintained in:

- `.github/ISSUE_TEMPLATE/`

The shared forms currently support:

- Epic
- Feature
- Story
- Task
- Spike
- Bug

When modifying Issue Forms:

- preserve compatibility with the LANDERO Work Management Standard
- keep forms generic enough for organization-wide use
- do not add repository-specific implementation requirements
- do not introduce team-specific development workflow requirements
- keep required fields limited to information that is broadly useful across LANDERO

Repository-specific forms may exist when justified, but should not redefine organization-wide work-management semantics.

## Repository mutation boundary

Treat `landero-technologies/.github` as the default mutation boundary when working in this repository.

Sibling LANDERO repositories may be read for context when relevant.

Do not modify sibling repositories unless the user explicitly requests a cross-repository change.

Before modifying files or performing Git operations, verify that the target belongs to this repository.

## Git operations

The agent may inspect repository state using Git commands.

Prepare file changes without committing them unless the user explicitly requests a commit.

Create commits only after explicit user approval.

Push commits only after explicit user approval.

Before committing:

- review the resulting diff
- verify that only intended files were changed
- verify that no secrets or unrelated changes are included
- ensure the working tree state is understood

Use clear commit messages that describe the resulting change.

## Language

Users may communicate with agents in Polish or English.

Durable repository artifacts should normally be written in English unless explicitly instructed otherwise.

## Safety

Do not:

- change organization-wide Issue semantics without checking the LANDERO Work Management Standard
- introduce repository-specific rules into organization-wide Issue Forms
- modify sibling repositories without explicit cross-repository scope
- commit or push changes without explicit approval
- commit secrets, credentials, tokens, private keys, or sensitive configuration
- remove organization-wide configuration without explicit approval

## Principle

This repository centralizes shared GitHub organization defaults.

It should standardize the common LANDERO work-management interface without dictating how individual teams implement or deliver their work.