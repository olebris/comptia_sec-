# Sum: 14- Monitoring & Incident Response

Created time: 3 avril 2025 15:25
Last edited by: OLB_
Last edited time: 3 avril 2025 15:30

<aside>
👉

Every organization will eventually experience a security incident, and
having a solid incident response plan in place with a team who knows
what they need to do is critical to appropriately handling incidents.
Incident response typically follows a response cycle with preparation,
detection, analysis, containment, eradication, recovery, and lessons
learned phases. Although incident response may involve all of these
phases, they are not always conducted as distinct elements, and
organizations and IR teams may be in multiple phases at the same
time, depending on the status of the incident in question.

Preparation for incident response includes building a team, putting in
place policies and procedures, conducting exercises, and building the
technical and information-gathering infrastructure that will support
incident response needs. Incident response plans don't exist in a
vacuum. Instead, they are accompanied by communications and
stakeholder management plans, business continuity and disaster
recovery plans, and other detailed response processes unique to each
organization.

Threat hunting is used to help identify information that may indicate
an issue or compromise has occurred. Looking for key events like
account lockouts, concurrent session usage, attempts to access blocked
content, unusual resource consumption, resource inaccessibility,
missing logs, and out-of-cycle logging are all examples of data that can
help indicate compromise. Once they've identified an issue,
responders also need a way to talk about incidents, attackers, tools,
and techniques. That's where attack frameworks come into play.
MITRE's ATT&CK framework is a complete knowledgebase of
adversary tactics and techniques, and it has broad support in tools and
systems across the information security field.

A key component in many organizations' incident response plan is
monitoring computing resources, including systems, applications, and
infrastructure. That's often done using a security information and
event management (SIEM) tool. SIEM tools centralize information
gathering and analysis and provide dashboards and reporting that
allow incident information to be seen and quickly identified through
visualization, reporting, and manual analysis as well as automated
analysis capabilities. They work with logging infrastructures using
tools like syslog, syslog-ng, or others that gather and centralize logs,
building logging infrastructures that capture critical information used
for incident analysis. At the same time, additional information like
network flows and traffic information, file and system metadata, and
other artifacts are used by responders who need to analyze what
occurred on a system or network.

Once an incident has been identified, responders must mitigate and
control it. Doing so involves changing system, device, and software
configurations to prevent further issues and to stop the incident.
Firewall changes, use of security tools like MDM and DLP tools,
application allow lists and block lists or deny lists, and other
techniques may be used to stop an incident in its tracks. These
changes can be included in runbooks and playbooks that document
what the organization does and what choices and processes it will
follow before, during, and after it takes action. Finally, organizations
conduct lessons learned activities and run root cause analysis
processes to determine why an event occurred and how to prevent it in
the future.

**The incident response cycle and incident response process
outline how to respond to an incident.** The Security+ exam's
incident response cycle includes preparation, detection, analysis,
containment, eradication, recovery, and lessons learned. A response
process may not be in a single phase at a time, and phases may move
forward or backward depending on discoveries and further events.
Organizations train their staff and hold exercises like tabletop
exercises, walk-throughs, and simulations to allow their teams to
practice incident response.

**Threat hunting uses data to identify potential indicators of
compromise**. IoCs are a critical part of a modern threat hunter's
toolkit. They include detecting things like account lockout, concurrent
session usage, impossible travel, attempted access to blocked content,
resource consumption, resource inaccessibility, out-of-cycle logging,
and missing logs, among many other potential IoCs. IoCs are
documented and published through threat feeds and other services
and sources.

**Data sources and data management for incident response
provide insight into what occurred as well as investigative
and detection tools.** Security information and event management
(SIEM) tools are used in many organizations to gather and analyze
data using dashboards, automated analysis, and manual investigation
capabilities. Information such as vulnerability scan output, system
configuration data, system and device logs, and other organizational
data are ingested and analyzed to provide broad insight into events
and incidents. Network traffic information is gathered using NetFlow,
sFlow, and packet analyzers, among other tools. They provide useful
information about bandwidth usage as well as details about which
systems communicated, the ports and protocols in use, time and date,
and other high-level information useful for incident analysis. In
addition to log and event information, metadata from files and other
locations is commonly used for incident investigation and incident
response.

**Mitigation techniques ensure that the impact of incidents
are limited**. Incident responders use a variety of techniques to
mitigate and contain and recover from incidents. One of the most
common tasks is to change configuration for endpoint security
solutions as well as devices. That may include using allow lists or
block/deny lists, quarantining files or devices, making firewall
changes, using MDM or DLP tools, adding content or URL filtering
rules, or revoking or updating certificates. At the network and
infrastructure level, isolation, containment, and segmentation are all
used to separate systems involved in incidents from other systems or
networks. Root cause analysis is used to determine why an incident
was able to happen or why it happened and to guide preparation work
to avoid future incidents.

</aside>

## EXAM CHECK

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:

Domain 2.0: Threats, Vulnerabilities, and Mitigations
2.4. Given a scenario, analyze indicators of malicious
activity.

- Indicators (Account lockout, Concurrent session usage,
Blocked content, Impossible travel, Resource
consumption, Resource inaccessibility, Out-of-cycle
logging, Published/documented, Missing logs)

2.5. Explain the purpose of mitigation techniques used to
secure the enterprise.

- Application allow list
- Isolation
- Monitoring

Domain 4.0: Security Operations
4.4. Explain security alerting and monitoring concepts and
tools.

- Monitoring computing resources (Systems,
Applications, Infrastructure)
- Activities (Log aggregation, Alerting, Scanning,
Reporting, Archiving, Alert response and
remediation/validation (Quarantine, Alert tuning))
- Tools (Benchmarks, Agents/agentless, Security
information and event management (SIEM), NetFlow)

4.8. Explain appropriate incident response activities.

- Process (Preparation, Detection, Analysis,
Containment, Eradication, Recovery, Lessons learned)
- Training
- Testing (Tabletop exercise, Simulation)
- Root cause analysis
- Threat hunting

4.9. Given a scenario, use data sources to support an
investigation.

- Log data (Firewall logs, Application logs, Endpoint logs,
OS-specific security logs, IPS/IDS logs, Network logs,
Metadata)
- Data sources (Vulnerability scans, Automated reports,
Dashboards, Packet captures)