# Sum: 15- Forensics

Created time: 3 avril 2025 18:12
Last edited by: OLB_
Last edited time: 3 avril 2025 18:15

<aside>
👉

Digital forensics plays a role in legal cases, criminal investigations,
internal investigations, incident responses, and intelligence activities.
For most organizations, legal holds, e-discovery, internal
investigations, and IR are the most common uses. Legal holds are a
notice from opposing counsel to retain data that may be relevant to a
current or pending case. Using a discovery model like the EDRM
model can help ensure that your discovery and holds process is well
planned and executed.

Forensic data acquisition can be time sensitive, so analysts must
understand the order of volatility for systems, which identifies the
targets most likely to change or lose data if they are not preserved first.
Throughout acquisition and the forensic life cycle, maintaining a chain
of custody helps ensure that evidence is admissible in court.

Cloud services have included additional complexity to forensic efforts.
In addition to technical concerns that can make it impossible to
conduct direct forensic investigations, contractual and policy
considerations need to be taken into account. Many organizations now
evaluate right-to-audit clauses, regulatory and jurisdictional concerns,
and data breach notification time frames as part of their contracting
process for new third-party and cloud services.

Acquisition tools and forensic suites provide the ability to collect
forensic images and data and to analyze them using powerful
capabilities like automatic recognition of images and documents, as
well as timelining and other features. Hashing and validating ensures
that acquired images are intact, and matching the source data helps
ensure that the forensic data will be admissible in court.

Reporting occurs at the end of a forensic analysis and needs to be
complete, with documented reasoning for each conclusion or
statement made about the forensic evidence. A standard forensic
reporting format helps ensure that readers know what to expect and
that they can easily understand what is being presented.

Forensic techniques may be used for more than just investigations and
incident response. They also have a role to play in both intelligence
and counterintelligence activities. Intelligence organizations may
acquire information using forensic techniques or work to combat other
organizations' activities by examining the tools and artifacts that they
leave behind.

**Legal holds and e-discovery drive some forensic activities.**
Organizations face legal cases and need to respond to legal holds,
which require them to preserve and protect relevant information for
the active or pending case. E-discovery processes also require forensic
and other data to be provided as part of a legal case. Organizations
must build the capability and technology to respond to these
requirements in an appropriate manner to avoid losing cases in court
and to support incident response processes.

**Acquisition techniques and procedures ensure usable and
admissible forensic data.** Different system components and
resources are more likely to be changed or lost during the time it takes
for a forensic acquisition. Thus, forensic practitioners refer to the
order of volatility to determine what is the most volatile and what is
the least volatile. Your forensic acquisition process should take the
order of volatility into account as well as the circumstances of your
acquisition process as part of incident response or legal holds to
determine what to capture first.

**There are many options for acquisition tools, and selecting
the right tool combines technical needs and skillsets.** Image
acquisition tools provide the ability to copy disks and volumes using a
bit-by-bit method that will capture the complete image including
unused or slack space. Acquisition processes vary based on where the
data is located, including acquisition using snapshots of virtual
machines, data volume copies for cloud environments, and disk
images for workstations and mobile devices. Incident responders must
bear in mind both maintaining a chain of custody and the specific
technical requirements of the system or devices they are capturing
data from.

**Validation and preservation of forensic data is a key part of
the forensic process.** Hashing drives and images ensures that the
acquired data matches its source. Forensic practitioners continue to
commonly use MD5 or SHA1 despite issues with both hashing
methods because adversarial techniques are rarely at play in forensic
examinations. Checksums can be used to ensure that data is not
changed, but they do not create the unique fingerprints that hashes are
also used to provide for forensic artifacts. Preservation requires
following chain-of-custody processes as well as forethought about the
use of write blockers, forensic copies, and documented processes and
procedures.

**Forensic reports must be well organized and to the point**.
Forensic analysis doesn't end when the technical examination of
devices and drives is over. Forensic reports summarize key findings,
then explain the process, procedures and tools, and any limitations or
assumptions that impact the investigation. Next, they detail the
forensic findings with appropriate evidence and detail to explain how
conclusions were reached. They conclude with recommendations or
overall conclusions in more detail than the summary provided

</aside>

## EXAM CHECK

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:

Domain 4.0: Security Operations
4.8. Explain appropriate incident response activities.
Digital forensics (Legal hold, Chain of custody,

- Acquisition, Reporting, Preservation, E-discovery)