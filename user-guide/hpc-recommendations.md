---
title: Recommendations and best practice
contributors: [Ziad Al-Bkhetan, Johan Gustafsson, Giorgia Mori]
description: General recommendations for secure, reproducible and maintainable workspace and compute configuration.
toc: true
type: guides
---

## Workspace management

- Use descriptive names for workflows, credentials, compute environments and launch configurations.
- Record the owner, purpose and infrastructure associated with shared resources.
- Review participants regularly and apply least-privilege roles.
- Test changes with a small workflow before relying on them for production work.

## Tokens and credentials

- Never share personal access tokens or store them in source control.
- Use separate tokens for separate infrastructure where practical.
- Revoke lost, exposed or unused tokens promptly.
- Limit administrator permissions to people who manage shared resources.

## Tower Agent

- Use a dedicated agent working directory that is not shared by multiple users.
- Run the agent using a method permitted by the HPC provider, such as a scheduled background job.
- Use descriptive logs and retain enough information to diagnose disconnections.
- Confirm outbound network connectivity and local security requirements.

## Workflow reproducibility

- Prefer fixed releases, tags or commit revisions over moving development branches.
- Record workflow revision, parameters, configuration, inputs, compute environment and outputs.
- Validate new workflows and major updates with known test data.

## Resource use

- Use an appropriate long-running queue for the Nextflow head process where required.
- Use project and account settings consistently so resource usage is attributed correctly.
- Follow facility-specific recommendations for CPU, memory, storage and wall time.
