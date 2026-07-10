---
title: Troubleshooting
contributors: [Giorgia Mori]
description: Checks for common access, workflow and compute-environment problems.
toc: true
type: guides
---

## I cannot see my workspace

- Confirm you logged in with the email address added by the workspace administrator.
- Ask the administrator to check the workspace **Participants** list.
- Refresh the browser or sign out and back in after membership changes.

## The compute environment is unavailable

- Check whether the required Tower Agent or cloud connection is active.
- Confirm the credential and compute environment have not been disabled or changed.
- Check infrastructure availability, allocation status, queues and network access.
- Ask the administrator whether the environment is shared or requires a user-specific agent.

## A run remains queued

Check scheduler queues, project allocation, requested resources, head-job submission options and any facility outage or maintenance notice.

## A task failed

Review the first relevant failed task, including exit code, standard error, command, work directory and execution log. Check input paths, permissions, containers, reference data and available resources.

## Outputs are missing

Confirm the output path supplied at launch, workflow publication settings, storage permissions and whether the workflow completed its final publication steps.

## Resume does not work as expected

Resume relies on compatible cached work. Changes to inputs, workflow code, configuration, work directory or cleanup may prevent reuse. Relaunch without resume when a clean execution is required.
