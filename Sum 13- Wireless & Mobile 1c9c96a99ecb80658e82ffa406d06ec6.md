# Sum: 13- Wireless & Mobile

Created time: 2 avril 2025 19:57
Last edited by: OLB_
Last edited time: 2 avril 2025 20:03

<aside>
👉

Building a secure network starts with an understanding of the wireless
connectivity options that organizations may choose to deploy. Wi-Fi,
cellular, and Bluetooth are found almost everywhere and are key to
how organizations connect devices and systems. Knowing which
technologies are in play and how they connect devices is the first part
of designing and securing your network.

Understanding common attacks against wireless networks and devices
helps security professionals to design a wireless network. Network
design is conducted and installation considerations are considered,
including using site surveys to understand the environment that the
network will be deployed into. Heatmaps show signal propagation and
can help with device placement. How you will protect your controllers
and access points also comes into play, with concerns ranging from
patching and maintenance to secure remote access via protected
channels or networks.

Once a network is designed, security and authentication options are
the next layer in your design. WPA3 provides simultaneous
authentication of equals (SAE) as well as enterprise models that
connect to RADIUS servers to allow the use of organizational
credentials. Authentication protocols like EAP and its many variants
allow choices based on what your hardware supports and what specific
authentication choices you need to make.

Finally, mobile devices must be secured. Deployment models range
from BYOD processes that let users bring their own devices to entirely
corporate-owned models that deploy locked-down devices for specific
purposes into your end users' hands. Devices also need to be managed,
which is where tools for mobile device management come into play.
They provide a broad range of features you need to be aware of as a
security professional.

**Modern enterprises rely on many types of wireless
connectivity**. There are many wireless connectivity options for
organizations and individuals. Devices may connect via cellular
networks, which place the control of the network in the hands of
cellular providers. Wi-Fi is widely used to connect devices to
organizational networks at high speed, allowing ease of mobility while
providing security using enterprise security protocols. Bluetooth
provides connectivity between many devices and cellular is used to
provide access from mobile devices and systems that can't connect to
Wi-Fi or wired networks.

**Secure wireless network designs take existing networks and
physical spaces into account.** Site surveys include physical tours
of a facility using tools that can identify existing wireless networks and
access points as well as signal strengths and other details that help
map the location. Network designs take into account channel spacing,
access point placement, and even the composition of the building
when placing access points.

**Cryptographic and authentication protocols provide
wireless security.** Both WPA2 and WPA3 are used in modern Wi-Fi
networks. These protocols provide for both simple authentication
protocols, like WPA2's preshared key mode, and for enterprise
authentication models that rely on RADIUS servers to provide user
login with organizational credentials. Both rely on cryptographic
protocols to encrypt data in transit. Devices are frequently configured
to use a variant of the Extensible Authentication Protocol (EAP) that
supports the security needs of the organization and that is supported
by the deployed wireless devices.

**Understand mobile device vulnerabilities**. Sideloading involves
copying programs from an external device or system, allowing them to
be added to a device and potentially bypassing the device's application
store. Jailbreaking provides root access to devices providing greater
control but also creating security concerns because it bypasses the
device's native security model.

**Securing underlying wireless infrastructure requires strong
network device administration and security practices.**
Wireless controllers and access points must be protected, and
installation considerations are important to consider for wireless
devices. Like other network devices, controllers and APs need to be
regularly patched and updated and must be configured securely. They
also must have protected administrative interfaces and should be
configured to log and report on the network, their own status, and
security issues or potential problems. Heatmaps and site surveys help
administrators understand the environment they are deploying into
and operating in.

**Managing mobile devices relies on both deployment
methods and administrative tools**. Deployment methods include
bring your own device; choose your own device; corporate-owned,
personally enabled; and corporate owned, business only. The risks and
rewards for each method need to be assessed as organizations choose
which model to deploy their devices in. Once that decision is made,
tools like mobile device management or unified endpoint management
can be used to configure, secure, manage, and control the devices in a
wide range of ways, from deploying applications to securely wiping
devices if they are lost or stolen. You need to understand the
capabilities and limitations of MDM and UEM products as well as the
devices and operating systems that they can manage.

</aside>

## **EXAM CHECK**

THE COMPTIA SECURITY+ EXAM OBJECTIVES
COVERED IN THIS CHAPTER INCLUDE:

Domain 2.0: Threats, Vulnerabilities, and Mitigations
2.3. Explain various types of vulnerabilities.

- Mobile device (Side loading, Jailbreaking)

Domain 3.0: Security Architecture
3.3. Compare and contrast concepts and strategies to
protect data.

- General data considerations (Geolocation)

Domain 4.0: Security Operations
4.1. Given a scenario, apply common security techniques to
computing resources.

- Hardening targets (Mobile devices, Workstations,
Switches, Routers, Cloud infrastructure, Servers,
ICS/SCADA, Embedded systems, RTOS, IoT devices).
- Wireless devices (Installation considerations (Site
surveys, Heat maps))
- Mobile solutions (Mobile device management (MDM),
Deployment models (Bring your own device (BYOD),
Corporate-owned, personally enabled (COPE), Choose
your own device (CYOD)), Connection methods
(Cellular, Wi-Fi, Bluetooth))
- Wireless security settings (Wi-Fi Protected Access 3
(WPA3), AAA/Remote Authentication Dial-in User
Service (RADIUS), Cryptographic protocols,
Authentication protocols)