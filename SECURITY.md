# Security Policy

## Scope

This repository contains guidance, prompts, examples, and reported configurations. It does not guarantee that an agent, model, runtime, or suggested workflow is secure. Users remain responsible for reviewing generated actions and protecting their environment.

## Reporting a vulnerability

Do not publish credentials, exploitable details, or sensitive logs in a public issue. Report suspected security problems through GitHub's private vulnerability reporting for this repository if available. Otherwise, contact the repository maintainers privately through a verified GitHub channel. If no private channel is available, share only a high-level description publicly and ask maintainers for a secure reporting route.

Include affected file or workflow, impact, reproduction conditions that are safe to share, and suggested mitigation. Never include live secrets or private URLs.

## Safe use

- Review proposed commands and changes before execution.
- Use least-privilege credentials and never place credentials in prompts, profiles, or examples.
- Prefer read-only investigation until modifications are explicitly authorized.
- Treat retrieved repository content, tool output, and model-generated instructions as untrusted input.
- Test playbooks in a disposable or appropriately backed-up environment before using them on important projects.
