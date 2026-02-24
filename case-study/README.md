# Zero Trust Conditional Access Framework  
**Author:** Salvador A. Semedo  

---

## Executive Summary

This case study documents the design and implementation of a Zero Trust Conditional Access framework in Microsoft Entra ID for a simulated UK-based enterprise environment.

The objective was to strengthen identity security posture by enforcing phishing-resistant authentication for privileged administrators, restricting access from unmanaged devices, and applying structured, signal-driven access controls.

The implementation demonstrates practical application of Zero Trust identity principles using Microsoft Entra ID Conditional Access.

---

## Architecture Overview

The solution was designed using a layered identity protection model consisting of:

- User segmentation (Privileged Admins, HR Users, Standard Users)  
- Authentication Strength policies enforcing phishing-resistant MFA  
- Named Locations defining trusted UK corporate IP ranges  
- Device-based Conditional Access using device compliance state  
- Risk-based evaluation using Microsoft Entra ID Identity Protection  

Access decisions are evaluated dynamically based on user role, device state, location, and authentication strength.

---

## Implementation Approach

The deployment followed a staged approach to prevent tenant lockout and ensure controlled enforcement.

1. Policies were created in Report-only mode.  
2. Policy logic was validated using the Conditional Access What If tool.  
3. Sign-in logs were analysed to confirm correct evaluation results.  
4. Policies were then moved to the On state for active enforcement.  

Key controls implemented:

- Break-glass account exclusions to prevent administrative lockout  
- Phishing-resistant MFA required for privileged administrators  
- Conditional restrictions for unmanaged devices  
- Structured policy targeting based on group membership  

---

## Verification and Validation

Policy behaviour was validated through:

- Conditional Access What If simulation  
- Sign-in log analysis  
- Authentication strength evaluation results  
- Testing compliant and non-compliant scenarios  

Blocked access attempts correctly generated:

**Error 53003**  
**Grant control not satisfied**

This confirmed the enforcement of authentication strength requirements.

---

## Risk Mitigation Outcomes

The implementation reduced risk in the following areas:

- Mitigated phishing and MFA downgrade attacks against privileged accounts  
- Reduced likelihood of sensitive data exposure from unmanaged devices  
- Prevented tenant lockout through emergency access exclusions  
- Minimized policy conflicts through staged rollout and log validation  

---

## Conclusion

This case study demonstrates the practical implementation of a Zero Trust identity model using Microsoft Entra ID.

Rather than relying on basic MFA enforcement, the framework applies layered, conditional, signal-driven logic to dynamically control access.

The lab highlights architectural design, policy structuring, governance awareness, and validation through log analysis aligned with real-world IAM engineering practices.
