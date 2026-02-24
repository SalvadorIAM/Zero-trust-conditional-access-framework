# Policy Configuration and Validation Screenshots

This folder contains evidence of the Zero Trust Privileged Admin Conditional Access implementation, including identity preparation, authentication strength configuration, policy deployment, and enforcement validation.

---

## Phase 1 – Identity Preparation

### 01 – Privileged Admin Group Overview
![Privileged Admin Group Overview](01-admin-group-overview.png)

### 02 – All Security Groups
![All Security Groups](02-security-groups.png)

### 03 – Privileged Admin Membership
![Privileged Admin Membership](03-admin-membership.png)

### 04 – HR User Membership
![HR User Membership](04-hr-membership.png)

### 05 – Standard User Membership
![Standard User Membership](05-standard-membership.png)

---

## Phase 2 – Control Design

### 06 – Named Location: Trusted UK Office
![Named Location](06-named-location-uk.png)

### 07 – Authentication Strength: Phishing Resistant
![Authentication Strength](07-auth-strength-phishing.png)

---

## Phase 3 – Conditional Access Configuration

### 08 – Grant Control: Require Authentication Strength
![CA Grant Control](08-ca-grant-auth-strength.png)

### 09 – Conditional Access Policy Created
![CA Policy Created](09-ca-policy-created.png)

---

## Phase 4 – Enforcement and Validation

### 10 – Policy Evaluation Result
![Policy Evaluation](10-ca-policy-evaluation.png)

### 11 – Login Blocked Due to Authentication Strength Requirement
![Login Blocked](11-login-blocked.png)

### 12 – Sign-in Failure (Error 53003)
![Sign-in Error 53003](12-error-53003.png)

### 13 – Conditional Access Grant Control Not Satisfied
![Grant Not Satisfied](13-ca-grant-not-satisfied.png)
