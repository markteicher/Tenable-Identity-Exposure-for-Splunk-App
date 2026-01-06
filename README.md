# Tenable-Identity-Exposure-Utilities
Tenable Identity Exposure Utilities


⚠️ Disclaimer

This tool is not an official Tenable product.

Use of this software is not covered by any license, warranty, or support agreement you may have with Tenable. All functionality is implemented independently using publicly available Tenable Identity Exposure API documentation


Neither Tenable Identity Exposure nor BloodHound provides true executive dashboards.


# Tenable Identity Exposure for Splunk

## Overview
Full Splunk App for **Tenable Identity Exposure**.  
Provides operational and analytical visibility into Active Directory identity risk, exposure indicators, attack indicators, privileged access, and administrative activity using Tenable Identity Exposure APIs.

This app is designed to extend Tenable Identity Exposure data beyond administrator-only access and enable Splunk-based analytics, correlation, and visualization.

---

## Features

### 🛡️ Core Capabilities
| Feature | Description |
|--------|-------------|
| 🧭 Identity Exposure Visibility | Centralized view of AD identity risks and deviations |
| 🚨 Indicators of Exposure (IoE) | Severity-based exposure indicators |
| 🧨 Indicators of Attack (IoA) | Detection of active or emerging identity attacks |
| 🧑‍💻 User & Group Monitoring | User, group, and computer inventory |
| 🛡️ Privileged Account Tracking | Native admins, delegated admins, shadow admins |
| 📋 Activity Logging | Administrative and configuration activity tracking |
| 📜 License Visibility | Active user counts, license limits, expiration |

### 📈 Advanced Analytics
| Feature | Description |
|--------|-------------|
| 📊 Risk Trending | Identity risk evolution over time |
| 📉 Deviance Trending | WoW, MoM, QoQ deviation tracking |
| 🧮 Severity Breakdown | Exposure and attack indicators by severity |
| 🧠 Risk Heatmaps | High-risk users, groups, and systems |
| ⏱️ Exposure Aging | Time-based risk and remediation analysis |

### ⚙️ Operational Visibility
| Feature | Description |
|--------|-------------|
| 🧑‍💻 Users Count | Active user counts per domain |
| 🚨 Deviances Count | Total detected identity deviances |
| 🎯 Compliance Score | Tenable-calculated score (0–100) |
| 🛡️ Admin Monitoring | Native and delegated admin metrics |
| 🔁 Data Freshness | Collection status and ingestion health |

### 🚀 Deployment
| Feature | Description |
|--------|-------------|
| 🖥️ Splunk Web Setup | UI-based configuration |
| 🔐 API-Based Collection | Secure ingestion via Tenable Identity Exposure APIs |
| ☁️ Splunk Cloud Ready | AppInspect-aligned |
| 📊 Pre-built Dashboards | Immediate visibility out of the box |

---

## Installation

### Step 1: Deploy the App
1. Download `Tenable_Identity_Exposure_For_Splunk_App-1.0.0.tar.gz`
2. In Splunk Web, navigate to **Apps → Manage Apps**
3. Click **Install app from file**
4. Upload the archive and click **Upload**
5. Restart Splunk when prompted

### Step 2: Configure the App
Navigate to **Apps → Tenable Identity Exposure → Setup**

#### API Configuration
- **API Base URL**: `https://customer.tenable.ad`
- **API Key**: Tenant API key
- **Verify SSL**: Enabled by default
- **Request Timeout**: Configurable

#### Proxy Configuration (Optional)
- **Use Proxy**
- **Proxy URL**
- **Proxy Authentication** (if required)

#### Data Inputs
Enable ingestion for:
- Domains
- Users
- Groups
- Computers
- Privileged Accounts
- Indicators of Exposure (IoE)
- Indicators of Attack (IoA)
- Activity Logs
- License & Usage Metrics

### Step 3: Validate Configuration
1. Click **Test API Connection**
2. Confirm successful authentication
3. Verify index creation and permissions

### Step 4: Verify Data Collection
```spl
index=security_tenable_tie
| stats count by sourcetype
