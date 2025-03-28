# Sum: 3-  Malicious Code

Created time: 27 mars 2025 21:24
Last edited by: OLB_
Last edited time: 27 mars 2025 21:57

<aside>
👉

Security professionals need to be aware of the most common forms of
malware. This includes understanding how to identify common
indicators of malicious activity related to malware attacks and
malware itself.
The Security+ exam objectives focus on a few different types of
malware. These include ransomware, which most frequently targets
victims by encrypting files and holding them for ransoms paid via
cryptocurrency. Trojans are malware that is disguised to look like
legitimate software but that takes malicious action once downloaded
and run.
Worms are malware that spread themselves on networks via
vulnerable services, email, or file shares. Viruses are similar but only
infect local systems and often require user action like running an
application to infect a system.
Spyware is malicious software that is intended to gather information
about users, systems, and networks. It then sends that information
back to remote systems or command and control servers. Keyloggers
are a specialized type of spyware that capture keystrokes, allowing
malicious actors to know what you've typed. Keyloggers exist in both
software and hardware form, although the Security+ exam focuses on
them as malware.
Rootkits are used to retain access to a system and are commonly part
of an attacker's toolkits as well as being used together with other
malware to help keep a foothold on a compromised system. Rootkits
are designed to conceal malicious action and to counter protective
measures like antivirus, antimalware, and endpoint detection and
response tools.
Logic bombs are code that executes under a specific condition or
conditions, taking unwanted action. Unlike the other malware on this
list, logic bombs typically need to be identified by reviewing source
code or scripts.
Bloatware is simply unwanted software installed on systems by
vendors or as part of software packages. Bloatware takes up resources
like disk space, memory, and CPU cycles. It isn't truly malicious
software but is often vulnerable to attack and can allow actual
malicious software to gain access to systems. Bloatware is typically
removed by uninstalling it.
Finally, there are many ways to fight malware, from antivirus and
endpoint detection and response tools to configuration and patching.
Awareness is often the most effective tool in an organization's arsenal
as it can help prevent attacks, can allow responses to occur more
quickly, and can help limit the impact of human mistakes throughout
malware life cycles and attacks.

**Understand and explain the different types of malware.**
Malware includes ransomware, Trojans, worms, spyware, bloatware,
viruses, keyloggers, logic bombs, and rootkits. Each type of malware
has distinctive elements, and security analysts need to know what
identifies each type of malware, how to identify it, what controls are
commonly deployed against it, and what to do if you encounter it.

**Explain common indicators of malicious activity associated
with malware types.** Indicators of compromise associated with
malware vary based on the type of malware and how it is designed and
used. Common examples of IoCs associated with malware include
command and control (C&C) traffic patterns, IP addresses, hostnames,
and domains. Use of system utilities in unexpected ways, lateral
movement between systems, creation of files and directories,
encryption of files, and data exfiltration are also commonly seen,
particularly with Trojans and rootkits. Signatures for malware are
commonly used to identify specific files associated with given malware
packages although malware writers use defensive techniques intended
to make this harder.

**Understand the methods to mitigate malware**. Malware may
require specialized techniques and processes to remove it or to deal
with the impact of the malware. Techniques range from manual
removal to the use of tools to identify and remove malicious files, and
often rely on reinstallation of a system or restoration from a known
good backup to ensure all malware is removed.

</aside>

## CHECK EXAM

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:
Domain 2.0: Threats, Vulnerabilities, and Mitigations

2.4. Given a scenario, analyze indicators of malicious
activity.

- Malware attacks (Ransomware, Trojan, Worm,
Spyware, Bloatware, Virus, Keylogger, Logic bomb,
Rootkit)