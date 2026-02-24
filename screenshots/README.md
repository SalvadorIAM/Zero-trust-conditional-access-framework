# Policy Configuration and Validation Screenshots

This folder contains evidence of the Zero Trust Privileged Admin Conditional Access implementation, including identity preparation, authentication strength configuration, policy deployment, and enforcement validation.

---

## Phase 1 – Identity Preparation

### 01 – Privileged Admin Group Overview
![Privileged Admin Group Overview](01-privileged-admin-group-overview.png)

### 02 – All Security Groups
![All Security Groups](02-all-security-groups.png)

### 03 – Privileged Admin Membership
![Privileged Admin Membership](03-privileged-admin-membership.png)

### 04 – HR User Membership
![HR User Membership](04-hr-user-membership.png)

### 05 – Standard User Membership
![Standard User Membership](05-standard-user-membership.png)

---

## Phase 2 – Control Design

### 06 – Named Location: Trusted UK Office
![Named Location](06-named-location-trusted-uk-office.png)

### 07 – Authentication Strength: Phishing Resistant
![Authentication Strength](07-authentication-strength-phishing-resistant.png)

---

## Phase 3 – Conditional Access Configuration

### 08 – Grant Control: Require Authentication Strength
![CA Grant Control](08-ca-admin-grant-auth-strength.png)

### 09 – Conditional Access Policy Created
![CA Policy Created](09-ca-admin-policy-created.png)

---

## Phase 4 – Enforcement and Validation

### 10 – Policy Evaluation Result
![Policy Evaluation](10-policy-evaluation-result.png)

### 11 – Login Blocked Due to Authentication Strength Requirement
![Login Blocked](11-login-blocked-phishing-resistant-required.png)

### 12 – Sign-in Failure (Error 53003)
![Sign-in Error 53003](12-signin-error-53003.png)

### 13 – Conditional Access Grant Control Not Satisfied
![Grant Not Satisfied](13-conditional-access-grant-not-satisfied.png)
