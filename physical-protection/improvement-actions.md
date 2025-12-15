# Physical Protection – Improvement Actions

## Create customized or use default DLP policies for endpoints
**Status:** Not Implemented (Pending Admin Action)  
**Evidence:** Internal evidence on file (NDA)

### Work Performed
- Reviewed endpoint data protection configuration in Microsoft Intune to determine
  whether Windows Information Protection (WIP) or endpoint DLP policies were present.
- Confirmed access level is read-only, preventing policy creation or modification.
- Verified that no active WIP policy was currently deployed to endpoints.

### Findings
- No WIP / endpoint DLP policy detected during review.
- Endpoint data protection posture requires policy creation and assignment.

### Recommendations
- Create a WIP or endpoint DLP policy aligned with organizational data handling requirements.
- Deploy initially in **Simulation/Audit** mode to measure impact.
- Review alerts and policy matches before transitioning to **Enforce** mode.
- Re-review policy status after device sync and monitor protection status.

---

## Protect Windows Devices
**Status:** Not Implemented (Prepared / Simulation Phase)  
**Evidence:** Internal evidence on file (NDA)

### Work Performed
- Reviewed existing DLP policy categories and synchronization status.
- Identified baseline policies designed to protect sensitive data types.

### Findings
- Default customer account information policy is synchronized and operating in
  **Simulation** mode.
- Additional policy categories (HR, Finance, Healthcare, IP, Adaptive) are available
  but not yet enforced.

### Recommendations
- Validate simulation results and tune policy conditions.
- Confirm endpoint coverage and user scope.
- Transition policies to **Enforce** mode after validation and approval.
