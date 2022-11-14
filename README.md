# Multi-cloud Distributed Ledger (DLT) using Bevel and Anthos

Blockchain and DLT networks are multi-party systems. Each party has
their own tools, methodology and probably preferred cloud provider.
Although cloud Blockchain-as-a-service offerings (BaaS) can save a lot
of Infrastructure management efforts, it sometimes assumes that all parties will be
in the same Cloud or you may have limited region availability, scale or network segrargation.

If you want to build cross-cloud blockchain solutions with more control and portability in mind , this is what this article is trying to explore.

## Potential use cases

Imagine two parties join forces to build a blockchain network between
them. 'Party A' uses Azure, and "Party B" uses their own private cloud
infrastructure or other cloud provider.

In this scenario, managed blockchain is only useful if all party join
the same infrastructure. For these scenarios, we need to build a
standard platform across different infrastructure.

This platform must have standard visibility, operations, and compliance
across a wide range of resources and locations regardless of the hosting
infrastructure.

The benefits of using this approach are:

-   Supports heterogeneous deployments in a multi-cloud, multi-owner
    model where each node is completely owned and managed by separate
    organizations.

-   Centrally manage and monitor the Network status and compliance.

## Architecture

This reference Architecture provides a cloud agnostic & multi-party DLT
Network. It Supports heterogeneous deployments in a multi-cloud,
multi-owner model where each owner can host their nodes anywhere but be
part of the network.

This architecture uses a three-party example, each party host their
nodes in different location. As below:

-   Party A: Uses Azure Kubernetes Service.

-   Party B: Uses GCP GKE.

-   Party C: Uses AWS EKS.

<p align="center">
  <img src="images/MultiCloud-DLT.svg">
</p>


### Components
