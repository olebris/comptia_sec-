# 2.3 Race conditions

Created time: 29 décembre 2024 18:52
Last edited by: OLB_
Last edited time: 27 mars 2025 23:35

- Based on timing
    - doing the same action multiple times before check/validation
- TOCTTOU Attacks
    - Time-of-check to time-of-use
    - something might happen between the check and the use
    - A Time-of-Check-to-Time-of-Use (TOCTTOU or TOC/TOU) issue is a
    type of race condition that occurs when a program checks access
    permissions too far ahead of a resource request.
- Time-of-Check (TOC) is the instance when a system verifies access
permissions or other security controls.
- Time-of-Use (TOU) is the moment when the system accesses the
resource or uses the permission that was granted.
- The Target of Evaluation (TOE) refers to the particular
component, system, or mechanism being evaluated or tested for
potential vulnerabilities, such as the system's method of
managing and validating access permissions.

<aside>
👉

If the systems administrator revokes a particular permission, that restriction would not be applied to the user until the next time they log on. If the user is logged on
when the access revocation takes place, they will have access to the resource indefinitely. The user simply needs to leave the session open for days, and the new restrictions will never be applied. To prevent this race condition, the developer should evaluate access permissions at the time of each request rather than caching a listing of permissions

</aside>