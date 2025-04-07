# Sum: 10- Cloud & Virtualization

Created time: 31 mars 2025 13:58
Last edited by: OLB_
Last edited time: 3 avril 2025 15:26

<aside>
👉

Cloud computing changes the cybersecurity landscape. Although
cybersecurity professionals still must implement controls that protect
the confidentiality, integrity, and availability of information and
systems, they now do so in an environment that requires the
cooperation of cloud service providers. Under the shared
responsibility model of cloud security, cloud customers and providers
must come to a common understanding of who will be responsible for
meeting each security control requirement.

Organizations adopting cloud security controls may choose to
implement cloud-native security controls offered by their providers,
third-party controls that work across a variety of environments, or a
mixture of the two. They may implement cloud access security brokers
(CASBs) that allow the consistent enforcement of security policies
across diverse cloud platforms.

Organizations should also understand the vulnerabilities that appear
in cloud environments. These include virtualization issues, such as
virtual machine escape and resource reuse. Using cloud services
located in different jurisdictions may also introduce data sovereignty
concerns.

**Explain the three major cloud service models.** In the anything-
as-a-service (XaaS) approach to computing, there are three major
cloud service models. Infrastructure-as-a-service (IaaS) offerings
allow customers to purchase and interact with the basic building
blocks of a technology infrastructure. Software-as-a-service (SaaS)
offerings provide customers with access to a fully managed application
running in the cloud. Platform-as-a-service (PaaS) offerings provide a
platform where customers may run applications that they have
developed themselves.

**Describe the four major cloud deployment models**. Public
cloud service providers deploy infrastructure and then make it
accessible to any customers who wish to take advantage of it in a
multitenant model. The term private cloud is used to describe any
cloud infrastructure that is provisioned for use by a single customer. A
community cloud service shares characteristics of both the public and
private models. Community cloud services do run in a multitenant
environment, but the tenants are limited to members of a specifically
designed community. Hybrid cloud is a catch-all term used to describe
cloud deployments that blend public, private, and/or community
cloud services together.

Understand the shared responsibility model of cloud
security. Under the shared responsibility model of cloud security,
cloud customers must divide responsibilities between one or more
service providers and the customers' own cybersecurity teams. In an
IaaS environment, the cloud provider takes on the most responsibility,
providing security for everything below the operating system layer. In
PaaS, the cloud provider takes over added responsibility for the
security of the operating system itself. In SaaS, the cloud provider is
responsible for the security of the entire environment, except for the
configuration of access controls within the application and the choice
of data to store in the service.

**Implement appropriate security controls in a cloud
environment**. Cloud customers should understand how to use the
controls offered by providers and third parties to achieve their security
objectives. This includes maintaining resource policies and designing
resilient cloud implementations that achieve high availability across
multiple zones. From a storage perspective, cloud customers should
consider permissions, encryption, replication, and high availability.
From a network perspective, cloud customers should consider the
design of virtual networks with public and private subnets to achieve
appropriate segmentation. From a compute perspective, customers
should design security groups that appropriately restrict network
traffic to instances and maintain the security of those instances.

</aside>

## EXAM CHECK

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:
Domain 2.0: Threats, Vulnerabilities, and Mitigations
2.3. Explain various types of vulnerabilities.

- Virtualization (Virtual machine (VM) escape, Resource
reuse)
- Cloud-specific

Domain 3.0: Security Architecture
3.1. Compare and contrast security implications of
different architecture models.

- Architecture and infrastructure concepts (Cloud,
(Responsibility matrix, Hybrid considerations, Third-
party vendors), Infrastructure as code (IaC), Serverless,
Microservices, On-premises, Centralized vs.
decentralized, Containerization, Virtualization)

3.3. Compare and contrast concepts and strategies to
protect data.

- General data considerations (Data sovereignty)

Domain 4.0: Security Operations
4.1. Given a scenario, apply common security techniques to
computing resources.

- Hardening targets (Cloud infrastructure