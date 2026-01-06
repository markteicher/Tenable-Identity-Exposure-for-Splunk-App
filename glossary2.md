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

### **Crown Jewel Asset**
A highly sensitive system, account, or resource whose compromise would have significant operational or security impact, such as domain controllers or privileged service accounts.

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

End of glossary section (A–Z).
