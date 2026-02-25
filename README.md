# Foundations Lab Final  
## The Professional Identity & Workbench

**Author:** Leigh Pritchett  
**Institutional Affiliation:** The Knowledge House    
**Course:** Foundations Portfolio  
**Instructor:** George Robbins  
**Date:** February 23, 2026  

---

### Abstract/Executive Summary
This repository serves as the primary technical workbench and version-controlled portfolio for the Knowledge House 2026 Cybersecurity Cohort Foundations Intensive. This initial commit establishes the technical environment using Git version control and VS Code integration.

---

### Professional Introduction
I am a transitioning professional dedicated to mastering the technical and ethical requirements of the 2026 cybersecurity landscape. My specialization focus will be digital forensics and red teaming.

### Cybersecurity Focus: Red Teaming & Digital Forensics
My professional trajectory is centered on the dual-disciplines of offensive security and post-incident reconstruction. 

* **Red Teaming:** I am focused on mastering adversarial tactics, techniques, and procedures (TTPs) to identify systemic vulnerabilities before they can be exploited by malicious actors.
* **Digital Forensics:** Complementing my offensive interest, I am developing skills in host and network forensics to perform deep-dive analysis of security breaches, ensuring evidence integrity and comprehensive root-cause identification.

### References
MITRE. (2024). *MITRE ATT&CK®*. https://attack.mitre.org/

---

### Security Foundations: Governance & Frameworks
**The CIA Triad:**

The CIA triad is a foundational model consisting of **Confidentiality, Integrity, and Availability**.

* **Confidentiality** ensures that sensitive information is accessible only to those with legitimate authorization.

* **Integrity** guarantees that data is true, verified, and has not been altered by unauthorized sources.

* **Availability** ensures that systems and data are consistently accessible to authorized users upon demand.

**The AAA Framework**

The AAA framework—**Authentication, Authorization, and Accounting**—defines the process for controlling access to network resources.

* **Authentication** verifies the identity of a user or entity.

* **Authorization** determines the specific level of access granted to that identified entity.

* **Accounting** involves tracking and logging the actions taken by a user during their session for audit purposes.

**The Impact of Governance on Cybersecurity Roles**

Governance provides the necessary oversight and strategic framework for cybersecurity roles within an institution. It ensures that security practitioners operate within established policies to maintain organizational compliance. Effective governance prevents individuals and entities from violating internal company standards as well as broader state and federal regulations, such as HIPAA or GDPR.

### References

International Organization for Standardization. (2018). *Information technology — Security techniques — Information security management systems — Overview and vocabulary* (ISO/IEC Standard No. 27000:2018). https://www.iso.org/standard/73906.html  

National Institute of Standards and Technology. (2014). *An introduction to information security* (NIST Special Publication 800-12 Revision 1). U.S. Department of Commerce. https://doi.org/10.6028/NIST.SP.800-12r1

---

### **Security Philosophy and Reflection: The Intersections of Governance and Technical Skill**  

Governance is just as vital as technical skill in Cybersecurity because it provides oversight of the legal and ethical boundaries technical tools must operate within. Therefore, my security philosophy is that proficiency in technical skills should be guided by Governance in order to properly represent the core pillars of the CIA Triad:  

* **Confidentiality:** Pertains not only to encryption but also to determining who has access to sensitive information.  

* **Integrity:** Should utilize rigorous scrutiny to make sure that data remains trustworthy and unaltered by bad actors.  

* **Availability:** Is maintaining the reliability and resilience of the system against attacks and accidents.   

Today’s material aligns most closely with the Governance, Risk, and Compliance (GRC) domain. This domain creates the "playbook" that technical teams follow to ensure their work is documented, authorized, and reproducible.  Without a strong governance framework, misused technical skills can lead to liability or data loss. Understanding why security protocols are implemented allows me to be a more effective practitioner in both offensive and investigative roles.  

### References  

National Institute of Standards and Technology. (2014). *An introduction to information security* (NIST Special Publication 800-12 Revision 1). U.S. Department of Commerce. https://doi.org/10.6028/NIST.SP.800-12r1  

MITRE. (2024). *ATT&CK Matrix for Enterprise*. https://attack.mitre.org/matrices/enterprise/  

---

### **Lab Infrastructure & Virtualization Setup**  

A hypervisor is a software that sits as a layer on top of the physical host of the source CPU, ram and network.  It divides those resources up to virtualize them into individual virtual machines, or guests of the host machine, to create distinct virtual servers that are isolated to only see what data it needs to be seen.  Additionally, the other virtual servers are isolated from each other.  The hypervisor provides the security necessary to make that separation possible.

Virtual machines are simply put, an entirely separate computer created by software that has been created on your physical computer, sometimes supported by an operating system and allocated a portion of the resources.  In this case the resources are shared by the operating system hosting it.  In other cases, the virtual machine is installed directly on the physical hardware, called a barebones or bare metal installation and in that case the virtual machine has direct access to the resources rather than a shared allocation.

In cyber security, isolation is important regarding virtual machines for a variety or reasons.  one reason is that virtual machines are often used as testing environments.  Keeping those testing environments isolated prevents the machine hosting them form becoming compromised by any experimentation being done.  Isolation is also a key security issue when it comes to preventing unauthorized access between machines that may be being used by different people or departments in an organization.  It prevents those that don't have the right to access possible sensitive information from seeing what is going on in the virtual machine that is on the same system because of the barriers that are in place as part of the hypervisor's programming.

It is because of the isolation aspect of VMs that the CIA Triad can be effectively implemented in this way:  

* *Confidentiality* is assured as each virtual machine is kept separate by the hypervisor software  

* *Integrity* is kept due to this isolation preventing the outside alteration of the other virtual machines that may be on the shared host system  

* *Availability* is maintained in other isolated machines if one or more virtual machines should go offline for any reason, preventing the entire system from going down  

### References  

Red Hat. (n.d.). *What is a virtual machine?*  
https://www.redhat.com/en/topics/virtualization/what-is-a-virtual-machine  

National Institute of Standards and Technology. (2011). *Guide to Security for Full Virtualization Technologies* (NIST Special Publication 800-125). U.S. Department of Commerce.  

---

### **Reflection:**  

As previously stated, isolation is an essential part of security, especially when it comes to working with an environment where there is testing being done.  This isolation prevents any possible "bleed over" of malicious code to the host machine that is providing the environment for the virtual machines.  This makes the experimentation possible without the concern of possibly corrupting any important files or making it so that you will need to wipe your system to be sure that you have removed anything malicious that may have gotten onto your host system.  Instead you can just refresh your virtual machine the create a whole new clean working environment.  I feel that the concept of isolation complies mostly with the **Risk Management** aspect of the **GRC** as this pertains to the assessment, management and mitigation of any risks.  

