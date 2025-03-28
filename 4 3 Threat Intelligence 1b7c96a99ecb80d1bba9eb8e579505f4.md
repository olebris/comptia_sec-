# 4.3 Threat Intelligence

Created time: 15 mars 2025 15:17
Last edited by: OLB_
Last edited time: 22 mars 2025 13:46

Threat intelligence is the set of activities and resources available to cybersecurity professionals seeking to learn about changes in the threat environment

Threat intelligence information can also be used for **predictive analysis** to identify likely risks to the organization

- CTI
    - Research Threats and Threat Actors
    - Prevention and Information to make decisions
- OSINT
    - public info on Internet / public data / Social networks ..
- Commercial services: Third party Intelligence service
    - collect and sell CTI data
    - also called “closed-source intelligence”
- Sharing CTI data
    - Cyber Threat Alliance (CTA)
- Dark Web
    - overlay Network over Internet
    - hacking groups
    - Forum to watch
- CTI: Provide Threat feeds with IoCs (Indicators of Compromise)
    - IP
    - Hostnames / domains
    - emails addresses
    - URL
    - file path
    - file hash
    - CVE
    - Other IoC (log patterns,file hash ..)
- CTI: build a vulnerability database

[https://www.senki.org/operators-security-toolkit/open-source-threat-intelligence-feeds](https://www.senki.org/operators-security-toolkit/open-source-threat-intelligence-feeds)

[https://www.misp-project.org/feeds/](https://www.misp-project.org/feeds/)

[https://threatmap.checkpoint.com/](https://threatmap.checkpoint.com/)

### Threat intelligence assessment

- Is information on time / timely ?
- Is the info accurate ?
- is the info relevant to the organization?

⇒ build a confidence score 

- discredited
- improbable
- doubtful
- possible
- probable
- confirmed$

### Threat Intelligence management and Exchange

- Standards for describe a CTI Object
    - STIX (XML or JSON )
    - OpenIOC

```bash
#STIX
{
"type": "threat-actor",
"created": "2019-10-20T19:17:05.000Z",
"modified": "2019-10-21T12:22:20.000Z",
"labels": [ "crime-syndicate"],
"name": "Evil Maid, Inc",
"description": "Threat actors with access to hotel rooms",
"aliases": ["Local USB threats"],
"goals": ["Gain physical access to devices", "Acquire data"],
"sophistication": "intermediate",
"resource:level": "government",
"primary_motivation": "organizational-gain"
}
```

Exchange protocol (over HTTPS) ⇒ TAXII

[https://oasis-open.github.io/cti-documentation/](https://oasis-open.github.io/cti-documentation/)

### Information Sharing Organizations

- Information Sharing and Analysis Centers (ISACs)
- communities to assist members and provide tools
- ISACs
    - by sector (finance, energy, avaition…)
    - provide CTI feeds, alert, tools, Incident response help

![image.png](image%2028.png)

**Other source for CTI**

- vendors product site
- RFC Request for Comments
- Social media accounts of ptominent security professionnals