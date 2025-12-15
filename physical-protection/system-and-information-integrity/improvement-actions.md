# System and Information Integrity – Improvement Actions

## Block process creations originating from PSExec and WMI commands
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Created an Attack Surface Reduction (ASR) policy in Intune to block process creation
  from PSExec and WMI.
- Assigned policy to a test device group.
- Validated enforcement through endpoint security telemetry and event logging.
- Control reduces lateral movement and remote execution attack vectors.

---

## Block Win32 API calls from Office macros
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Deployed ASR rule to block Win32 API calls initiated by Office macros.
- Assigned to Windows device group via Intune.
- Confirmed deployment and enforcement through Defender telemetry.
- Control mitigates macro-based malware and malicious API execution.

---

## Configure an endpoint security solution for Linux
**Status:** Out of Scope  
**Evidence:** Internal analysis on file (NDA)

- Reviewed control requirements.
- Verified no Linux endpoints are present in the environment.
- Documented implementation approach for future readiness.

---

## Configure an endpoint security solution for macOS
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Deployed Microsoft Defender for Endpoint for macOS via Intune.
- Onboarded macOS device using configuration profile.
- Verified reporting and protection status in Defender XDR.

---

## Configure and validate network connections
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Validated Defender cloud connectivity.
- Confirmed cloud-delivered protection, real-time protection, and behavior monitoring
  are active and healthy.

---

## Create a Web Application Firewall (WAF) policy
**Status:** Implemented (Readiness Confirmed)  
**Evidence:** Internal evidence on file (NDA)

- Verified ability to configure Azure WAF using default protection rules.
- Documented readiness to deploy web-layer protections if required.

---

## Deploy updates for Linux endpoint security solutions
**Status:** Out of Scope  
**Evidence:** Internal analysis on file (NDA)

- Verified Linux endpoints are not in use.
- Reviewed Defender update mechanisms for Linux platforms for future use.

---

## Disable Google Chrome plugins that require authorization
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Confirmed Chrome ADMX policy deployed via Intune.
- Policy disables outdated plugins and reduces browser attack surface.
- Minor remediation required for devices pending check-in.

---

## Configure detection whitelist in monitoring solutions
**Status:** Out of Scope  
**Evidence:** Internal analysis on file (NDA)

- Control not applicable due to cloud-only monitoring scope.

---

## Enable automated investigation and remediation
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Enabled Automated Investigation and Remediation (AIR) in Defender.
- Configured device groups for full remediation capabilities.

---

## Enable supervised chat
**Status:** Out of Scope / Not Applicable  
**Evidence:** Internal analysis on file (NDA)

- Feature is education-only and does not map to NIST 800-171 or CMMC L2 requirements.

---

## Explore security recommendations
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Reviewed Defender Threat & Vulnerability Management recommendations.
- Validated exposure insights and remediation guidance.

---

## Investigate entities on devices using live response
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Validated Live Response capability.
- Successfully initiated and closed investigative sessions.

---

## View and analyze threat protection reports
**Status:** Implemented  
**Evidence:** Internal evidence on file (NDA)

- Reviewed Defender threat protection reports.
- Confirmed visibility into alerts, severity, trends, and exposure.

---

## Verify logging settings
**Status:** Out of Scope  
**Evidence:** Internal analysis on file (NDA)

- Verified logging health with no active issues reported.

---

## Use group policy settings to configure antivirus
**Status:** Implemented (Cloud Equivalent)  
**Evidence:** Internal evidence on file (NDA)

- Configured Microsoft Defender Antivirus via Intune Endpoint Security
  instead of traditional Group Policy.
- Policies centrally manage antivirus settings in a cloud-only environment.
