 Brute Force Login → Account Takeover

## 🏢 Organization:
**VasanthCorp Security Operations Center**

---

## 🧑‍💻 Incident Details
| Field | Information |
|------|-------------|
| Alert Source | Microsoft Defender for Cloud Apps / Azure AD |
| Impacted User | `arun.patil@vasanthcorp.com` |
| Device | `HR-LAPTOP-09.vasanthcorp.com` |
| Category | Credential Access |
| MITRE ATT&CK | **T1110 — Brute Force Attack** |
| Severity | High |
| Analyst | VR |
| Status | Closed — True Positive |

---

## 📌 Executive Summary
Multiple failed login attempts (57 failures) followed by a **successful login from Russia** were detected on the account `arun.patil@vasanthcorp.com`.

User confirmed the login was **not authorized**.

➡ **Account Takeover confirmed**

---

## 📊 Investigation Findings

| Evidence | Source |
|---------|--------|
| 57 failed login attempts | Azure AD Sign-in Logs |
| Successful login from Moscow, Russia | Impossible Travel Detection |
| Malicious IP identified | Threat Intel Lookup |
| Authentication: Password only | No MFA enabled |
| User denied login | Phone verification |

✔ Validated and classified as **True Positive**

---

## 🛡️ Remediation Actions

| Action | Status |
|--------|-------|
| Forced password reset | ✔ Done |
| Enabled MFA | ✔ Implemented |
| Blocked malicious IP | ✔ IP added to firewall blocklist |
| Lateral movement check | ✔ Negative |
| Organization-wide IOC sweep | ✔ No Spread |

---

## 📚 MITRE ATT&CK Mapping

| Tactic | Technique |
|--------|----------|
| Credential Access | **T1110 – Brute Force** |
| Initial Access | Valid Accounts via stolen credentials |

---

## 🎯 Final Verdict
| Result | Meaning |
|--------|---------|
| **True Positive** | Unauthorized access confirmed |

---

## 🧠 Key Improvements
- Mandatory MFA deployment
- Smart lockout policy configuration
- Enhanced risky sign-in monitoring

---

## 📸 Evidence Screenshots

Available under:
