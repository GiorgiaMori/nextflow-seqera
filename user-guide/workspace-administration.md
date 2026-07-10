---
title: Workspace administrator overview
contributors: [Giorgia Mori]
description: Responsibilities and recommended setup sequence for Australian Nextflow Seqera Service workspace administrators.
toc: true
type: guides
---

**For:** workspace owners and administrators

## Administrator responsibilities

Workspace administrators coordinate access to shared workflows, credentials and compute environments. They should understand which infrastructure and data types are approved for the workspace and apply least-privilege access.

## Recommended setup sequence

1. Confirm the workspace purpose, users and data requirements.
2. [Manage participants and roles](/user-guide/manage-participants).
3. Add or validate the workflows required by the group.
4. Confirm whether an existing compute environment can be reused.
5. Configure credentials and compute only when needed.
6. Test the complete workflow with a small dataset.
7. Document workspace-specific conventions for users.

## Shared resources

Credentials, workflows and compute environments may be shared across workspace participants. Changes can therefore affect other users. Use descriptive names, document ownership and purpose, and avoid deleting or changing resources without checking their current use.

## Security and governance

Do not store tokens or secrets in workflow parameters, descriptions, scripts committed to version control, or shared documentation. Follow institutional requirements for sensitive data and approved compute locations.
