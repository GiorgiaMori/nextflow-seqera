---
title: Cloud and other infrastructures
contributors: [Ziad Al-Bkhetan, Johan Gustafsson, Giorgia Mori]
description: Guidance and external references for configuring cloud and other supported compute platforms.
toc: true
type: guides
---

**For:** workspace administrators and cloud or infrastructure specialists

## AWS Batch

Seqera supports AWS Batch and Batch Forge. Configuration requires an approved AWS account, suitable permissions, networking, storage and cost controls. Follow the [Seqera AWS Batch documentation](https://docs.seqera.io/platform/latest/compute-envs/aws-batch/).

Before enabling broad use, confirm budget ownership, region, storage lifecycle, access controls, logging and the treatment of sensitive data.

## Azure and other platforms

See the [Seqera compute environment overview](https://docs.seqera.io/platform/latest/compute-envs/overview/) for currently supported platforms and configuration instructions.

## Validate before use

Test a small workflow and verify data access, container retrieval, outputs, logs, cost attribution and cleanup behaviour before using production data.
