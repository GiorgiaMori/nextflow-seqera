---
title: Run your first workflow
contributors: [Giorgia Mori]
description: A start-to-finish guide to launching a workflow through the Australian Nextflow Seqera Service.
toc: true
type: guides
---

**For:** researchers and other workspace participants  
**You will need:** access to a workspace, an available workflow and a configured compute environment

## Before you begin

Confirm that you can open the intended workspace and that it contains an appropriate workflow and compute environment. Ask your workspace administrator when you are unsure which resources to use.

## 1. Open the workspace

Log in and select the relevant organisation workspace from the workspace menu.

## 2. Select a workflow

Open the workspace launch area and select an existing workflow. If the workflow is not available, ask an administrator to add it or follow [Add a workflow](/user-guide/add-workflow) if you have permission.

## 3. Check the workflow revision

Confirm that the selected branch, tag or revision is the one recommended by the workflow maintainer. Using a fixed release or commit improves reproducibility.

## 4. Select a compute environment

Choose the compute environment approved for your project and data. Different environments may use different infrastructure, allocations, storage locations or costs.

## 5. Provide inputs and parameters

Complete the required workflow fields. Check:

- input file paths and permissions;
- output location;
- reference data and genome build;
- sample sheet format;
- profile or configuration settings;
- resource parameters and project allocation.

## 6. Review the launch configuration

Give the launch a descriptive name and review the workflow revision, compute environment, parameters and output location before launching.

Avoid including sensitive information in run names or free-text descriptions.

## 7. Launch and monitor the run

Launch the workflow, then open the run details to monitor its status. See [Monitor runs and find outputs](/user-guide/monitor-runs).

## 8. Record reproducibility information

Retain the workflow revision, parameters, configuration, input identifiers, run URL or run identifier, and output location with your project records.
