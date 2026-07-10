---
title: Monitor runs and find outputs
contributors: [Giorgia Mori]
description: Guidance for monitoring workflow execution, reviewing logs and locating outputs.
toc: true
type: guides
---

**For:** all users who launch or review workflows

## Monitor run status

Open the run details page to review the overall status and individual tasks. A run may remain queued while waiting for the compute scheduler or may pause while large images, inputs or reference data are transferred.

## Review failed tasks

For a failed run, identify the first relevant failed task and review its command, exit status, standard output, standard error and execution log. Later failures may be consequences of the original problem.

## Find outputs

The output location depends on the workflow and launch configuration. Check the workflow documentation and the output path supplied at launch. Seqera records run metadata and logs, but scientific result files are generally written to the configured storage location.

## Resume or relaunch

Use resume only when the workflow, inputs and relevant configuration remain compatible with the previous run. Create a new launch when you need a distinct, auditable run with changed inputs or parameters.

## Record the run

Keep the workflow revision, launch parameters, run identifier, compute environment and output location with your analysis records.
