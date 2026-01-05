# Identity Exposure Coverage Matrix  
**Tenable Identity Exposure vs BloodHound (Enterprise)**

| Capability / Domain                                   | Tenable Identity Exposure (Alsid) | BloodHound (Enterprise) | Notes |
|------------------------------------------------------|----------------------------------|--------------------------|-------|
| **Data Collection Model**                             | Relay-based (agent / service)    | Native graph ingestion   | TIE requires infrastructure relays |
| **AD Object Graph Modeling**                          | ⚠ Partial                         | ✔ Full                   | BloodHound is graph-native |
| **Attack Path Analysis**                              | ⚠ Abstracted                     | ✔ Explicit                | BH shows real privilege paths |
| **Privilege Escalation Paths**                        | ⚠ High-level signals             | ✔ Exact edges             | BH exposes concrete attack chains |
| **Delegation Abuse Detection**                        | ✔ Yes                             | ✔ Yes                    | BH provides deeper context |
| **Kerberos Abuse (DCSync, RBCD, etc.)**               | ⚠ Limited                        | ✔ Full                   | BH maps abuse primitives directly |
| **ACL / ACE Resolution**                              | ⚠ Simplified                     | ✔ Exhaustive              | BH resolves effective permissions |
| **Trust Relationship Mapping**                        | ⚠ Partial                        | ✔ Full                   | BH models transitive trust paths |
| **Group Nesting Depth Analysis**                      | ⚠ Limited                        | ✔ Unlimited               | BH resolves deep nesting |
| **Shadow Admin Detection**                            | ✔ Yes                             | ✔ Yes                    | BH shows *how* it happens |
| **Tiering / Security Boundary Awareness**             | ⚠ Opinionated                    | ✔ Model-driven            | BH does not impose vendor bias |
| **Risk Scoring Transparency**                         | ❌ Opaque                         | ✔ Transparent             | BH scoring is explainable |
| **Raw Data Export (Full Fidelity)**                   | ❌ CSV only                       | ✔ Graph / JSON            | TIE loses graph semantics |
| **API Coverage**                                      | ⚠ Limited                        | ✔ Extensive               | BH Enterprise exposes graph APIs |
| **Non-Admin Consumption (Executives)**                | ❌ No                             | ⚠ With tooling            | Neither is exec-ready OOTB |
| **SOC / SIEM Integration**                            | ⚠ CSV / PowerBI recommended      | ✔ Native Splunk apps      | BloodHound Splunk app exists |
| **Historical State Comparison**                       | ⚠ Limited                        | ✔ Full                    | BH supports temporal analysis |
| **Change Impact Analysis**                            | ⚠ Signal-based                   | ✔ Graph-delta             | BH shows what changed and why |
| **Explainability (“Why is this risky?”)**             | ❌ Minimal                        | ✔ Explicit path           | Key executive failure in TIE |
| **Vendor Lock-in**                                    | ✔ High                           | ⚠ Moderate                | BH graph can be reused |
| **Licensing Cost vs Insight Depth**                   | ❌ Poor                           | ✔ Strong                  | TIE heavily marketed |
| **Designed for Practitioners**                        | ❌ No                             | ✔ Yes                     | BH built by operators |
| **Marketing vs Technical Accuracy**                   | ❌ Marketing-led                 | ✔ Reality-led             | Central philosophical gap |
