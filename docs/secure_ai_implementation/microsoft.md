# Microsoft Copilot 365

## 🛠 Phase 1: Foundations and Data Security (Pre-Deployment)
Before you implement your AI, make sure your data is organized and secure.

| Area | Control Point | Tool | Technical Action |
| --- | --- | --- | --- |
| Classification | Sensitivity Labels | Purview | Enable Auto-labeling so that the system automatically labels files containing, for example, account numbers or personal data, so that Copilot knows what requires special protection. |
| Retention | Data Minimization | Purview | Configure Retention Policies. Remove old, outdated procedures from SharePoint to avoid AI hallucinations. |
| Access | Least Privilege | SharePoint Admin | Run the Data Access Governance report. Remove “Everyone” permissions for sensitive sites and replace them with dedicated groups. |
| Admin | Just-In-Time Access | Entra ID (PIM) | Enable Privileged Identity Management. Administrative access to Copilot only for the duration of the task. |

## 🏗 Phase 2: Configuration and Integration (Implementation)
Securing the AI “brain” (Copilot Studio) and points of contact with the web application.

| Area | Control Point | Tool | Technical Action |
| --- | --- | --- | --- |
| Knowledge | Grounding Scope | Copilot Studio | Limit the scope of Generative Answers to specific SharePoint/OneDrive folders only (not the entire tenant). |
| Identity | App Registration | Entra ID | Set Delegated permissions (Sites.Selected). Copilot can only see what the user can see. |
| Web Security | Content Security Policy | Web Server / App Header | Configure the CSP frame-ancestors header to prevent clickjacking attacks on the Copilot chat window in your application. |
| Auth Flow | On-Behalf-Of (OBO) | Entra ID / MSAL.js | Configure the OBO flow so that your web application can securely exchange the user token for a token for Copilot Studio (no need for a second login). |

## 🔍 Phase 3: Monitoring and Audit (Post-Deployment)

| Area | Control Point | Tool | Technical Action |
| --- | --- | --- | --- |
| Conditional Access | Conditional Access | Entra ID | Enforce policy: Access to Copilot = MFA + Trusted Device (Intune Compliant). |
| Response | CAE (Continuous) | Entra ID | Enable Continuous Access Evaluation to immediately block the AI session after account deactivation or location change. |
| Audit | Query Logging | Purview | Enable Unified Audit Log. Ensure you have a license (E3/E5) that allows Copilot log retention beyond 90 days. Log every query (Prompt) sent to Copilot for auditing purposes. |
| Monitoring | Prompt Injection | Sentinel | Connect the Microsoft 365 connector to Sentinel. Import ready-made analytical rules (NRT - Near Real Time) for Microsoft Copilot to detect Prompt Injection or mass data export by AI. |
| Monitoring | Malware Protection | Defender for O365 | Configure alerts for malicious links/files sent in chats (especially when using external plugins). |
| DLP | Clipboard & Export Protection | Purview Endpoint DLP | Block the ability to copy sensitive responses from Copilot to unmanaged applications (e.g., private Gmail, Notepad) on employee computers. |