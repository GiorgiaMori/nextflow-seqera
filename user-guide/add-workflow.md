---
title: Add a workflow to a workspace
contributors: [Ziad Al-Bkhetan, Johan Gustafsson, Giorgia Mori]
description: Instructions for workspace administrators who add a Nextflow workflow to a workspace.
toc: true
type: guides
---

**For:** workspace owners, administrators and users permitted to manage workflows

## Before adding a workflow

Confirm that:

- the workflow is maintained in an accessible Git repository;
- its documentation describes required inputs and outputs;
- the intended revision is suitable for production use;
- it is compatible with the selected compute environment;
- its licence and data requirements are appropriate for your use.

## Add the workflow

Follow the [Seqera documentation for adding a pipeline](https://docs.seqera.io/platform/latest/launch/launchpad/#adding-a-new-pipeline).

Use a clear name and description that help workspace participants distinguish the workflow from alternatives. Where possible, configure or document a recommended stable release rather than relying on a moving development branch.

## Test before broad use

Launch the workflow with a small, known dataset. Confirm that the compute environment, software containers, storage paths, parameters and outputs behave as expected before directing other users to it.

## Related guidance

- [Run your first workflow](/user-guide/run-first-workflow)
- [Configure compute environments](/user-guide/compute-env)
- [Recommendations and best practice](/user-guide/hpc-recommendations)
