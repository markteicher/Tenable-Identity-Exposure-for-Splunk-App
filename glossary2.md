##glossary2.md
---

# Tenable Identity Exposure — Glossary of Terms (A–Z)

## A

### **Active Directory (AD)**
Microsoft directory service used to manage users, computers, groups, and authentication within a Windows domain environment. Tenable Identity Exposure analyzes Active Directory objects, relationships, configurations, and behaviors to identify identity-based attack paths and misconfigurations.

### **Active User Count**
The number of users currently enabled and active within the monitored Active Directory domains. This metric is used for licensing, exposure analysis, and monitoring abnormal user growth or reduction.

### **Attack Path**
A sequence of permissions, configurations, or relationships that allow an attacker to move from one identity or asset to another within Active Directory, potentially escalating privileges or gaining domain-wide control.

---

## B

### **Baseline**
A reference state of Active Directory configurations and identity relationships used to detect deviations over time. Baselines help identify newly introduced risks or misconfigurations.

### **Broken Inheritance**
A condition where an Active Directory object does not inherit permissions from its parent container, potentially allowing unauthorized access or privilege escalation.

---

## C

### **Compliance Score**
A numerical score (0–100) calculated by Tenable Identity Exposure based on detected deviances and their severity. The score reflects how closely the Active Directory environment aligns with security best practices.

### **Critical Indicator**
A high-severity security condition identified by Tenable Identity Exposure that represents an immediate or high-impact risk to identity security.


---

## D

### **Delegation**
An Active Directory mechanism that allows one account or service to act on behalf of another. Misconfigured delegation can enable attackers to impersonate privileged users.

### **Deviance**
Any configuration, permission, or relationship that diverges from expected or secure Active Directory practices and increases attack surface.

---

## E

### **Exposure Indicator**
A measurable condition or configuration that increases the likelihood of identity compromise, lateral movement, or privilege escalation.

---

## F

### **Forest**
A collection of one or more Active Directory domains that share a common schema, configuration, and trust relationships. Tenable Identity Exposure can analyze risks across single or multiple forests.

---

## G

### **Group Membership Explosion**
A condition where users or service accounts are members of an excessive number of groups, increasing the likelihood of unintended privilege inheritance.

---

## H

### **High-Privilege Account**
Any account with administrative or elevated permissions, such as Domain Admins, Enterprise Admins, or accounts with delegated control over critical objects.

---

## I

### **Indicator of Exposure (IoE)**
A classification used by Tenable Identity Exposure to describe identity-related security weaknesses that could be exploited by attackers.

### **Indicator of Attack (IoA)**
A detected behavior or condition suggesting an active or imminent identity-based attack, such as suspicious privilege escalation patterns.

---

## J

### **Junction Point Abuse**
A technique where attackers exploit directory object links or permissions to redirect access or escalate privileges.

---

## K

### **Kerberos Delegation**
A Kerberos feature allowing services to authenticate on behalf of users. Improper configuration can allow attackers to impersonate high-privilege identities.

---

## L

### **Lateral Movement**
The process by which an attacker moves from one compromised identity or system to others within the environment.

---

## M

### **Managed Account**
An account that is monitored, governed, and periodically reviewed for permissions and usage within Active Directory.

---

## N

### **Native Administrator**
Built-in administrative accounts within Active Directory that possess elevated privileges by default.

---

## O

### **Organizational Unit (OU)**
A container within Active Directory used to organize users, groups, and computers, often with delegated administrative permissions.

---

## P

### **Privileged Access**
Access rights that allow modification of security-sensitive objects or configurations.

---

## Q

### **Quarantine State**
A condition where an account or object is isolated due to detected risk or abnormal behavior.

---

## R

### **Risk Level**
A severity classification assigned to an exposure or indicator, typically ranging from low to critical.

---

## S

### **SDProp**
Security Descriptor Propagator, a Windows mechanism that enforces protected permissions on privileged groups. Misalignment can expose sensitive accounts.

---

## T

### **Trust Relationship**
A connection between Active Directory domains or forests allowing authentication across boundaries.

---

## U

### **Unconstrained Delegation**
A high-risk Kerberos configuration that allows a service to impersonate users to any service.

---

## V

### **Vulnerability Window**
The time period during which an identity-related weakness exists before remediation.

---

## W

### **Weak Permissions**
Overly permissive access controls that allow unauthorized actions on identity objects.

---

## X

### **Cross-Domain Attack Path**
An attack path that spans multiple Active Directory domains or forests.

---

## Y

### **Yellow Indicator**
A medium-severity exposure requiring attention but not representing immediate compromise.

---

## Z

### **Zero-Day Exposure**
An identity-related weakness that is newly discovered and not yet widely mitigated.

---

# Tenable Identity Exposure — Glossary (Working Draft)

## Attack Path
**Attack Path**  
Shows the possible paths that an attacker can take to compromise an asset from an entry point.

---

## Asset Exposure
**Asset Exposure**  
Shows all paths that can potentially take control of an asset.

---

## Exposure Signal
**Exposure Signal**  
An Exposure Signal is a combination of risks that could make any weakness potentially dangerous to the organization.  
An exposure signal is identified when multiple weaknesses coexist on an asset, increasing the likelihood of exploitation.

**Example conditions contributing to an Exposure Signal include:**
- Privileged access to a business-critical application
- Unpatched vulnerabilities on the asset
- A device not covered by endpoint protection

When combined, these weaknesses indicate that the asset represents a significant risk to the organization.

---

## Indicator of Exposure (IoE)
**Indicator of Exposure (IoE)**  
A security indicator representing a misconfiguration, risky setting, or weakness in Active Directory that could contribute to an attack path.

---

## Indicator of Attack (IoA)
**Indicator of Attack (IoA)**  
A signal representing malicious activity or behavior detected within Active Directory that indicates an active or attempted attack.


---

## Compliance Score
**Compliance Score**  
A calculated score ranging from 0 to 100 that represents the security posture of the environment, based on the number of detected deviances and their severity levels.

---

## Active User Count
**Active User Count**  
The number of Active Directory users currently considered active within the monitored domain or forest.

---

## Privileged Account
**Privileged Account**  
An account with elevated permissions in Active Directory, including administrative or delegated rights that can affect security posture.

---

## Native Administrator
**Native Administrator**  
A built-in Active Directory administrative account with default high-level privileges.

---

## Kerberos Delegation
**Kerberos Delegation**  
A configuration that allows a service to impersonate a user when accessing resources, which can become dangerous if misconfigured.

---

## Dangerous Kerberos Delegation
**Dangerous Kerberos Delegation**  
A Kerberos delegation configuration identified as risky because it could allow attackers to impersonate users or escalate privileges.

---

## SDProp
**SDProp**  
A mechanism in Active Directory that periodically enforces security descriptors on protected objects.

---

## SDProp Consistency
**SDProp Consistency**  
The state where security descriptors on protected objects are correctly enforced and aligned with expected configurations.

---

## Domain Controller
**Domain Controller**  
A server that hosts Active Directory Domain Services and is responsible for authentication, authorization, and directory services.

---

## Domain Controller Managed by Illegitimate User
**Domain Controller Managed by Illegitimate User**  
A condition where a domain controller is administered by an account that should not have management privileges.

---

## Risk Criticality
**Risk Criticality**  
A classification that represents the potential impact and exploitability of a detected risk.

---

## User Category
**User Category**  
A classification of users based on attributes such as role, privilege level, or behavior.

---

## User Monitoring
**User Monitoring**  
Tracking changes and activity related to Active Directory users, including creation, modification, and privilege changes.

---

## Administrative Account Monitoring
**Administrative Account Monitoring**  
Monitoring focused on accounts with administrative privileges to detect risky configurations or behaviors.

---

## Risk Evolution
**Risk Evolution**  
The progression of detected risks within the environment over time, used for trend analysis.

---

## Exposure Path
**Exposure Path**  
A chain of relationships and configurations that could allow an attacker to move through Active Directory to reach a target.

---

## Business-Critical Asset
**Business-Critical Asset**  
An asset identified as essential to business operations, where compromise would have significant impact.

---

## Endpoint Coverage
**Endpoint Coverage**  
The presence or absence of endpoint security controls on devices monitored by Tenable Identity Exposure.

---

## Management Plane
**Management Plane**  
The administrative control surface of Active Directory where configuration and privilege changes occur.

---

## Identity Risk
**Identity Risk**  
Risk associated with user identities, credentials, permissions, and authentication mechanisms.

---

## Privilege Escalation Path
**Privilege Escalation Path**  
A sequence of misconfigurations or relationships that could allow a user to gain higher privileges.

---

## Exposure Surface
**Exposure Surface**  
The total set of identity-related weaknesses that could be exploited in the environment.

---

## Remediation Recommendation
**Remediation Recommendation**  
Guidance provided by Tenable Identity Exposure to resolve a detected deviance or reduce risk.

---

## Risk Indicator
**Risk Indicator**  
A measurable signal used to identify potential security weaknesses or attack opportunities.

---

## Forest
**Forest**  
The highest-level Active Directory container that can include multiple domains sharing trust relationships.

---

## Domain
**Domain**  
A logical grouping of users, computers, and resources within an Active Directory forest.

---

## Trust Relationship
**Trust Relationship**  
A configuration that allows users in one domain or forest to access resources in another.

---

## Exposure Analysis
**Exposure Analysis**  
The process of evaluating identity data to identify attack paths, exposure signals, and risks.


### ACL changed
Modification to the Access Control List of an Active Directory object that changes permissions assigned to users or groups.

### SPN changed
Modification to an existing Service Principal Name associated with an account, affecting Kerberos service authentication mapping.

### Member removed
Removal of a user, computer, or group from an Active Directory group.

### New member
Addition of a user, computer, or group to an Active Directory group.

### New trust
Creation of a trust relationship between domains or forests enabling cross-domain authentication.

### Unknown file type added
Addition of a file with an unrecognized or unsupported file type to a monitored location.

### New object
Creation of a new Active Directory object such as a user, group, computer, organizational unit, or policy object.

### Object removed
Deletion of an existing Active Directory object.

### Password changed
Successful change of a password for a user or service account.

### UAC changed
Modification to User Account Control flags that alter account behavior or privilege characteristics.

### New GPO linked
Linking of a Group Policy Object to a site, domain, or organizational unit.

### GPO link removed
Removal of a Group Policy Object link from a site, domain, or organizational unit.

### Owner change
Change of ownership for an object, transferring control and permission authority.

### File renamed
Change to the name of a file without modifying its contents.

### SPN created
Creation of a new Service Principal Name for an account to support Kerberos authentication.

### Failed authentication reset
Unsuccessful attempt to reset authentication failure counters.

### Failed authentication
Unsuccessful authentication attempt due to invalid credentials or policy restrictions.


## TLS requirements
Minimum Transport Layer Security version and configuration required to secure communications between Tenable Identity Exposure components.

## Cipher Suites
Approved cryptographic algorithms used to establish secure TLS connections.

## Secure Relay
A hardened communication component that securely transfers identity data from on-premises environments to Tenable Identity Exposure.

## Cryptographic settings
Configuration parameters governing encryption, hashing, and key management used by the platform.

## Virtual machine requirements
Hardware and software specifications required to deploy Tenable Identity Exposure components on virtual machines.

## Allowed files and processes
List of files and executable processes permitted to run for Tenable Identity Exposure components.

## SAML
Security Assertion Markup Language used for federated authentication to the Tenable Identity Exposure platform.

## Tenable Identity Exposure account
A tenant-level account representing an organization within Tenable Identity Exposure.

## Tenable Identity Exposure User Portal
The web-based interface used to access dashboards, investigations, and remediation guidance.

## Trusted Certificates
Digital certificates trusted by Tenable Identity Exposure to validate encrypted communications.

## Tenable Identity Exposure Insights
Contextual risk intelligence and recommendations derived from identity exposure analysis.

## Prioritization and Remediation
Workflow that ranks identity risks and provides guidance to reduce exposure.

## Top Risks
Highest-priority identity-related risks detected in the environment.

## Exposure Signals
A combination of correlated weaknesses that collectively represent a significant identity risk.

## If You Have 5 Minutes
A curated view highlighting the most critical actions requiring immediate attention.

## Demographics
Statistical breakdown of identities, accounts, and roles within the environment.

## Finding Trends
Historical analysis showing how identity risks evolve over time.

## Exposure Center Overview
Centralized view summarizing identity exposure posture across environments.

## Exposure Instance Details
Detailed information about a specific detected exposure.

## Asset Criticality Rating (ACR)
Score representing the business importance of an asset.

## Remediation Cost
Estimated effort or impact required to remediate a finding.

## Finding details
Granular information describing a specific security finding.

## Asset details
Information describing an asset involved in an exposure or attack path.

## Weakness details
Technical attributes explaining why a weakness exists.

## Remediation
Actions recommended to reduce or eliminate identified risks.

## Identity 360 — Comprehensive Identity Risk Management
Unified view of identities, relationships, risks, and remediation paths.

## Accounts
User, service, or computer accounts within Active Directory or connected identity systems.

## Devices
Endpoints or systems associated with identities.

## Weaknesses
Security conditions that increase the likelihood of compromise.

## Entitlements
Privileges or permissions granted to identities.

## Roles
Defined sets of permissions assigned to identities.

## Groups
Collections of accounts used to manage permissions.

## Access
Effective permissions an identity has over resources.

## Exposure Card
Visual representation summarizing exposure context and severity.

## Relationships
Connections between identities, devices, permissions, and resources.

## Trail Flow Table
Chronological representation of identity-related events and changes.

## IoE
Indicator of Exposure identifying a risky configuration or condition.

## Event
Recorded change or activity observed in the identity environment.

## Deviant Object
An object whose configuration deviates from expected security baselines.

## Attribute "ntsecuritydescriptor"
Active Directory attribute defining permissions and access control.

## Indicators of Exposure
Rules identifying misconfigurations or risky identity conditions.

## Level of Severity
Classification indicating the potential impact of a finding.

## Deviance Resolution
Process of correcting a deviating configuration.

## Detection Date
Timestamp indicating when an exposure was identified.

## Indicator of Exposure Details
Detailed context explaining why an indicator was triggered.

## Deviant Objects
Set of objects affected by a specific exposure.

## Incriminating Attributes
Attributes contributing directly to a detected risk.

## RSoP-Based Indicators of Exposure
Indicators derived from Resultant Set of Policy analysis.

## Enhancements
Improvements or additional capabilities introduced to exposure detection.

## Benefits
Security and operational advantages gained by using Tenable Identity Exposure.

## Technical Aspects
Underlying architectural and functional components of the platform.

## Remediate Deviances from Indicators of Exposure
Guided actions to correct detected deviations.

## AdminCount Attribute Set on Standard Users
Condition where non-admin accounts inherit protected admin privileges.

## Dangerous Kerberos Delegation
Misconfigured delegation enabling credential abuse.

## Ensure SDProp Consistency
Verification that protected object permissions are correctly enforced.

## Indicators of Attack
Signals indicating active or attempted identity compromise.

## Indicator of Attack Details
Contextual information explaining an attack indicator.

## Indicators of Attack Incidents
Correlated attack indicators grouped as incidents.

## Incident Details
Comprehensive information about a detected security incident.

## Attack Details
Technical explanation of how an attack is performed.

## YARA Detection Rules
Pattern-matching rules used to detect malicious activity.

## Attack Path
Sequence of actions an attacker could take to reach a target asset.

## Blast Radius
Scope of impact if an attack path is successfully exploited.

## Asset Exposure
Extent to which an asset can be compromised via attack paths.

## Attack Relations
Relationships between identities, permissions, and attack techniques.

## Add Member
Action adding an account to a group.

## Exploitation
Abuse of a weakness to gain unauthorized access.

## Allowed To Act
Permission allowing an identity to act on behalf of another.

## Allowed to Act Description
Explanation of delegated action capability.

## Allowed to Act Exploitation
Abuse of delegated permissions for privilege escalation.

## Allowed to Act Remediation
Steps to remove unsafe delegated permissions.

## Allowed To Delegate
Permission enabling delegation of credentials.

## Allowed To Description
Explanation of delegation capability.

## Allowed To Exploitation
Abuse of delegation permissions.

## Allowed To Remediation
Steps to correct unsafe delegation.

## Belongs To GPO
Relationship between an object and a Group Policy Object.

## Belongs To Description
Explanation of GPO linkage.

## Belongs To Exploitation
Abuse of GPO linkage for privilege escalation.

## Belongs To Remediation
Steps to correct insecure GPO associations.

## DCSync
Technique allowing replication of directory secrets.

## DCSync Description
Explanation of directory replication abuse.

## DCSync Exploitation
Use of replication rights to extract credentials.

## DCSync Remediation
Actions to remove unauthorized replication permissions.
