# 4.5 Endpoint security

Created time: 15 mars 2025 19:00
Last edited by: OLB_
Last edited time: 5 avril 2025 16:19

- Control the edge (internet access)
- Access control
- posture assessment / Health check
- persistent agent / agentless / dissolvable agent (temporary)
- quarantine if assessment fails
- Allow Lists and Deny Lists (software installation)
- Antivirus / Antimalware
    - signature
    - heuristic (behavior)
    - AI /ML  (security based on a “normal” baseline)
    - sandboxing
- EDR
- XDR (add network detection, cloud services, correlate endpoints, watch data repositories)
- DLP
- HIPS
- **Secure boot** ensures that the system boots using
only software that the original equipment manufacturer (OEM) trusts.
- **Measured boot**  relies on the UEFI firmware to hash the firmware, bootloader, drivers, and anything else that is part
of the boot process creating a boot log stored in TPM. **The logs can be validated remotely** to let
security administrators know the boot state of the system. This boot attestation process allows comparison against known good states

- **TPM (Trusted Platform Module)**
    - **Remote Attestation**: Enables verification of hardware and software configurations, ensuring that a system's integrity can be validated remotely.
    - **Binding**: Encrypts data to protect it from unauthorized access, ensuring that only the intended recipient can decrypt and use the data.
    - **Sealing**: Encrypts data and sets specific requirements for the state of the TPM chip that must be met before
    decryption can occur, adding an extra layer of security by linking data access to the system's integrity.

<aside>
👉

As you prepare for the exam, keep in mind the roles that TPMs, HSMs, key management services (KMSs) and secure enclaves play in system security and organization operations. Remember that TPMs are used for system security; HSMs are used to create, store, and manage keys for multiple systems; and a KMS is a service used to manage secrets.

</aside>

- CIS (Benchmarks) -Center for Internet Security
    - configuration standards can be used as a base and modified to an
    organization's needs
- Windows Registry
    - Hardening the Windows Registry involves configuring permissions for the Registry,
    disallowing remote Registry access and limiting access to Registry tools like regedit
- Windows GPO
    - Microsoft provides the Security Compliance Toolkit (SCT)
- SELinux / Apparmor
- Config Management Tools
    - Jamf Pro / Configuration Manager for Windows / CFEngine
    - Mobile device management tools for Mobiles
- Process
    
    1- Use CIS Benchmarks for a baseline
    
    2- Deploy with GPO / Central management Tools
    
    3- Maintain with Central Management Tools
    
- Patching

**ENCRYPTION**

- Transparent FDE
- Volume Encryption