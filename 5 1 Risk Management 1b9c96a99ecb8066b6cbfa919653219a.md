# 5.1 Risk Management

Created time: 17 mars 2025 22:35
Last edited by: OLB_
Last edited time: 5 avril 2025 17:40

- **Threats** are any possible events that might have an adverse impact on the confidentiality, integrity, and/or availability of our information or information systems.
- **Vulnerabilities** are weaknesses in our systems or controls that could be exploited by a threat.
- **Risks** occur at the intersection of a vulnerability and a threat that might exploit that vulnerability.

## Risk Assessment

- Evaluate Impact and Likelihood of a risk
    - Risk Severity = likelihood * impact
- Ah Hoc risk assessment
    - for one particular situation or threat or new project
- One time risk assessment
    - for a company acquisition, CEO request  …
- Recurring risk assessments
    - are performed at regular intervals but no particular monitoring in between
- Continuous risk assessment
    - part of an ongoing process and monitoring
    - required by compliance / legal requirement

## RISK ANALYSIS (part of Risk assessment process)

- ARO Annual Rate of Occurence
- Asset Value (AV)
- (EF) Exposure Factor : % of the asset that is lost
- **Quantitative risk assessment** (numerical approach)
    - AV * EF  = SLE  Single Loss Expectancy
        - Laptop stolen: (AV) 1000€ * 1.0 (EF) = 1000€ (SLE)
    - ALE - Annual Lost Expectancy
        - AV * EF *ARO = ALE
- **Qualitative risk assessment**
    - impact / ARO / Cost / Overall RISK
    - traffic light approach

![image.png](image%2044.png)

- Risk Likehood approach
    - probability Vs Impact Matrix
    
    ![image.png](image%2045.png)
    

## RISK MANAGEMENT

four strategies to choose from

- risk mitigation
    - most common choice
    - set security controls to mitigate the risk
- risk avoidance
    - change business practices to completely eliminate the risk
- risk transference
    - purchasing an insurance policy that covers a risk or transfert the risk to third party
- risk acceptance
    - simply continue operations as normal in the face of the risk (conscious decision)
    - can act an exception or exemption for that risk if documented and approved
    

### Risk Tracking

- **inherent risk** facing an organization is the original level of risk
- **residual risk** is the risk that remains after an organization implements mitigation controls or transference
- **Risk Appetite** :level of risk tolerance accepted by the company  (cost of doing business)
- **Risk threshold** : specific level at which a risk becomes unacceptable (> risk appetite)
- **Risk** **tolerance** : ability for a company to withstand risks and continue operations without any significant impact ! <> risk appetite !
- Key Risk Indicators (KRIs) are metrics used to measure and provide early warning signals for increasing levels of risk

Good LEVEL of RISK = residual risk is at or below the organization's risk appetite

### Risk Register

document listing all risks and containing:

- Risk owner
- Risk threshold information
- Key Risk Indicators (KRIs)
- Risk Matrix

### Risk reporting

- formal document w/ detail information for each risk (based on risk register)
- describe risk status and evolution (Risk Trend Analysis / Risk Event Reports)

### Business Impact Analysis

The business impact analysis (BIA) is a formal process designed to
identify the mission-essential functions within an organization and
facilitate the identification of the critical systems that support those
functions.There are four key metrics used in the BIA :

- Mean Time Between Failures (MTBF) is a measure of the
reliability of a system. It is the expected amount of time that will
elapse between system failures
- Mean Time to Repair (MTTR) is the average amount of time
to restore a system to its normal operating state after a failure
- Recovery Time Objective (RTO) is the amount of time that
the organization can tolerate a system being down before it is
repaired. *(The service team is meeting expectations when the time
to repair is less than the RTO)*
- Recovery Point Objective (RPO) is the amount of data that
the organization can tolerate losing during an outage