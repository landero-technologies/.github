# LANDERO GitHub Organization Configuration

This repository contains organization-wide GitHub configuration and default community health files for LANDERO.

## Purpose

The repository provides shared GitHub configuration that should apply consistently across LANDERO repositories.

It is not an application or implementation repository.

## Issue Forms

Organization-wide Issue Forms are maintained in:

```text
.github/ISSUE_TEMPLATE/
```

LANDERO provides standard forms for:

- Epic
- Feature
- Story
- Task
- Spike
- Bug

Repositories that do not define local Issue Forms should inherit these organization-wide defaults.

The forms are intended to keep Issue structure and expected information consistent across repositories.

## Local repository exceptions

A repository may define its own Issue Forms when there is a justified repository-specific need.

Local forms should remain compatible with:

- LANDERO Issue Types
- LANDERO Workflow
- shared work management conventions
- organization-wide GitHub Project usage

## Shared standards

The canonical LANDERO work management standard is maintained in:

```text
landero-foundation/docs/standards/work-management.md
```

Related organization-wide standards are maintained in:

```text
landero-foundation/docs/standards/
```

## Tool independence

LANDERO does not require a specific tool for creating or managing Issues.

Developers and teams may use:

- GitHub web interface
- GitHub CLI
- IDE integrations
- AI-assisted workflows
- automation
- other approved tooling

The resulting Issues should remain compatible with the shared LANDERO work management standard.

## Principle

This repository centralizes GitHub organization defaults.

It does not define how individual teams must implement or deliver their work.