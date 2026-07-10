---
title: HPC and Tower Agent guidance
contributors: [Ziad Al-Bkhetan, Johan Gustafsson, Georgina Samaha, Giorgia Mori]
description: Administrator guidance for connecting Slurm or PBS Pro HPC infrastructure through Tower Agent credentials.
toc: true
type: guides
---

**For:** workspace administrators and HPC specialists  
**You will need:** workspace administrator access, an HPC account, a project allocation, terminal access and outbound network connectivity

## Overview

Seqera supports HPC systems using workload managers such as Slurm and PBS Pro. Tower Agent runs on the HPC and communicates with Seqera to launch and monitor work.

Compute environments and credentials are shared within a workspace, but each HPC user should use their own account and personal access token unless an explicitly approved service-account model is available.

## 1. Create a personal access token

Open **User tokens** from your user menu, create a descriptively named token and copy it to a secure location. The token is displayed only at creation time. Do not share it or commit it to version control.

Use separate tokens for distinct credentials or infrastructure where practical, and revoke tokens that are lost or no longer needed.

## 2. Create Tower Agent credentials

1. Open the relevant workspace.
2. Go to **Credentials** and select **Add credentials**.
3. Choose the Tower Agent credential type.
4. Give it a descriptive name identifying the infrastructure and purpose.
5. Keep **Shared agent** disabled unless you have confirmed that the shared-agent model is appropriate and supported.
6. Keep the credential setup window open while starting the agent on the HPC.

See the [Seqera Agent credentials documentation](https://docs.seqera.io/platform/latest/credentials/agent_credentials) for current interface details.

## 3. Start the agent on the HPC

1. Log in to the HPC using your own account.
2. Create a dedicated agent working directory that is not shared with other users.
3. Copy the generated Slurm or PBS command from Seqera.
4. Add your personal access token and the intended agent work directory securely.
5. Run the agent according to local HPC policy, preferably through a managed background job rather than an unattended login shell.
6. Confirm that the agent connects before saving the credential.

The agent requires outbound access to the Seqera service.

## 4. Configure the compute environment

1. Open **Compute environments** and choose **Add compute environment**.
2. Select the workload-manager platform used by the HPC, such as Slurm or PBS Pro.
3. Give the environment a descriptive name including the HPC and project or allocation where useful.
4. Select the Tower Agent credential.
5. Configure the work directory, queues and project or account settings.
6. Add required module-loading or setup commands to the pre-run script.
7. Configure head-job resources and submission options in line with local HPC guidance.
8. Save and test the environment with a small workflow.

For example, Setonix uses Slurm and Gadi uses PBS Pro. Always follow the current documentation and policies of the relevant facility.

## 5. Use the environment

Each user running through their own HPC identity may need to start an agent using their own access token and the workspace credential connection ID. The environment is available while a valid agent connection is running.
