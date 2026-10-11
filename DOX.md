# DOX.md — BlueboxC DOX fork

## Purpose

Distribute the DOX framework with a stable AGENTS.md entry point and an editable DOX.md project hierarchy.

## Ownership

Root owns AGENTS.md, README.md, LICENSE and the inherited banner/video assets. templates/ owns reusable project documents and the optional Beads fragment.

## Local Contracts

- AGENTS.md contains generic framework rules; this file describes this repository.
- Keep copyable templates separate from this repository's own contracts. Do not replace templates with this repository's project index.
- Preserve upstream attribution and the MIT license.
- Publish only generic instructions and documentation; exclude operator configuration, project databases, credentials and session contents.
- Beads remains optional and applies only to an already initialized workspace. This fork creates no databases, hooks or runtime.
- Keep independent projects and module ownership separate unless the owner explicitly requests integration.

## Work Guidance

Keep the fork small. Reuse the upstream framework and document deviations in README.md.

## Verification

Check local Markdown links, indexed child documents, template section order, framework markers and the absence of machine-specific paths. Confirm the upstream LICENSE and image blob identities remain unchanged.

## Child DOX Index

- [templates/DOX.md](templates/DOX.md) — Copyable root/child contracts and optional Beads instructions.
