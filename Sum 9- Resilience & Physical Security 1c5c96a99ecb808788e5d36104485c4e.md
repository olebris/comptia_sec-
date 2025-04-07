# Sum:  9- Resilience & Physical Security

Created time: 29 mars 2025 18:39
Last edited by: OLB_
Last edited time: 3 avril 2025 15:26

<aside>
👉

Building a resilient infrastructure with the ability to recover from
issues is a key part of ensuring the availability of your systems and
services. Redundant systems, networks, and other infrastructure and
capabilities help provide that resilience. At the same time, techniques
like the use of geographic dispersal, power protection, and even
diversity of technologies and vendors can play a critical role in keeping
your organization online and operational.

Resilience relies on a variety of technical and procedural design
elements. Geographic diversity helps ensure that a natural disaster or
human-caused issue doesn't take down your organization. High-
availability designs using clustering and load balancing handle both
scaling and system and component failures. Multicloud systems and
platform diversity are used to avoid a vendor's outage or failure from
causing broader issues. Backup power from generators and UPS
systems helps control power-related events.

Backups, whether to tape, disk, or third-party storage services, help
ensure that data is not lost if something happens to systems or drives.
You should know the difference between a full backup, a differential
backup, and an incremental backup. Snapshots, which copy the state
of a system at a point in time, and images, which are used to copy a
complete system, are also used as ways to both back up and clone
systems. Journaling records changes, allowing for them to be
replicated if needed.

How you respond to an outage or issue and how you recover from it
can make the difference between being back online quickly or being
offline for an extended period of time. Capacity planning, testing, and
designing for continuity of operations are all key parts of being ready
for an issue and handling it appropriately.

Disaster recovery sites are used to return to operation, with hot sites
built and fully ready to go, warm sites waiting for data and staff to
operate, and cold sites providing power and connectivity but needing
significant effort and deployment of technology to come online. In any
restoration event, knowing the restoration order will help bring
systems and services online in an order that makes sense based on
dependencies and criticality.

Keeping organizations physically secure also helps protect them. Site
security involves using controls to make facilities less likely to be
targeted, using controls like fences, bollards, lighting, access badges,
and entry access systems to dissuade potential bad actors. Sensors are
used to detect issues and events and to trigger responses. Detecting
physical attacks requires additional care because they may not be
easily detected by automated or electronic means.

**Redundancy builds resilience.** Redundant systems, networks, and
even datacenters are a key element in ensuring availability. Redundant
designs need to address the organizational risks and priorities that
your organization faces to ensure the best trade-offs between cost and
capabilities. Geographic dispersal; load balancers and clustering;
power protection and redundancy; RAID; backups; and diversity of
technologies, systems, cloud service providers, and platforms are all
ways to build and ensure resiliency. Considerations include
availability, resilience, cost, responsiveness, scalability, ease of
deployment, risk transference, ease of recovery, patch availability,
inability to patch, power, and compute. Capacity planning helps to
ensure that there is enough capacity to handle issues and outages
including ensuring you have enough people, technology, and
infrastructure to recover. Multicloud environments as well as platform
diversity can help ensure that a single technology or provider's outage
or issue does not take your organization offline, but they create
additional complexity and costs.

**Backups help ensure organizations can recover from events
and issues**. Backups are designed to meet an organization's
restoration needs, including how long it takes to recover from an issue
and how much data may be lost between backups. Backup locations
and frequency are determined based on the organization's risk profile
and recovery needs, with offsite backups being a preferred solution to
avoid losing backups in the same disaster as the source systems.
Snapshots, journaling, and replication each have roles to play in
ensuring data is available and accessible. Encryption is used to keep
backups secure both in-transit and at rest.

**Response and recovery are critical when failures occur.**
Failures will occur, so you need to know how to respond. Having a
disaster recovery location, like a hot, warm, or cold site or a redundant
cloud or hosted location, can help ensure that your organization can
return to operations more quickly. Having a predetermined
restoration order provides a guideline on what needs to be brought
back online first due to either dependencies or importance to the
organization. Testing, including tabletop exercises, failover testing,
simulations, and parallel processing, are all common ways to ensure
response and recovery will occur as planned.

**Physical security controls are a first line of defense**. Keeping
your site secure involves security controls like fences, lighting, alarms,
bollards, access control vestibules, cameras, and other sensors.
Ensuring that only permitted staff are allowed in using locks, badges,
and guards helps prevent unauthorized visitors. Sensors must be
selected to match the environment and needs of the organization.
Infrared, ultrasonic, pressure, and microwave sensors have different
Technet24
capabilities and costs. Brute-force attacks, as well as attacks against
RFID and environmental attacks, need to be considered in physical
security design.

</aside>

## EXAM CHECK

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:
Domain 1.0: General Security Concepts
1.2. Summarize fundamental security concepts.

- Physical security (Bollards, Access control vestibule,
Fencing, Video surveillance, Security guard, Access
badge, Lighting, Sensors)

Domain 2.0: Threats, Vulnerabilities, and Mitigations
2.4. Given a scenario, analyze indicators of malicious
activity.

- Physical attacks (Brute force, Radio frequency
identification (RFID) cloning, Environmental)

Domain 3.0: Security Architecture
3.1. Compare and contrast security implications of
different architecture models.

- Considerations (Availability, Resilience, Cost,
Responsiveness, Scalability, Ease of deployment, Risk
transference, Ease of recovery, Patch availability,
Inability to patch, Power, Compute)

3.4. Explain the importance of resilience and recovery in
security architecture.

- High availability (Load balancing vs. clustering)
- Site considerations (Hot, Cold, Warm, Geographic
dispersion)
- Platform diversity
- Multi-cloud systems
- Continuity of operations
- Capacity planning (People, Technology, Infrastructure)
- Testing (Tabletop exercises, Fail over, Simulation,
Parallel processing)
- Backups (Onsite/offsite, Frequency, Encryption,
Snapshots, Recovery, Replication, Journaling)
- Power (Generators, Uninterruptible power supply
(UPS))