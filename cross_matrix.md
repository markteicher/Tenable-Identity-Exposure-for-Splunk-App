```mermaid
flowchart LR

%% Columns
subgraph COL1["Capability"]
    C1["Data Collection Method"]
    C2["Deployment Model"]
    C3["Data Ownership"]
    C4["Export / API Access"]
    C5["Executive Accessibility"]
    C6["Operational Usability"]
    C7["Attack Path Fidelity"]
    C8["Real-Time Graph Analysis"]
    C9["RBAC / Read-Only Access"]
    C10["Third-Party Integration"]
    C11["Cost Transparency"]
end

subgraph COL2["Tenable Identity Exposure (Alsid)"]
    T1["Relay-based collectors"]
    T2["Centralized SaaS + Relays"]
    T3["Tenable-controlled model"]
    T4["CSV-centric, limited APIs"]
    T5["Admin-only visibility"]
    T6["Low outside admins"]
    T7["Abstracted risk modeling"]
    T8["No true graph traversal"]
    T9["Limited / admin-focused"]
    T10["External BI required"]
    T11["High / opaque"]
end

subgraph COL3["BloodHound Enterprise"]
    B1["Native AD telemetry"]
    B2["On-prem / hybrid"]
    B3["Customer-owned graph"]
    B4["Full API + graph access"]
    B5["Exec views via RBAC"]
    B6["High across teams"]
    B7["Ground-truth attack paths"]
    B8["Live graph traversal"]
    B9["Strong RBAC / read-only"]
    B10["SIEM / SOAR / API-native"]
    B11["Transparent / role-based"]
end

%% Row alignment
C1 --- T1
C1 --- B1

C2 --- T2
C2 --- B2

C3 --- T3
C3 --- B3

C4 --- T4
C4 --- B4

C5 --- T5
C5 --- B5

C6 --- T6
C6 --- B6

C7 --- T7
C7 --- B7

C8 --- T8
C8 --- B8

C9 --- T9
C9 --- B9

C10 --- T10
C10 --- B10

C11 --- T11
C11 --- B11
