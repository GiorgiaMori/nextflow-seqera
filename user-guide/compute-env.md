---
title: Configure compute environments
contributors: [Ziad Al-Bkhetan, Johan Gustafsson, Georgina Samaha, Giorgia Mori]
description: An overview for administrators connecting HPC, cloud or other compute infrastructure to Seqera.
toc: true
type: guides
---

**For:** workspace administrators and infrastructure specialists  
**Required role:** workspace owner or administrator

## Do you need to configure compute?

You do not need to configure a compute environment to run workflows when your workspace already has an appropriate environment. Ask the workspace administrator which environment to use.

Create a new environment only when the workspace needs access to infrastructure that has not already been configured, or when a separate allocation, queue, storage location or security boundary is required.

## Before you begin

Confirm:

- you have administrator access to the Seqera workspace;
- you have an account and allocation on the target infrastructure;
- the target platform is supported by Seqera;
- network access between the infrastructure and Seqera is permitted;
- storage paths and permissions are understood;
- the intended data is permitted on the infrastructure.

## Choose the relevant instructions

- For Slurm or PBS Pro HPC systems using a Tower Agent, see [HPC and Tower Agent guidance](/user-guide/hpc-agent).
- For AWS Batch and other commercial cloud services, see [Cloud and other infrastructures](/user-guide/cloud-compute).
- For platform options not covered locally, see the [Seqera compute environment documentation](https://docs.seqera.io/platform/latest/compute-envs/overview/).

## Test the environment

After configuration, run a small known workflow and confirm job submission, container execution, input access, output publication, logs and resource accounting.
