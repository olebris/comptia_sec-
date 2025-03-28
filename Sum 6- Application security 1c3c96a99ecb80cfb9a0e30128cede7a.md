# Sum: 6-  Application security

Created time: 27 mars 2025 23:42
Last edited by: OLB_
Last edited time: 27 mars 2025 23:46

<aside>
👉

Software plays an integral role in every organization, performing tasks
ranging from financial transactions to the management of sensitive
physical infrastructure components. Cybersecurity professionals must
ensure that the software used in their environment undergoes rigorous
testing to determine whether it meets business requirements and does
not expose the organization to serious cybersecurity risks.
Achieving this goal requires a strong understanding of the different
types of vulnerabilities that may arise in source code and in the
deployment of client-server and web applications. In this chapter, you
learned about many of these vulnerabilities and the tools used to
manage software security risks.

**Understand secure software development** concepts. Software
should be created using a standardized software development life cycle
that moves software through development, test, staging, and
production environments. Developers should understand the issues
associated with code reuse and software diversity. Web applications
should be developed in alignment with industry-standard principles
such as those developed by the Open Worldwide Application Security
Project (OWASP).

**Know how to analyze the indicators associated with
application attacks.** Software applications may suffer from a wide
range of vulnerabilities that make them susceptible to attack. You
should be familiar with these attacks, including memory injection,
buffer overflow, and race condition attacks. You should also
understand web-specific attacks, such as Structured Query Language
injection (SQLi) and cross-site scripting (XSS). Understanding the
methods behind these attacks helps security professionals build
adequate defenses and identify attacks against their organizations.

**Know how to implement application security controls.**
Application security should be at the forefront of security operations
principles. This includes protecting code through the use of input
validation. Web applications that rely on cookies for session
management should secure those cookies through the use of transport
encryption. Code should be routinely subjected to code review as well
as static and dynamic testing. Code signing provides end users with
assurance that code came from a trusted source. Sandboxing allows
the testing of code in an isolated environment.

**Explain the common benefits and drawbacks of automation
and scripting related to secure operations.** The main benefits of
automation are achieving efficiency and saving time, enforcing
baselines, standardizing infrastructure configurations, scaling in a
secure manner, retaining employees, lowering reaction times, and
serving as a workforce multiplier. The main drawbacks are complexity,
cost, creating a single point of failure, building up technical debt, and
maintaining ongoing supportability.

**Explain common use cases of automation and scripting for
cybersecurity.** Security professionals use automation and scripting
techniques in many different use cases. These include user and
resource provisioning, creating guard rails, managing security groups,
creating and escalating tickets, enabling and disabling services and
access, performing continuous integration and testing, and making use
of application programming interfaces (APIs).

</aside>

## CHECK EXAM

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:
Domain 2.0: Threats, Vulnerabilities, and Mitigations
2.3. Explain various types of vulnerabilities.

- Application (Memory injection, Buffer overflow, Race
conditions (Time-of-check (TOC), Target of evaluation
(TOE), Time-of-use (TOU)), Malicious update)
- Web-based (Structured Query Language injection
(SQLi), Cross-site scripting (XSS))

2.4. Given a scenario, analyze indicators of malicious
activity.

- Application attacks (Injection, Buffer overflow, Replay,
Privilege escalation, Forgery, Directory traversal)

Domain 4.0: Security Operations
4.1. Given a scenario, apply common security techniques to
computing resources.

- Application security (Input validation, Secure cookies,
Static code analysis, Code signing)
- Sandboxing

4.3. Explain various activities associated with vulnerability
management.

- Identification methods (Application security, Static
analysis, Dynamic analysis, Package monitoring)

4.7. Explain the importance of automation and
orchestration related to secure operations.

- Use cases of automation and scripting (User
provisioning, Resource provisioning, Guard rails,
Security groups, Ticket creation, Escalation,
Enabling/disabling services and access, Continuous
integration and testing, Integrations and Application
programming interfaces (APIs))
- Benefits (Efficiency/time saving, Enforcing baselines,
Standard infrastructure configurations, Scaling in a
secure manner, Employee retention, Reaction time,
Workforce multiplier)
- Other considerations (Complexity, Cost, Single point of
failure, Technical debt, Ongoing supportability)

Domain 5.0: Security Program Management and
Oversight
5.1. Summarize elements of effective security governance.

- Policies (Software development lifecycle (SDLC))