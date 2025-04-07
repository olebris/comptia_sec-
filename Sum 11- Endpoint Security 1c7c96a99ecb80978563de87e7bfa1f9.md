# Sum: 11- Endpoint Security

Created time: 31 mars 2025 17:24
Last edited by: OLB_
Last edited time: 31 mars 2025 17:29

<aside>
👉

Endpoints are the most common devices in most organizations, and
they are also the most varied. Therefore, you must pay particular
attention to how they are secured from the moment they boot up. You
can do this by using secure boot techniques built into the firmware of
the systems themselves to preserve boot integrity while leveraging
TPMs, hardware security modules, key management systems, and
secure enclaves to properly handle secrets.

Understanding operating system vulnerabilities and their impact in
endpoint security is critical for security professionals. You also need to
be aware of and understand the impact of hardware life cycles,
including firmware updates and end-of-life and legacy hardware
considerations.

As a security professional, you need to know about the many common
types of endpoint protection options that are available, as well as when
and how to use them. Antivirus/antimalware software helps prevent
malware infection. Host-based firewalls and IPSs, disabling ports and
protocols, changing default passwords and other settings, and using
security baselines are all common techniques used as part of endpoint
protection. Tools like Group Policy and SELinux help to enforce and
improve security baselines and capabilities. EDR and XDR tools add
another layer to the set of security protections for endpoint devices by
combining detection and monitoring tools with central reporting and
incident response capabilities. Finally, data loss prevention (DLP)
tools are deployed to ensure that data isn't inadvertently or
intentionally exposed.

Drive encryption keeps data secure if drives are stolen or lost. At the
end of their life cycle, when devices are retired or fail, or when media
needs to be reused, sanitization procedures are employed to ensure
that remnant data doesn't leak. Wiping drives as well as physical
destruction are both common options. It is critical to choose a
sanitization method that matches the media and security level
required by the data stored on the media or drive.

Another important element in endpoint security is how organizations
secure specialized and embedded systems. Internet of Things, SCADA,
ICS, and other devices using real-time operating systems are
everywhere throughout organizations in medical systems, smart
meters, vehicles, industrial processes and manufacturing equipment,
drones, smart devices, and a multitude of other locations. With often
limited capabilities, different security models, and a host of other
special requirements, securing embedded systems takes additional
focus and planning to ensure they remain secure.

Asset management starts with the procurement process when security
considerations are taken into account and assets, including hardware,
software, and data are all added to inventories and management
systems when they are acquired. Ensuring that assets have an owner
or responsible party and that they are classified based on the
sensitivity of the services or data that they support or contain is part of
the asset management process for security. Ensuring that assets are
inventoried and accounted for throughout their life cycle, and that
they are properly disposed of, finishes the life cycle.

**Understand operating system and hardware vulnerabilities.**
Operating systems may be vulnerable, host vulnerable services or
applications, or may have weak or insecure configurations that need to
be addressed. Patching, configuration management, and security
baselines all play a role in operating system security. Hardware
security frequently focuses on firmware updates and security as well as
life cycle management to properly address end-of-life and legacy
hardware issues.

**Hardening and protecting systems relies on security tools
and technology to keep systems secure**. Securing endpoint
devices requires considering the entire device: how it boots, how data
is secured, how it is configured, what services it provides, if its
communications are secure, and how it is protected against network
threats. Fortunately, security professionals have a wide range of tools,
including secure and trusted boot, to protect against attacks on the
boot process or drivers. Antivirus, antimalware, EDR, XDR, and data
loss prevention tools provide insight into what systems are doing and
where issues may exist while adding more controls that administrators
and security professionals can use to keep systems and data secure.
Network security tools like host intrusion prevention and detection
systems, host firewalls, and similar tools can detect and often stop
attacks from the network.

**Hardening endpoints also relies on configuration, settings,
policies, and standards to ensure system security**. Although
tools and technology are important to protect endpoints, configuration
and settings are also an important part of the process. Disabling
unnecessary services, changing default passwords, applying settings in
the Windows Registry or operating systems settings in Linux, and
otherwise using built-in and add-on configuration options to match
security configurations to the device's risk profile is critical. Finally,
patch management for the operating system and the applications
installed on devices protects against known vulnerabilities and issues.

**Specialized systems like SCADA, ICS, and IoT systems exist
throughout your organization and require unique security
solutions**. SCADA and ICS or industrial control systems are used to
manage and monitor factories, power plants, and many other major
components of modern companies. IoT systems are Internet-
connected devices that perform a wide variety of tasks, from
monitoring to home automation and more. They may be controlled by
third parties or have other security implications that must be
addressed as part of a security plan to keep each endpoint secure.

**Explain the importance of asset management for software,
data, and hardware**. Assets must be managed from acquisition
through their life cycle until disposal or decommissioning. Proper
management includes ensuring that ownership and classification are
maintained and tracked, and that inventories of assets are up to date
and include appropriate information to support operations, security,
and incident response needs.

**Drive encryption and sanitization help prevent data
exposure**. Encrypting drives and media helps keep them secure if
they are stolen or lost. Full-disk encryption covers the entire drive,
whereas volume or file encryption protects portions of the contents.
Sanitizing drives and media involves wiping them using a secure
deletion process, or their destruction to ensure that the data cannot be
recovered. Using appropriate processes based on the security
requirements for the data and the type of drive or media involved is
critical to making sure that the data is properly removed

</aside>

## EXAM CHECK

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:
Domain 1.0: General Security Concepts
1.4. Explain the importance of using appropriate
cryptographic solutions.

- Tools (Trusted Platform Module (TPM), Hardware
security module (HSM), Key management system,
Secure enclave)

Domain 2.0: Threats, Vulnerabilities, and Mitigations
2.3. Explain various types of vulnerabilities.

- Operating system (OS)-based
Hardware (Firmware, End-of-life, Legacy)
- Misconfiguration

2.5. Explain the purpose of mitigation techniques used to
secure the enterprise.

- Patching
- Encryption
- Configuration enforcement
- Decommissioning
- Hardening techniques (Encryption, Installation of
endpoint protection, Host-based firewall, Host-based
intrusion prevention system (HIPS), Disabling
ports/protocols, Default password changes, Removal of
unnecessary software)

Domain 3.0: Security Architecture
3.1. Compare and contrast security implications of
different architecture models.

- Architecture and infrastructure concepts (IoT,
Industrial control systems (ICS)/supervisory control
and data acquisition (SCADA), Real-time operating
system (RTOS), Embedded systems)

Domain 4.0: Security Operations
4.1. Given a scenario apply common security techniques to
computing resources.

- Secure baselines (Establish, Deploy, Maintain)
- Hardening targets (Workstations, Servers, ICS/SCADA,
Embedded systems, RTOS, IoT devices)

4.2. Explain the security implications of proper hardware,
software, and data asset management.

- Acquisition/procurement process
- Assignment/accounting (Ownership, Classification)
- Monitoring/asset tracking (Inventory, Enumeration)
- Disposal/decommissioning (Sanitization, Destruction,
Certification, Data retention)

4.4. Explain security alerting and monitoring concepts and
tools.

- Tools (Antivirus, Data loss prevention (DLP))

4.5. Given a scenario, modify enterprise capabilities to
enhance security.

- Operating system security (Group Policy, SELinux)
- Endpoint detection and response (EDR)/extended
detection and response (XDR)