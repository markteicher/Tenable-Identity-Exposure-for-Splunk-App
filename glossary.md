# Tenable Identity Exposure — Glossary

This glossary defines key terms used within **Tenable Identity Exposure** (formerly Alsid).  
It is intended to support **operators, security engineers, and Splunk app users**, not marketing audiences.

---

## Active Directory (AD)
Microsoft directory service used for authentication, authorization, and identity management across Windows environments.

---

## Attack Path
A sequence of relationships, permissions, and configurations that allow an attacker to move from one identity or system to another within Active Directory.

---

## Compliance Score
A score from **0–100** calculated by Tenable Identity Exposure based on:
- Number of detected deviances
- Severity of each deviance  
This score reflects **directory hygiene**, not real-time attack likelihood.

---

## Container
A logical grouping of objects in Active Directory, such as users, groups, or computers (e.g., Organizational Units).

---

## Data Collector (Relay)
A deployed component that connects to Active Directory to collect identity, permission, and configuration data.  
Equivalent to **BloodHound data collectors**.

---

## Deviance
Any configuration, permission, or behavior that deviates from security best practices or increases attack surface.

---

## Domain
A logical boundary in Active Directory that defines a set of users, computers, and policies managed together.

---

## Domain Controller (DC)
A server that authenticates users and enforces security policies within an Active Directory domain.

---

## Exposure Indicator (Indicator of Exposure)
A categorized security condition representing a specific type of identity risk (e.g., dangerous delegation, excessive privileges).

---

## Identity Exposure
The degree to which identities, permissions, or configurations in Active Directory increase the risk of compromise.

---

## Identity Relationship
A trust, permission, or delegation relationship between identities or systems (e.g., group membership, ACLs).

---

## Indicator of Attack (IOA)
A detected behavior or condition that may indicate malicious activity or attack progression within Active Directory.

---

## Kerberos Delegation
A mechanism that allows a service to impersonate a user to access another service.  
Misconfigurations can enable lateral movement and privilege escalation.

---

## Native Administrator
Built-in privileged accounts in Active Directory (e.g., Domain Admins, Enterprise Admins).

---

## Privileged Account
Any account with elevated permissions that can modify AD objects, policies, or security settings.

---

## Relay
Tenable terminology for the **Data Collector** used to ingest Active Directory data.

---

## Risk
A condition where identity configuration or permissions could be abused by an attacker.  
Risk does **not** necessarily mean exploitation has occurred.

---

## SDProp (Security Descriptor Propagator)
A mechanism that enforces permissions on protected Active Directory objects.  
Misconfiguration can result in privilege persistence.

---

## Security Principal
An identity object that can be authenticated and assigned permissions (users, groups, computers).

---

## Trust
A relationship between domains or forests that allows authentication across boundaries.

---

## User Category
A classification of users based on role or behavior (e.g., standard user, privileged user, service account).

---

## Privilege Escalation
The act of gaining higher-level permissions than originally assigned, often through misconfigurations.

---

## Lateral Movement
Movement by an attacker from one system or identity to another within Active Directory.

---

## Forest
A collection of one or more Active Directory domains that share a common schema and trust relationships.

---

## Least Privilege
Security principle where identities are granted only the permissions necessary to perform their function.

---

## Attack Surface
The total set of identity relationships, permissions, and configurations that could be exploited.

---

## Delegation Abuse
Exploitation of Kerberos delegation settings to impersonate users or services.

---

## Privileged Path
A chain of relationships that leads from a low-privileged identity to a high-privileged identity.

---

## Operational Visibility
The ability to continuously observe identity state, changes, and risk within Active Directory.

---

## Identity Graph
A representation of identities and their relationships used to analyze attack paths and exposure.

---

## Exposure Evolution
Tracking how identity risks and deviances change over time.

---

## Remediation
Actions taken to reduce or eliminate identity risks (e.g., removing excessive privileges).

---

## Administrative Scope
The range of objects and permissions an administrator can control.

---

## Misconfiguration
An incorrect or insecure Active Directory setting that increases risk.

---

## Service Account
An account used by applications or services, often with elevated permissions.

---

## Identity Drift
Gradual accumulation of permissions or misconfigurations over time.

---

## Attack Readiness
The degree to which identity infrastructure is prepared to resist real-world attacks.

---

## Auditability
The ability to examine identity configuration, permissions, and changes for review or compliance purposes.

---

## Zero Trust (Contextual)
A security model emphasizing verification and minimal trust, not natively enforced by AD but relevant to identity risk analysis.

---

## Data Freshness
How recent the collected identity data is relative to the current AD state.

---

## Detection Coverage
The breadth of identity risks and misconfigurations that the platform can identify.

---

## Operational Maturity
The ability of an organization to consistently manage identity risk using people, process, and technology.

---
