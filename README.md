# 🛡️ Hurly Cabalan — Cybersecurity Portfolio

> **Azure Security Engineer | SOC Analyst in Training**
> Certifications in Progress: SC-200 | AZ-500
> Location: Doha, Qatar | Target Market: GCC

---

## 📊 Master Progress Tracker

| Scenario | Cert | Domain | Status | Exam Topics Covered | MITRE | QCSF |
|---|---|---|---|---|---|---|
| 01 - Brute Force Detection | SC-200 | Identity | 🔴 Not Started | Analytics Rules, KQL, Incidents | T1110 | ✅ |
| 02 - Insider Threat / Privilege Escalation | SC-200 | Identity | 🔴 Not Started | PIM, UEBA, Hunting | T1078 | ✅ |
| 03 - C2 Beacon Detection | SC-200 | Threat Hunting | 🔴 Not Started | Hunting Queries, DeviceNetworkEvents | T1071 | ✅ |
| 04 - Account Takeover | SC-200 | Identity | 🔴 Not Started | SigninLogs, SOAR, Playbooks | T1586 | ✅ |
| 05 - Misconfigured Resource Exposure | SC-200 | Defender for Cloud | 🔴 Not Started | Secure Score, Policy, Workflow | T1530 | ✅ |
| 06 - Privileged Identity Attack | AZ-500 | Domain 1 | 🔴 Not Started | PIM, Conditional Access, Identity Protection | T1078 | ✅ |
| 07 - External Identity Compromise | AZ-500 | Domain 1 | 🔴 Not Started | B2B, Conditional Access, Access Reviews | T1199 | ✅ |
| 08 - Network Intrusion Attempt | AZ-500 | Domain 2 | 🔴 Not Started | NSG, Firewall, DDoS, Bastion | T1190 | ✅ |
| 09 - Lateral Movement via Network | AZ-500 | Domain 2 | 🔴 Not Started | Private Endpoints, NSG, WAF, Flow Logs | T1021 | ✅ |
| 10 - VM Compromise & Recovery | AZ-500 | Domain 3 | 🔴 Not Started | JIT, Disk Encryption, Defender for Cloud | T1486 | ✅ |
| 11 - Storage & Key Vault Attack | AZ-500 | Domain 3 | 🔴 Not Started | SAS, Key Vault, Soft Delete, Defender Storage | T1530 | ✅ |
| 12 - Database Security | AZ-500 | Domain 3 | 🔴 Not Started | SQL ATP, Dynamic Masking, Always Encrypted | T1213 | ✅ |
| 13 - Full SOC Investigation | AZ-500 | Domain 4 | 🔴 Not Started | Defender for Cloud, Policy, Logic Apps, Sentinel | T1595 | ✅ |

**Legend:** 🔴 Not Started | 🟡 In Progress | 🟢 Complete

---

## 💰 Azure $200 Credit Tracker

| Service | Estimated Cost | Actual Cost | Scenarios Used |
|---|---|---|---|
| Log Analytics Workspace | ~$10-15 | - | All |
| Microsoft Sentinel | ~$0-5 | - | SC-200 heavy |
| Defender for Cloud Enhanced | ~$15 | - | 05, 13 |
| VM (B1s - spin up/down only) | ~$8-10 | - | 10 |
| Logic Apps/Playbooks | ~$1-2 | - | 04, 13 |
| Storage Account | ~$1-2 | - | 11 |
| Buffer | ~$10 | - | - |
| **Total Estimated** | **~$45-60** | **-** | |
| **Remaining Credit** | **~$140-155** | **-** | |

---

## 📅 Study Timeline

| Month | Focus | Cert Target |
|---|---|---|
| Month 1 | SC-200 70% / AZ-500 30% | SC-200 Exam |
| Month 2 | AZ-500 Domains 1-2 Scenarios | Progress |
| Month 3 | AZ-500 Domains 3-4 + Speed Training + Exam | AZ-500 Exam |

---

## ⚡ Daily Execution Model (Every Session)

> **Learn → Lab → Explain — same session, every session**

| Block | Duration | Activity |
|---|---|---|
| Step 1 | 30-60 min | Read 1 Microsoft Learn module — concept only |
| Step 2 | 2-3 hours | Lab — apply that exact concept hands-on |
| Step 3 | 15-30 min | Explain out loud — "What did I just do and why?" |

**Ratio:** 70% Labs / 30% Theory — Labs dominate always.

---

## 📆 Weekly Structure

**Month 1 — SC-200**
| Week | Focus |
|---|---|
| Week 1 | KQL speed — write without copying, interpret output |
| Week 2 | Attack patterns — Scenarios 01-02 |
| Week 3 | Correlation + Threat Hunting — Scenarios 03-04 |
| Week 4 | Defender for Cloud + Exam Prep — Scenario 05 + Practice exams |

**Month 2 — AZ-500 Foundation**
| Week | Focus |
|---|---|
| Week 1 | Identity — MFA, Conditional Access, Identity Protection — Scenario 06 |
| Week 2 | Access — RBAC, PIM, JIT — Scenario 07 |
| Week 3 | Secrets & Data — Key Vault, Managed Identity — Scenarios 08-09 |
| Week 4 | Integration — cross-domain reasoning — Scenario 10 |

**Month 3 — AZ-500 Mastery + Speed Training**
| Week | Focus |
|---|---|
| Week 1 | Compute + Storage + Database — Scenarios 11-12 |
| Week 2 | Full SOC Investigation — Scenario 13 |
| Week 3 | ⚡ Speed Drills — given scenario, choose correct control in under 60 seconds |
| Week 4 | Practice exams 40+ questions/day — book and sit AZ-500 exam |

> **Speed Drill Format (Week 3 Month 3):** Read scenario → identify attack → name the failed control → state the fix. Target: under 60 seconds per drill.

---

## 🔗 Integration Rule (Mandatory Every Scenario)

> **"This happened because [control] failed or was bypassed."**

| Detection | Control That Failed | Fix |
|---|---|---|
| Brute Force succeeded | MFA not enforced | Conditional Access MFA policy |
| Privilege escalation | No PIM / permanent role assigned | PIM just-in-time activation |
| Data exposure | Storage public access enabled | Azure Policy deny public access |
| C2 beacon undetected | No threat hunting scheduled | Scheduled hunting queries in Sentinel |
| Account takeover | No impossible travel detection | Identity Protection risk policy |

---

## 🧠 Global Evidence Confidence Model

> Applied in every scenario before escalation decision.

| Confidence Level | Signal Criteria | Action |
|---|---|---|
| 🔴 Weak | Single signal — no corroboration | Continue investigating — do NOT escalate yet |
| 🟡 Medium | 2 correlated signals from different sources | Escalate with caveat — flag as probable |
| 🟢 Strong | Multi-source + behavioral anomaly + TI match | Escalate immediately as confirmed incident |

> **Rule:** Never escalate on a single signal alone. User self-reporting is a data point — not evidence.

---

## 🤖 Global Automation vs Human Boundary

> Applied in every scenario playbook design.

| Action | Automation | Human Decision |
|---|---|---|
| Disable compromised account | ✅ Auto-trigger | ❌ |
| Block malicious IP | ✅ Auto-trigger | ❌ |
| Send alert notification | ✅ Auto-trigger | ❌ |
| Declare incident severity | ❌ | ✅ Analyst decides |
| Confirm TP vs FP | ❌ | ✅ Analyst decides |
| Escalate to L2/L3 | ❌ | ✅ Analyst decides |
| Notify CISO/management | ❌ | ✅ Senior analyst decides |
| Legal hold / HR involvement | ❌ | ✅ Management decides |

> **Principle:** Automate containment. Humans own decisions.

---

## 📁 Repository Structure

```
📁 Security-Portfolio/
├── 📁 SC-200/
│   ├── 📁 Scenario-01-BruteForce/
│   ├── 📁 Scenario-02-InsiderThreat/
│   ├── 📁 Scenario-03-C2Beacon/
│   ├── 📁 Scenario-04-AccountTakeover/
│   └── 📁 Scenario-05-MisconfiguredResource/
├── 📁 AZ-500/
│   ├── 📁 Scenario-06-PrivilegedIdentity/
│   ├── 📁 Scenario-07-ExternalIdentity/
│   ├── 📁 Scenario-08-NetworkIntrusion/
│   ├── 📁 Scenario-09-LateralMovement/
│   ├── 📁 Scenario-10-VMCompromise/
│   ├── 📁 Scenario-11-StorageKeyVault/
│   ├── 📁 Scenario-12-DatabaseSecurity/
│   └── 📁 Scenario-13-FullSOCInvestigation/
└── 📄 README.md
```

---

# SC-200 SCENARIOS

---

## 🔗 SC-200 Attack Chain — One Story, Five Stages

> **All 5 SC-200 scenarios are connected. Same threat actor. Escalating attack. One complete incident.**

| Stage | Scenario | What Happens |
|---|---|---|
| Stage 1 | 01 - Brute Force | Attacker hammers login page, gets initial access |
| Stage 2 | 02 - Insider/Privilege Escalation | Attacker activates PIM role, gains elevated access |
| Stage 3 | 03 - C2 Beacon | Attacker deploys malware, establishes C2 channel |
| Stage 4 | 04 - Account Takeover | Attacker pivots to high-value account, exfiltrates data |
| Stage 5 | 05 - Misconfigured Resource | Root cause found — storage misconfiguration enabled attack |

> **The story:** *APT group targets a Qatar-based organization. Initial access via credential brute force → privilege escalation via PIM → malware deployed → lateral movement to high-value account → data staged in misconfigured storage for exfiltration. SOC detects at Stage 1 and contains before Stage 4 completes.*

---

## 🔴 Scenario 01 — Brute Force Attack Detection

**Cert:** SC-200 | **Domain:** Mitigate Threats Using Microsoft Sentinel
**Exam Topics:** Analytics Rules, KQL, Incidents, Alerts, Playbooks
**Status:** 🔴 Not Started

---

### 📖 The Story
> *An attacker systematically tries multiple passwords against a corporate Azure AD account. The SOC receives an alert, investigates, contains, and remediates before full compromise occurs. This is Stage 1 of a larger attack chain.*

---

### 🎭 Threat Actor Profile
| Field | Detail |
|---|---|
| Actor Type | External Attacker / Opportunistic |
| Motivation | Credential Theft / Initial Access |
| TTPs Used | T1110 - Brute Force, T1078 - Valid Accounts |
| Tools | Password spray, credential stuffing tools |

---

### ⚠️ Alert
- **What triggered:** Sentinel Analytics Rule — 10+ failed sign-in attempts from single IP within 10 minutes
- **Alert severity:** High
- **Data source:** SigninLogs

**KQL Query — Optimized for Performance:**
```kql
// PERFORMANCE NOTE: project early to reduce data processed downstream
// Filter before aggregation — never summarize full table first
SigninLogs
| where TimeGenerated > ago(1h)                          // time-bound first — always
| where ResultType != "0"                                 // filter early — reduces rows
| project TimeGenerated, UserPrincipalName, IPAddress, ResultType, ResultDescription
| summarize
    FailedAttempts = count(),
    FirstAttempt = min(TimeGenerated),
    LastAttempt = max(TimeGenerated)
    by UserPrincipalName, IPAddress
| where FailedAttempts > 10                              // threshold filter after summarize
| sort by FailedAttempts desc
```
> **KQL Performance Note:** `project` before `summarize` reduces columns processed. Always filter by `TimeGenerated` first — it partitions data at ingestion level and cuts query cost significantly.

---

### 🧪 Hypothesis
> *Before touching logs — what do I expect to find?*

| Question | Expected Answer |
|---|---|
| Is this a real attack or noise? | Real — volume too high for legitimate user error |
| Which logs will confirm or deny? | SigninLogs + Threat Intelligence + post-login activity |
| What does success look like for the attacker? | A successful login following the failed attempts |
| What control should have stopped this? | MFA — if enforced, password alone is useless |

---

### 🔍 Investigation
| Step | Action | Finding |
|---|---|---|
| 1 | Query SigninLogs for failed attempts | 47 failed attempts from single IP |
| 2 | Check IP against threat intelligence | IP flagged as malicious in TI feed |
| 3 | Check for successful login after failures | 1 successful login after 47 failures |
| 4 | Review post-login activity | Unusual file access detected |
| 5 | Timeline correlation | Account compromised at [TIME] |

**Evidence & Artifacts:**
- [ ] Screenshot: Sentinel incident dashboard
- [ ] Screenshot: KQL query results
- [ ] Screenshot: TI IP match
- [ ] Screenshot: Successful login after brute force

**Incident Timeline:**
| Time | Event |
|---|---|
| T+0 | First failed login attempt |
| T+10min | Analytics rule triggers alert |
| T+12min | SOC analyst picks up incident |
| T+15min | Investigation begins |
| T+20min | Compromised account identified |
| T+25min | Mitigation executed |

---

### ✅ TP / FP Decision

| Field | Answer |
|---|---|
| **Classification** | ✅ True Positive |
| **Justification** | 47 failed attempts + successful login + TI-flagged IP = confirmed attack |
| **Confidence Level** | 🟢 Strong — multi-source corroboration |
| **Control That Failed** | MFA not enforced — attacker succeeded with password alone |

---

### 🚨 FP Stress Cases

> *Two realistic scenarios that look like this alert but are NOT attacks. You must be able to disprove them.*

**FP Case 1 — User forgot password after account lock**
- User tried multiple passwords after vacation, locked themselves out, finally recalled correct one
- How to disprove: Check login geography — same location as user's normal pattern? Check device compliance — is it a known registered device? Check post-login behavior — normal work activity vs. unusual access?
- If geography matches + known device + normal activity → reclassify as FP, document and close

**FP Case 2 — Automated script using stale credentials**
- Legacy application or script running scheduled job with old credentials — fails repeatedly until someone updates config
- How to disprove: Check UserPrincipalName — is it a service account? Check login time — does it match scheduled job windows? Check if failures are perfectly periodic (automation) vs. random intervals (human attacker)?
- If service account + periodic intervals + no successful login → FP, escalate to app team to fix credentials

> **Key Rule:** User self-reporting "that was me" is a data point — NOT sufficient evidence alone. Always corroborate with logs before reclassifying.

---

### 🔍 Detection Failure Mode

> *How could an attacker bypass this detection? What is the backup signal?*

| Failure Scenario | How Attacker Evades | Backup Detection |
|---|---|---|
| Low-and-slow attack | Attacker spreads attempts over days — stays below 10/10min threshold | Adjust analytics rule to detect 5 failures over 24 hours |
| Distributed spray | Attacker uses many IPs — each IP only attempts once | Hunt for same UserPrincipalName across multiple source IPs |
| Valid MFA token stolen | Attacker passes MFA via adversary-in-the-middle proxy | Identity Protection impossible travel + session anomaly |
| Insider with valid credentials | No brute force — direct login | UEBA behavioral baseline deviation |

---

### 🛡️ Mitigation
- [ ] Disable compromised account immediately
- [ ] Block malicious IP via Conditional Access named location
- [ ] Force password reset
- [ ] Enable MFA immediately
- [ ] Revoke all active sessions

---

### 🤖 Automation vs Human Boundary

| Action | Who |
|---|---|
| Auto-disable account on alert trigger | ✅ Playbook |
| Block malicious IP | ✅ Playbook |
| Notify user of compromise | ✅ Playbook |
| Confirm TP vs FP | ✅ Human analyst |
| Escalate to L2 for forensics | ✅ Human analyst |
| Decide if data breach notification required | ✅ Senior analyst / CISO |

---

### 🧠 Decision
> Account confirmed compromised — 47 failures + TI-flagged IP + successful login + post-login anomaly. Immediate disable chosen over password reset alone because active session confirmed. Playbook auto-contained while analyst investigated.

---

### 💼 Business Impact Assessment
| Factor | Detail |
|---|---|
| Data at Risk | User email, files, Azure resources accessible to account |
| Financial Impact | Potential data breach costs, regulatory fines |
| Operational Impact | Account unavailable during investigation |
| Reputation Impact | High if customer data accessed |
| **Risk Before Mitigation** | 🔴 Critical |
| **Risk After Mitigation** | 🟡 Medium (pending full forensics) |

---

### 📋 Compliance Mapping
| Framework | Control | Status |
|---|---|---|
| QCSF | Identity & Access Management | ✅ |
| NIST CSF | PR.AC-1, DE.CM-1, RS.RP-1 | ✅ |
| ISO 27001 | A.9.4.2, A.12.4.1 | ✅ |

---

### 📞 Escalation Path
| Level | Role | Action | Trigger |
|---|---|---|---|
| L1 SOC | Analyst | Triage, contain account | Always |
| L2 SOC | Senior Analyst | Full investigation, forensics | Confirmed compromise |
| L3 SOC | IR Lead | Full incident response | Active breach confirmed |
| Management | CISO | Notification | Data exfiltration suspected |

---

### 📚 Lessons Learned
- [ ] What detection worked well?
- [ ] What slowed investigation?
- [ ] Were data connectors properly configured?
- [ ] Was analytics rule threshold correctly tuned?

### 🔧 What Could Be Done Better
- [ ] Improvement 1
- [ ] Improvement 2
- [ ] Improvement 3

---

### 🔗 Peer Review
| Reviewer | Role | Feedback | Date |
|---|---|---|---|
| Ammiel Mejia | Security Infrastructure Sr. Engineer | | |
| Richard | Senior Threat Hunter | | |

---

### 💼 Interview Q&A

**Q: Walk me through detecting a brute force attack in Sentinel.**
> A: I start with a KQL query against SigninLogs — time-bounded first for cost efficiency, then filter for failed ResultType, summarize by UserPrincipalName and IPAddress, and threshold at 10+ failures. I correlate with threat intelligence to check IP reputation, then look for a successful login following the failures. If I find one, I check post-login activity for behavioral anomalies. The analytics rule in Sentinel automates this detection so it fires as an incident automatically.

**Q: How do you differentiate brute force from legitimate failed logins?**
> A: Four factors: volume — legitimate users rarely fail 10+ times; IP reputation — is the source TI-flagged; timing pattern — random intervals suggest human attacker, perfectly periodic suggests automation or user error; post-login behavior — a real user resumes normal activity, an attacker pivots to unusual resources immediately.

**Q: Why is MFA the critical control here?**
> A: Because brute force only works when a password alone is sufficient to authenticate. If MFA is enforced, the attacker's 47 attempts are completely useless — the correct password still cannot complete the login without the second factor. This is why "Control That Failed" is always MFA not enforced in brute force scenarios.

---

### 📢 LinkedIn Post Template
```
🔐 Scenario Complete: Brute Force Attack Detection

Simulated a real brute force attack against Azure AD and built a full
detection and response workflow in Microsoft Sentinel.

What I built:
✅ Optimized KQL analytics rule — time-bounded, project-first for cost efficiency
✅ Automated incident creation with full timeline reconstruction
✅ Playbook to auto-disable compromised account on trigger
✅ FP stress testing — verified 2 legitimate scenarios that mimic attack

Key insight: MFA not enforced = brute force will always eventually succeed.
The control failure, not the attack itself, is what the SOC must fix.

#MicrosoftSentinel #SC200 #CyberSecurity #SOC #KQL #AzureSecurity #Qatar
```

---
---

## 🔴 Scenario 02 — Insider Threat / Privilege Escalation

**Cert:** SC-200 | **Domain:** Mitigate Threats Using Microsoft Sentinel
**Exam Topics:** PIM, UEBA, Hunting Queries, AuditLogs, Incidents
**Status:** 🔴 Not Started

---

### 📖 The Story
> *A legitimate employee with standard access activates a Global Admin PIM role at 2AM. The SOC detects the anomaly, investigates, and discovers data exfiltration in progress. This is Stage 2 — the attacker from Stage 1 now escalates privileges using the compromised account.*

---

### 🎭 Threat Actor Profile
| Field | Detail |
|---|---|
| Actor Type | Insider Threat / Compromised Employee Account |
| Motivation | Data Theft / Sabotage |
| TTPs Used | T1078 - Valid Accounts, T1548 - Privilege Escalation |
| Tools | Azure Portal, PIM self-activation |

---

### ⚠️ Alert
- **What triggered:** Sentinel alert — PIM role activation outside business hours
- **Alert severity:** High
- **Data source:** AuditLogs

**KQL Query — Optimized for Performance:**
```kql
// Filter by time and operation early — don't scan full AuditLogs table
AuditLogs
| where TimeGenerated > ago(24h)
| where OperationName == "Add member to role completed (PIM activation)"  // specific filter first
| project TimeGenerated, InitiatedBy, TargetResources, Result
| extend InitiatedByUser = tostring(InitiatedBy.user.userPrincipalName)
| extend ActivatedRole = tostring(TargetResources[0].displayName)
| where hourofday(TimeGenerated) !between (8 .. 18)   // off-hours filter
| project TimeGenerated, InitiatedByUser, ActivatedRole, Result
```
> **KQL Performance Note:** Always filter OperationName before extending new columns — extension functions are expensive and should run on already-filtered rows only.

---

### 🧪 Hypothesis
| Question | Expected Answer |
|---|---|
| Is this a real attack or noise? | Suspicious — off-hours PIM activation is abnormal baseline |
| Which logs will confirm or deny? | AuditLogs + UEBA anomaly score + post-activation activity |
| What does success look like for the attacker? | Global Admin access + data exfiltration window before detection |
| What control should have stopped this? | PIM approval workflow — requires justification and human approver |

---

### 🔍 Investigation
| Step | Action | Finding |
|---|---|---|
| 1 | Review PIM activation logs | Activation at 2AM — outside business hours |
| 2 | Check UEBA baseline | Unusual behavior score elevated significantly |
| 3 | Review actions post-activation | Mass file download detected |
| 4 | Cross-reference HR | Employee resignation submitted same day |
| 5 | Full activity timeline | Data exfiltration confirmed |

**Evidence & Artifacts:**
- [ ] Screenshot: PIM activation alert
- [ ] Screenshot: UEBA anomaly score
- [ ] Screenshot: Post-activation mass download
- [ ] Screenshot: File download KQL results

**Incident Timeline:**
| Time | Event |
|---|---|
| T+0 | PIM activation request submitted at 2AM |
| T+5min | Sentinel alert triggers |
| T+10min | SOC investigates |
| T+20min | Suspicious post-activation activity confirmed |
| T+30min | Account suspended, IR initiated, legal notified |

---

### ✅ TP / FP Decision

| Field | Answer |
|---|---|
| **Classification** | ✅ True Positive |
| **Justification** | Off-hours + UEBA anomaly + mass download + resignation same day = insider threat confirmed |
| **Confidence Level** | 🟢 Strong — 4 correlated signals |
| **Control That Failed** | PIM had no approval requirement — self-activation permitted without oversight |

---

### 🚨 FP Stress Cases

**FP Case 1 — Emergency after-hours change by legitimate admin**
- On-call admin activated elevated role to respond to a production incident at 2AM
- How to disprove: Check IT change management system — is there an approved emergency change ticket? Check post-activation activity — does it match the stated incident? Check if activity was communicated to SOC?
- If approved change ticket exists + activity matches stated purpose → FP, update process to notify SOC in advance

**FP Case 2 — Time zone mismatch for remote admin**
- Admin working from a different time zone — 2AM local is 9AM for them
- How to disprove: Check user's registered location and normal working hours pattern from UEBA baseline. Check if this type of activation has occurred before at same local time for this user?
- If consistent with user's established pattern + no behavioral anomaly → FP, update analytics rule to account for user time zone

---

### 🔍 Detection Failure Mode

| Failure Scenario | How Attacker Evades | Backup Detection |
|---|---|---|
| Activation during business hours | Attacker waits for 9AM to blend in | UEBA behavioral baseline — activity pattern deviation regardless of time |
| Gradual privilege escalation | Attacker uses lower roles first before targeting Global Admin | Hunt for incremental role activation pattern over days |
| Cleanup of audit logs | Attacker attempts log deletion | Azure Monitor activity log is immutable — cannot be deleted |
| Short activation window | Attacker activates then deactivates quickly | PIM activation log captures all activations even if immediately removed |

---

### 🛡️ Mitigation
- [ ] Revoke PIM activation immediately
- [ ] Suspend user account
- [ ] Preserve all audit logs for legal — do not delete anything
- [ ] Notify HR and Legal
- [ ] Review all files accessed during activation window

---

### 🤖 Automation vs Human Boundary

| Action | Who |
|---|---|
| Alert SOC on off-hours PIM activation | ✅ Playbook |
| Revoke PIM activation | ✅ Playbook |
| Suspend user account | ✅ Playbook |
| Confirm insider threat vs legitimate change | ✅ Human analyst |
| Legal hold decision | ✅ Management + Legal |
| HR escalation | ✅ Management |

---

### 🧠 Decision
> Off-hours PIM Global Admin activation + UEBA anomaly + mass file download + resignation confirmed = insider threat. Account suspended immediately. Legal notified for evidence preservation before any remediation that could destroy artifacts.

---

### 💼 Business Impact Assessment
| Factor | Detail |
|---|---|
| Data at Risk | All resources accessible to Global Admin |
| Financial Impact | IP theft, regulatory fines, legal costs |
| Operational Impact | Admin operations disrupted during investigation |
| **Risk Before Mitigation** | 🔴 Critical |
| **Risk After Mitigation** | 🟡 Medium |

---

### 📋 Compliance Mapping
| Framework | Control | Status |
|---|---|---|
| QCSF | Privileged Access Management | ✅ |
| NIST CSF | PR.AC-4, DE.CM-3, RS.AN-1 | ✅ |
| ISO 27001 | A.9.2.3, A.12.4.1 | ✅ |

---

### 📞 Escalation Path
| Level | Role | Action | Trigger |
|---|---|---|---|
| L1 SOC | Analyst | Initial triage | Always |
| L2 SOC | Senior Analyst | PIM + UEBA investigation | Confirmed suspicious activation |
| L3 IR | IR Lead | Full forensics | Data exfiltration suspected |
| Legal/HR | Management | Legal hold | Insider threat confirmed |

---

### 📚 Lessons Learned
- [ ] *(Fill in after completing scenario)*

### 🔧 What Could Be Done Better
- [ ] *(Fill in after completing scenario)*

---

### 🔗 Peer Review
| Reviewer | Role | Feedback | Date |
|---|---|---|---|
| Ammiel Mejia | Security Infrastructure Sr. Engineer | | |
| Richard | Senior Threat Hunter | | |

---

### 💼 Interview Q&A

**Q: How do you detect insider privilege escalation in Azure?**
> A: I use AuditLogs filtered for PIM activation events, then correlate with UEBA behavioral baseline. Key signals are off-hours activation, role type (Global Admin is highest risk), and post-activation activity patterns. UEBA gives me a behavioral score that flags when the user's activity deviates from their established baseline — that's often more reliable than time-of-day rules alone.

**Q: What is UEBA and how does Sentinel use it?**
> A: UEBA — User and Entity Behavior Analytics — builds a behavioral baseline for each user over time, then flags statistical deviations. In Sentinel, it scores entities based on anomalous behavior like accessing unusual resources, activating high privileges, or downloading atypical data volumes. It's powerful for insider threats because the attacker is using legitimate credentials — traditional rule-based detection misses them, but UEBA catches the behavioral shift.

**Q: Why preserve logs before remediation in an insider threat case?**
> A: Because this is a potential legal matter. Remediating first can destroy forensic evidence needed for HR action or legal proceedings. Evidence preservation always comes before remediation in insider threat scenarios — even if it means the account stays active slightly longer under monitoring.

---

### 📢 LinkedIn Post Template
```
🔐 Scenario Complete: Insider Threat / Privilege Escalation

Simulated a malicious insider escalating to Global Admin via PIM at 2AM
and built a full detection, investigation, and response workflow.

What I built:
✅ Off-hours PIM activation detection using KQL + AuditLogs
✅ UEBA behavioral anomaly correlation
✅ Evidence preservation workflow before remediation
✅ FP stress testing — legitimate emergency changes vs. real insider threat

Key insight: PIM with no approval requirement = any employee can become Global Admin.
The control failure is the missing approval workflow, not the activation itself.

#MicrosoftSentinel #SC200 #InsiderThreat #PIM #UEBA #CyberSecurity #Qatar
```

---
---

## 🔴 Scenario 03 — C2 Beacon Detection

**Cert:** SC-200 | **Domain:** Threat Hunting
**Exam Topics:** Hunting Queries, DeviceNetworkEvents, Threat Intelligence, Bookmarks
**Status:** 🔴 Not Started

---

### 📖 The Story
> *A device in the network makes regular periodic outbound connections to an unknown external IP — classic C2 beacon pattern. This is Stage 3 — after gaining initial access (Stage 1) and elevated privileges (Stage 2), the attacker deploys malware to establish persistent remote control.*

---

### 🎭 Threat Actor Profile
| Field | Detail |
|---|---|
| Actor Type | Advanced Persistent Threat |
| Motivation | Persistence / Data Exfiltration / Ransomware staging |
| TTPs Used | T1071 - Application Layer Protocol, T1102 - Web Service C2 |
| Tools | Cobalt Strike, Metasploit, custom beacons |

---

### ⚠️ Alert
- **What triggered:** Proactive threat hunting query — periodic connections to unknown external IP
- **Alert severity:** Critical
- **Data source:** DeviceNetworkEvents

**KQL Query — Optimized for Performance:**
```kql
// Project only needed columns first — reduces memory and processing cost
DeviceNetworkEvents
| where TimeGenerated > ago(24h)
| where ActionType == "ConnectionSuccess"              // filter early
| project TimeGenerated, DeviceName, RemoteIP, RemotePort
| summarize
    ConnectionCount = count(),
    FirstSeen = min(TimeGenerated),
    LastSeen = max(TimeGenerated)
    by DeviceName, RemoteIP, RemotePort
| extend BeaconDuration = datetime_diff('hour', LastSeen, FirstSeen)
| extend AvgConnectionsPerHour = ConnectionCount / (BeaconDuration + 1)
| where AvgConnectionsPerHour between (1 .. 10)       // beacon frequency range
| where ConnectionCount > 20
| sort by AvgConnectionsPerHour desc
```
> **KQL Performance Note:** `project` immediately after the table reference reduces columns before `summarize` runs — critical when DeviceNetworkEvents tables are large in production environments.

---

### 🧪 Hypothesis
| Question | Expected Answer |
|---|---|
| Is this a real attack or noise? | High suspicion — periodic low-volume connections match beacon signature |
| Which logs will confirm or deny? | DeviceNetworkEvents + TI match + DeviceProcessEvents for responsible process |
| What does the attacker gain? | Persistent C2 channel for remote control and ransomware staging |
| What control should have stopped this? | Egress network filtering + TI-based firewall rules |

---

### 🔍 Investigation
| Step | Action | Finding |
|---|---|---|
| 1 | Run hunting query for beacon pattern | Device connecting every 15 minutes to unknown IP |
| 2 | Check remote IP against TI | IP matches known C2 infrastructure |
| 3 | Review responsible process | Unusual process initiating outbound connection |
| 4 | Check device for other IOCs | Additional malware artifacts found |
| 5 | Scope assessment | Single device isolated — no lateral spread confirmed yet |

**Evidence & Artifacts:**
- [ ] Screenshot: Hunting query results
- [ ] Screenshot: TI IP match
- [ ] Screenshot: Process responsible for beacon (DeviceProcessEvents)
- [ ] Screenshot: Device isolation confirmation

**Incident Timeline:**
| Time | Event |
|---|---|
| T-Xdays | Malware deployed on device — beacon begins |
| T+0 | Threat hunter runs query — beacon pattern identified |
| T+10min | TI match confirms C2 infrastructure |
| T+15min | Responsible process identified |
| T+20min | Device isolated from network |
| T+25min | C2 IP blocked across firewall |

---

### ✅ TP / FP Decision

| Field | Answer |
|---|---|
| **Classification** | ✅ True Positive |
| **Justification** | Regular beacon pattern + TI-confirmed C2 IP + unknown process = confirmed malware |
| **Confidence Level** | 🟢 Strong — TI match + behavioral pattern + process anomaly |
| **Control That Failed** | No outbound egress filtering — C2 traffic exited freely |

---

### 🚨 FP Stress Cases

**FP Case 1 — Legitimate monitoring or telemetry software**
- Security agent, backup client, or IT monitoring tool sends periodic heartbeat to vendor cloud
- How to disprove: Check process name — is it a known vendor agent? Check destination domain — does it resolve to a legitimate vendor? Check if other devices have same connection pattern to same IP?
- If known software + verified vendor destination + consistent across managed fleet → FP, add to allowlist

**FP Case 2 — Browser or application auto-update check**
- Software checking for updates on a schedule — mimics beacon frequency
- How to disprove: Check RemotePort — update checks typically use 443. Check RemoteIP resolution — does it belong to a software vendor? Check if connection volume increases before/after version releases?
- If vendor-owned IP + standard port + correlates with update schedule → FP, document and allowlist

---

### 🔍 Detection Failure Mode

| Failure Scenario | How Attacker Evades | Backup Detection |
|---|---|---|
| Domain fronting | Attacker hides C2 behind legitimate CDN (Cloudflare, Azure) | Inspect TLS SNI header — destination vs. certificate mismatch |
| Jitter added to beacon | Attacker randomizes interval to avoid periodic pattern | Hunt for connection volume anomalies vs. strict periodicity |
| HTTPS-encrypted C2 | Traffic looks like normal web browsing | DNS query analysis — repeated lookups to unusual domains |
| Long sleep intervals | Beacon every 6-12 hours — below detection threshold | Extend hunting query to 7-day window with lower frequency threshold |

---

### 🛡️ Mitigation
- [ ] Isolate device from network immediately
- [ ] Block C2 IP across all firewall rules
- [ ] Add IP to Sentinel threat intelligence watchlist
- [ ] Initiate full malware scan and forensics
- [ ] Review all devices for same C2 communication pattern

---

### 🤖 Automation vs Human Boundary

| Action | Who |
|---|---|
| Add C2 IP to TI watchlist | ✅ Playbook |
| Alert SOC team on hunting hit | ✅ Playbook |
| Device network isolation | ✅ Playbook (MDE isolate action) |
| Confirm C2 vs legitimate software | ✅ Human analyst |
| Scope assessment — other devices | ✅ Human analyst |
| Declare ransomware risk | ✅ Senior analyst / CISO |

---

### 🧠 Decision
> Regular 15-minute beacon + TI-confirmed C2 IP + unknown process = ransomware staging confirmed. Device isolated immediately to prevent lateral spread. C2 IP blocked globally. Forensics initiated before reimaging to preserve evidence.

---

### 💼 Business Impact Assessment
| Factor | Detail |
|---|---|
| Data at Risk | All data on compromised device + accessible network shares |
| Financial Impact | Ransomware deployment risk — potentially catastrophic |
| Operational Impact | Device offline during investigation |
| **Risk Before Mitigation** | 🔴 Critical |
| **Risk After Mitigation** | 🟡 Medium |

---

### 📋 Compliance Mapping
| Framework | Control | Status |
|---|---|---|
| QCSF | Malware Protection, Network Security | ✅ |
| NIST CSF | DE.CM-1, RS.MI-1, RS.AN-1 | ✅ |
| ISO 27001 | A.12.2.1, A.13.1.1 | ✅ |

---

### 📞 Escalation Path
| Level | Role | Action | Trigger |
|---|---|---|---|
| L1 SOC | Analyst | Alert triage | Always |
| L2 Threat Hunter | Senior Analyst | Beacon investigation + scope | Confirmed pattern |
| L3 IR | IR Lead | Device forensics + full sweep | C2 confirmed |
| Management | CISO | Notification | Ransomware risk |

---

### 📚 Lessons Learned
- [ ] *(Fill in after completing scenario)*

### 🔧 What Could Be Done Better
- [ ] *(Fill in after completing scenario)*

---

### 🔗 Peer Review
| Reviewer | Role | Feedback | Date |
|---|---|---|---|
| Richard | Senior Threat Hunter | | |
| Ammiel Mejia | Security Infrastructure Sr. Engineer | | |

---

### 💼 Interview Q&A

**Q: How do you identify C2 beacon activity using KQL?**
> A: I look for periodic low-volume outbound connections from a single device to the same external IP — that's the beacon signature. My KQL summarizes connection count, first seen, and last seen by device and remote IP, then calculates average connections per hour. A true beacon typically falls between 1-10 connections per hour consistently over an extended period. I then cross-reference the remote IP against threat intelligence to confirm malicious infrastructure.

**Q: What is the difference between threat hunting and alert-based detection?**
> A: Alert-based detection is reactive — a rule fires when a known pattern occurs. Threat hunting is proactive — I go looking for threats that haven't triggered any alert yet. C2 beacons are a perfect example: a well-configured beacon might never trigger a standard alert, but a hunting query looking for periodic connection patterns will find it. Hunting assumes the attacker is already inside.

**Q: Why isolate the device before full forensics?**
> A: Isolation stops active C2 communication and prevents lateral spread — that's containment priority. I isolate first via MDE's network isolation feature, which cuts network access but preserves the device for forensic investigation. If I waited for forensics before isolating, the attacker retains control during the investigation window.

---

### 📢 LinkedIn Post Template
```
🔐 Scenario Complete: C2 Beacon Detection via Threat Hunting

Hunted for and detected a C2 beacon pattern in Microsoft Sentinel
using DeviceNetworkEvents before any alert was triggered.

What I built:
✅ Optimized KQL hunting query detecting periodic connection patterns
✅ TI correlation to confirm malicious C2 infrastructure
✅ FP stress testing — legitimate monitoring tools vs. real beacons
✅ Detection failure analysis — domain fronting, jitter, HTTPS evasion

Key insight: C2 beacons often never trigger standard alerts.
Proactive hunting is the only way to find them.

#ThreatHunting #MicrosoftSentinel #SC200 #KQL #C2Detection #CyberSecurity #Qatar
```

---
---

## 🔴 Scenario 04 — Account Takeover

**Cert:** SC-200 | **Domain:** Identity Threat Detection + SOAR
**Exam Topics:** SigninLogs, Playbooks, Logic Apps, Conditional Access, SOAR Automation
**Status:** 🔴 Not Started

---

### 📖 The Story
> *Building on the established C2 channel from Stage 3, the attacker pivots to a high-value account via credential takeover. Sentinel detects impossible travel, a playbook auto-responds to contain, and the SOC investigates the full breach scope including email forwarding rules created for ongoing data exfiltration.*

---

### 🎭 Threat Actor Profile
| Field | Detail |
|---|---|
| Actor Type | Cybercriminal / APT with C2 Access |
| Motivation | Financial Gain / Data Exfiltration |
| TTPs Used | T1586 - Compromise Accounts, T1114 - Email Collection |
| Tools | Credential stuffing, C2-assisted pivot |

---

### ⚠️ Alert
- **What triggered:** Impossible travel detection + brute force pattern → successful login
- **Alert severity:** Critical
- **Data source:** SigninLogs

**KQL Query — Optimized for Performance:**
```kql
// Use let statements to define subsets — avoids scanning full table twice
let BruteForce = SigninLogs
| where TimeGenerated > ago(1h)
| where ResultType != "0"
| project UserPrincipalName, IPAddress, FailedTime = TimeGenerated
| summarize FailedCount = count(), FailedTime = max(FailedTime) by UserPrincipalName, IPAddress;
let Success = SigninLogs
| where TimeGenerated > ago(1h)
| where ResultType == "0"
| project UserPrincipalName, SuccessIP = IPAddress, SuccessTime = TimeGenerated;
BruteForce
| join kind=inner Success on UserPrincipalName
| where IPAddress == SuccessIP
| extend TimeDiff = datetime_diff('minute', SuccessTime, FailedTime)
| where TimeDiff between (0 .. 60)
| project UserPrincipalName, IPAddress, FailedCount, FailedTime, SuccessTime, TimeDiff
```
> **KQL Performance Note:** `let` statements pre-filter each subset independently before the join — far more efficient than joining full tables then filtering. Always project only needed columns before joining.

---

### 🧪 Hypothesis
| Question | Expected Answer |
|---|---|
| Is this a real attack or noise? | Real — impossible travel + brute force pattern = high confidence takeover |
| Which logs will confirm or deny? | SigninLogs + post-login activity + OAuth consent logs |
| What does the attacker gain? | Email access + forwarding rules + OneDrive for data staging |
| What control should have stopped this? | Identity Protection impossible travel policy triggering MFA step-up |

---

### 🔍 Investigation
| Step | Action | Finding |
|---|---|---|
| 1 | Run account takeover KQL | Confirmed — brute force + success same IP |
| 2 | Check login geography | Qatar login then Russia within 30 minutes |
| 3 | Review post-login activity | Email forwarding rule created |
| 4 | Check other accounts same IP | 3 other accounts targeted |
| 5 | Assess data accessed | Inbox and OneDrive accessed |

**Evidence & Artifacts:**
- [ ] Screenshot: KQL account takeover results
- [ ] Screenshot: Impossible travel alert
- [ ] Screenshot: Email forwarding rule created
- [ ] Screenshot: Playbook execution log
- [ ] Screenshot: Conditional Access block applied

**Incident Timeline:**
| Time | Event |
|---|---|
| T+0 | Brute force begins from foreign IP |
| T+15min | Successful login — account taken over |
| T+16min | Impossible travel alert triggers |
| T+18min | Playbook auto-disables account |
| T+20min | SOC validates and begins investigation |
| T+35min | Email forwarding rule discovered and removed |

---

### ✅ TP / FP Decision

| Field | Answer |
|---|---|
| **Classification** | ✅ True Positive |
| **Justification** | Impossible travel + brute force + email forwarding rule = confirmed takeover |
| **Confidence Level** | 🟢 Strong — 3 correlated signals + post-compromise artifact |
| **Control That Failed** | Identity Protection risk policy not configured — impossible travel not triggering MFA step-up |

---

### 🚨 FP Stress Cases

**FP Case 1 — User travelling internationally using VPN**
- User is in Russia on business, VPN exit node appears as Qatar — creates apparent impossible travel
- How to disprove: Contact user directly. Check device compliance — is it a managed corporate device? Check if VPN usage is consistent with user's travel pattern? Check post-login activity — is it normal work activity?
- If user confirms travel + managed device + normal activity → FP, add VPN exit nodes to named locations in Conditional Access

**FP Case 2 — Shared account used by multiple team members in different locations**
- Shared service account accessed simultaneously by team in two different countries
- How to disprove: Check if account type is shared or individual. Check if multiple concurrent sessions exist. Check if this pattern has occurred before for this account?
- If shared account with documented multi-user access → FP, escalate to team to implement individual accounts (shared accounts are a security risk regardless)

> **Key Rule:** Never close an impossible travel alert as FP based on user claim alone without corroborating log evidence.

---

### 🔍 Detection Failure Mode

| Failure Scenario | How Attacker Evades | Backup Detection |
|---|---|---|
| VPN to appear local | Attacker uses VPN exit node in user's country | Focus on post-login behavioral anomaly vs. geographic signal |
| Slow data exfiltration | Attacker downloads files slowly to avoid volume threshold | File access pattern analysis — unusual file types or paths |
| Legitimate OAuth app abuse | Attacker creates OAuth app to access mail without direct login | Monitor OAuth app consents — alert on new apps with mail access |
| Session token theft | Attacker steals valid session — no login event at all | Impossible travel on existing session + Continuous Access Evaluation |

---

### 🛡️ Mitigation
- [ ] Playbook auto-disables account on alert trigger
- [ ] Block IP via Conditional Access named location
- [ ] Remove malicious email forwarding rule
- [ ] Force MFA re-enrollment
- [ ] Review all OAuth app consents granted by compromised account
- [ ] Notify user and confirm activity

---

### 🤖 Automation vs Human Boundary

| Action | Who |
|---|---|
| Disable account on impossible travel + brute force | ✅ Playbook |
| Block attacking IP | ✅ Playbook |
| Notify user of compromise | ✅ Playbook |
| Validate TP vs FP | ✅ Human analyst |
| Remove email forwarding rule | ✅ Human analyst |
| Assess BEC financial fraud risk | ✅ Senior analyst |

---

### 🧠 Decision
> Impossible travel + brute force + confirmed session + email forwarding rule = account takeover confirmed. Playbook contained automatically. Manual removal of forwarding rule required — automation cannot safely remove email rules without risk of destroying evidence.

---

### 💼 Business Impact Assessment
| Factor | Detail |
|---|---|
| Data at Risk | Email, OneDrive, Teams messages |
| Financial Impact | Business Email Compromise risk |
| Operational Impact | Account disabled — user unable to work |
| **Risk Before Mitigation** | 🔴 Critical |
| **Risk After Mitigation** | 🟢 Low after full remediation |

---

### 📋 Compliance Mapping
| Framework | Control | Status |
|---|---|---|
| QCSF | Identity Management, Incident Response | ✅ |
| NIST CSF | PR.AC-1, DE.AE-2, RS.RP-1 | ✅ |
| ISO 27001 | A.9.4.2, A.16.1.5 | ✅ |

---

### 📞 Escalation Path
| Level | Role | Action | Trigger |
|---|---|---|---|
| Playbook | Automated | Auto-disable account | Alert trigger |
| L1 SOC | Analyst | Validate automation, begin investigation | Always |
| L2 SOC | Senior Analyst | Full forensics | Confirmed takeover |
| L3 IR | IR Lead | BEC investigation | Financial fraud suspected |

---

### 📚 Lessons Learned
- [ ] *(Fill in after completing scenario)*

### 🔧 What Could Be Done Better
- [ ] *(Fill in after completing scenario)*

---

### 🔗 Peer Review
| Reviewer | Role | Feedback | Date |
|---|---|---|---|
| Ammiel Mejia | Security Infrastructure Sr. Engineer | | |
| Richard | Senior Threat Hunter | | |

---

### 💼 Interview Q&A

**Q: Walk me through detecting and responding to an account takeover using Sentinel.**
> A: I use a KQL query with two let statements — one for failed logins, one for successful logins — then join on UserPrincipalName where the same IP appears in both within a 60-minute window. That identifies brute force followed by success. I cross-reference with Identity Protection impossible travel alerts. Post-detection, a playbook automatically disables the account and blocks the IP. I then manually investigate post-login activity — email rules, OAuth consents, file access — to assess the full breach scope.

**Q: How do you build a playbook in Sentinel to auto-respond to incidents?**
> A: I create a Logic App triggered by a Sentinel incident. The trigger receives the incident entity — in this case the compromised user account. I add actions: call the Microsoft Entra API to disable the user, add the source IP to a named location in Conditional Access, and send a notification to the SOC team. The key design principle is automate containment actions, leave the TP/FP classification decision to the human analyst.

---

### 📢 LinkedIn Post Template
```
🔐 Scenario Complete: Account Takeover Detection & Automated SOAR Response

Detected an account takeover via impossible travel + brute force correlation
and built an automated playbook response in Microsoft Sentinel.

What I built:
✅ KQL using let statements for efficient join-based detection
✅ Logic App playbook auto-disabling account on trigger
✅ FP stress testing — VPN travel, shared accounts
✅ Detection evasion analysis — session token theft, OAuth abuse

Key insight: Impossible travel alone is noise.
Impossible travel + brute force pattern + post-login artifact = confirmed takeover.

#SOAR #MicrosoftSentinel #SC200 #AccountTakeover #Playbooks #CyberSecurity #Qatar
```

---
---

## 🔴 Scenario 05 — Misconfigured Resource Exposure

**Cert:** SC-200 | **Domain:** Defender for Cloud
**Exam Topics:** Secure Score, Recommendations, Policy, Workflow Automation
**Status:** 🔴 Not Started

---

### 📖 The Story
> *Root cause analysis of the full attack chain reveals a publicly exposed storage account — the misconfiguration that enabled the attacker to stage exfiltrated data without authentication. Defender for Cloud flagged this 7 days earlier. It was never actioned. This is the control failure that enabled Stages 1-4.*

---

### 🎭 Threat Actor Profile
| Field | Detail |
|---|---|
| Actor Type | APT / Opportunistic Scanner |
| Motivation | Data exfiltration staging point |
| TTPs Used | T1530 - Data from Cloud Storage |
| Tools | Cloud scanning tools, Shodan, custom scripts |

---

### ⚠️ Alert
- **What triggered:** Defender for Cloud recommendation — storage account publicly accessible
- **Alert severity:** High
- **Data source:** Defender for Cloud, StorageBlobLogs

**KQL Query — Optimized for Performance:**
```kql
// Filter AuthenticationType first — most specific filter, reduces rows dramatically
StorageBlobLogs
| where TimeGenerated > ago(7d)
| where AuthenticationType == "Anonymous"             // most selective filter first
| project TimeGenerated, AccountName, Uri, CallerIpAddress, OperationName
| summarize
    AccessCount = count(),
    UniqueIPs = dcount(CallerIpAddress),
    LastAccess = max(TimeGenerated)
    by AccountName, Uri
| where AccessCount > 0
| sort by AccessCount desc
```
> **KQL Performance Note:** Put the most selective filter first — `AuthenticationType == "Anonymous"` dramatically reduces rows before any projection or summarization runs.

---

### 🧪 Hypothesis
| Question | Expected Answer |
|---|---|
| Is this a real attack or noise? | Real misconfiguration — public storage is never acceptable for internal data |
| Which logs will confirm or deny? | StorageBlobLogs for anonymous access history |
| What does the attacker gain? | Free access to internal files — zero authentication required |
| What control should have stopped this? | Azure Policy denying public blob access at deployment time |

---

### 🔍 Investigation
| Step | Action | Finding |
|---|---|---|
| 1 | Review Defender for Cloud recommendation | Anonymous access enabled — flagged 7 days ago |
| 2 | Query StorageBlobLogs | 142 anonymous reads in 7 days |
| 3 | Identify data accessed | Internal documents publicly read |
| 4 | Identify who created misconfiguration | AuditLogs shows developer account |
| 5 | Assess data sensitivity | PII data confirmed in accessed files |

**Evidence & Artifacts:**
- [ ] Screenshot: Defender for Cloud recommendation
- [ ] Screenshot: Secure score before/after
- [ ] Screenshot: StorageBlobLogs KQL results
- [ ] Screenshot: Azure Policy assignment

**Incident Timeline:**
| Time | Event |
|---|---|
| T-7 days | Misconfiguration introduced by developer |
| T-7 days | Defender for Cloud recommendation generated — not actioned |
| T-7 days to T+0 | 142 anonymous reads — attacker accessed data freely |
| T+0 | SOC investigates Defender for Cloud backlog |
| T+5min | PII exposure confirmed |
| T+20min | Anonymous access disabled, DPO notified |

---

### ✅ TP / FP Decision

| Field | Answer |
|---|---|
| **Classification** | ✅ True Positive |
| **Justification** | Anonymous access + 142 external reads + PII data = confirmed exposure |
| **Confidence Level** | 🟢 Strong — logs confirm actual unauthorized access occurred |
| **Control That Failed** | No Azure Policy enforcing deny-public-access at deployment + Defender for Cloud recommendation backlog not actioned |

---

### 🚨 FP Stress Cases

**FP Case 1 — Intentionally public static website**
- Developer hosted a public-facing static website in blob storage — anonymous access is expected
- How to disprove: Check container name and content — does it contain static web assets (HTML, CSS, images) or internal documents? Check if the storage account has static website hosting enabled as a feature?
- If static website container + only public assets + no sensitive content → FP, document intentional public access, apply separate policy for internal storage accounts

**FP Case 2 — Defender for Cloud false recommendation on CDN-backed storage**
- Storage account behind Azure CDN intentionally allows anonymous reads for performance — Defender flags it as misconfiguration
- How to disprove: Check if CDN profile is attached. Check if data is public marketing content vs. internal data. Check access log — are requests coming via CDN or direct?
- If CDN-backed + public marketing content → FP, apply Defender for Cloud exemption with documented justification

---

### 🔍 Detection Failure Mode

| Failure Scenario | How Attacker Evades | Backup Detection |
|---|---|---|
| Slow data scraping | Downloads files gradually to avoid volume threshold | Enable Defender for Storage anomaly detection — unusual access pattern |
| Accessing via CDN cache | Attacker never directly touches storage — gets cached version | CDN access logs + Defender for CDN alerts |
| Attacker already has data | Misconfiguration fixed after exfiltration complete | DLP scanning of stored data + data classification before exposure |
| No logging enabled | Diagnostic logs not turned on — no StorageBlobLogs | Defender for Cloud recommendation: enable diagnostic logging |

---

### 🛡️ Mitigation
- [ ] Disable anonymous access immediately
- [ ] Enable Azure AD-only authentication
- [ ] Apply Azure Policy to deny all public storage accounts
- [ ] Notify DPO — PII exposure confirmed
- [ ] Configure workflow automation to auto-remediate future Defender recommendations within SLA

---

### 🤖 Automation vs Human Boundary

| Action | Who |
|---|---|
| Alert SOC on Defender for Cloud High recommendation | ✅ Workflow automation |
| Auto-apply policy deny-public-access | ✅ Azure Policy (prevent at deployment) |
| Confirm PII data sensitivity | ✅ Human analyst |
| DPO notification decision | ✅ Human analyst / management |
| Regulatory breach notification | ✅ Management + Legal |

---

### 🧠 Decision
> 142 anonymous reads of PII data over 7 days = confirmed breach event. Immediate remediation. DPO notified for QPDPL/GDPR assessment. Azure Policy deployed to prevent recurrence. Defender for Cloud recommendation backlog process reviewed — high recommendations must be actioned within 24 hours SLA.

---

### 💼 Business Impact Assessment
| Factor | Detail |
|---|---|
| Data at Risk | PII data exposed publicly for 7 days |
| Financial Impact | QPDPL / GDPR regulatory fines |
| Reputation Impact | High if breach publicly disclosed |
| **Risk Before Mitigation** | 🔴 Critical |
| **Risk After Mitigation** | 🟢 Low |

---

### 📋 Compliance Mapping
| Framework | Control | Status |
|---|---|---|
| QCSF | Data Protection, Cloud Security | ✅ |
| NIST CSF | PR.DS-1, DE.CM-7, RS.MI-3 | ✅ |
| ISO 27001 | A.13.2.1, A.18.1.3 | ✅ |

---

### 📞 Escalation Path
| Level | Role | Action | Trigger |
|---|---|---|---|
| L1 SOC | Analyst | Alert triage, immediate remediation | Always |
| L2 SOC | Senior Analyst | Data exposure assessment | PII confirmed |
| DPO | Data Protection Officer | Regulatory notification | PII breach confirmed |
| Management | CISO | Breach notification decision | Regulatory requirement |

---

### 📚 Lessons Learned
- [ ] *(Fill in after completing scenario)*

### 🔧 What Could Be Done Better
- [ ] *(Fill in after completing scenario)*

---

### 🔗 Peer Review
| Reviewer | Role | Feedback | Date |
|---|---|---|---|
| Ammiel Mejia | Security Infrastructure Sr. Engineer | | |
| Richard | Senior Threat Hunter | | |

---

### 💼 Interview Q&A

**Q: How do you use Defender for Cloud to identify and remediate misconfigurations?**
> A: Defender for Cloud generates prioritized recommendations based on secure score impact. I filter by severity — High first — and review each recommendation with its affected resources. For storage accounts I check if public access is enabled, then review the StorageBlobLogs to determine if unauthorized access actually occurred. Remediation is applying the specific fix — in this case disabling anonymous access — then deploying Azure Policy to prevent the same misconfiguration at deployment time for future resources.

**Q: Why did Defender for Cloud flag this 7 days before it was actioned?**
> A: That's a process failure, not a tooling failure. Defender for Cloud generated the correct recommendation immediately. The gap was the SOC not having an SLA for actioning High recommendations. The lesson is: detection without response is worthless. Every organization needs a defined SLA — High recommendations actioned within 24 hours, Critical within 1 hour.

---

### 📢 LinkedIn Post Template
```
🔐 Scenario Complete: Misconfigured Resource Exposure — Root Cause of Full Attack Chain

Investigated a publicly exposed storage account that Defender for Cloud
flagged 7 days before it was actioned — 142 anonymous reads of PII data.

What I built:
✅ StorageBlobLogs KQL optimized for anonymous access detection
✅ Defender for Cloud remediation + Azure Policy to prevent recurrence
✅ Workflow automation for recommendation SLA enforcement
✅ FP stress testing — legitimate public storage vs. real exposure

Key insight: The control that failed wasn't the storage config alone —
it was the missing SLA for actioning Defender for Cloud recommendations.

#DefenderForCloud #AzurePolicy #SC200 #CloudSecurity #CyberSecurity #Qatar
```

---
---

# AZ-500 SCENARIOS

---

## 🔗 AZ-500 Attack Chain — One Story, Eight Stages

> **All 8 AZ-500 scenarios are connected. Same nation-state threat actor. Full attack lifecycle.**

| Stage | Scenario | What Happens |
|---|---|---|
| Stage 1 | 06 - Privileged Identity Attack | Attacker compromises account, attempts Global Admin via PIM |
| Stage 2 | 07 - External Identity Compromise | Attacker exploits guest B2B access as pivot point |
| Stage 3 | 08 - Network Intrusion | Attacker probes network perimeter, tests firewall |
| Stage 4 | 09 - Lateral Movement | Attacker moves through subnets toward target systems |
| Stage 5 | 10 - VM Compromise | Attacker gains foothold on VM via exposed RDP |
| Stage 6 | 11 - Storage & Key Vault | Attacker targets secrets and data storage |
| Stage 7 | 12 - Database Security | Attacker attempts SQL injection on exposed database |
| Stage 8 | 13 - Full SOC Investigation | SOC detects full chain — investigation, containment, remediation |

> **The story:** *Nation-state affiliated group targets a Qatar energy sector organization. Entry via credential compromise → privilege escalation → network reconnaissance → lateral movement → VM foothold → secrets theft → database attack. Full SOC investigation uncovers the chain and fixes the root causes.*

---

## 🔴 Scenario 06 — Privileged Identity Attack

**Cert:** AZ-500 | **Domain:** Domain 1 — Identity & Access
**Exam Topics:** PIM, Conditional Access, Identity Protection, AuditLogs
**Status:** 🔴 Not Started

---

### 📖 The Story
> *An attacker with compromised credentials attempts to activate a Global Admin PIM role from an unknown IP. Azure AD Identity Protection detects the risky sign-in and Conditional Access blocks the activation. SOC investigates the scope.*

---

### 🎭 Threat Actor Profile
| Field | Detail |
|---|---|
| Actor Type | Nation-State / APT Group |
| Motivation | Full tenant compromise — energy sector target |
| TTPs Used | T1078 - Valid Accounts, T1548 - Privilege Escalation |
| Tools | Compromised credentials, VPN/proxy infrastructure |

---

### ⚠️ Alert
- **What triggered:** Identity Protection risky sign-in + PIM activation blocked by Conditional Access
- **Alert severity:** Critical
- **Data source:** AuditLogs, SigninLogs

**KQL Query — Optimized for Performance:**
```kql
// Specific OperationName filter first — AuditLogs is a large table
AuditLogs
| where TimeGenerated > ago(1h)
| where OperationName contains "PIM"
| where Result == "failure"
| project TimeGenerated, InitiatedBy, TargetResources, ResultReason
| extend User = tostring(InitiatedBy.user.userPrincipalName)
| extend RoleAttempted = tostring(TargetResources[0].displayName)
| project TimeGenerated, User, RoleAttempted, ResultReason
```
> **KQL Performance Note:** AuditLogs is one of the largest tables in any Sentinel workspace. Always filter OperationName before extending — extension is CPU-expensive and should run on minimal rows.

---

### 🧪 Hypothesis
| Question | Expected Answer |
|---|---|
| Is this a real attack or noise? | Real — risky sign-in + immediate PIM Global Admin attempt = coordinated attack |
| Which logs will confirm or deny? | AuditLogs + SigninLogs + Identity Protection risk events |
| What does the attacker gain? | Global Admin = full tenant control — highest possible impact |
| What control should have stopped this? | PIM approval requirement + Conditional Access blocking risky sign-ins |

---

### 🔍 Investigation
| Step | Action | Finding |
|---|---|---|
| 1 | Review Identity Protection risk event | High risk sign-in from unknown IP |
| 2 | Check PIM activation audit logs | Global Admin activation attempted and blocked |
| 3 | Review Conditional Access log | MFA challenge failed — unknown location |
| 4 | Scope assessment | Password spray across 5 accounts same IP |
| 5 | Review all PIM eligible assignments | 3 accounts have eligible Global Admin |

**Evidence & Artifacts:**
- [ ] Screenshot: Identity Protection risk alert
- [ ] Screenshot: PIM blocked activation
- [ ] Screenshot: Conditional Access sign-in log
- [ ] Screenshot: KQL audit results

**Incident Timeline:**
| Time | Event |
|---|---|
| T+0 | Attacker begins password spray from unknown IP |
| T+5min | Compromised credentials used — risky sign-in flagged |
| T+6min | PIM Global Admin activation attempted |
| T+7min | Conditional Access blocks — MFA challenge fails |
| T+10min | Identity Protection alert triggers |
| T+15min | SOC investigates — 5 accounts at risk |
| T+20min | All accounts secured, IP blocked |

---

### ✅ TP / FP Decision

| Field | Answer |
|---|---|
| **Classification** | ✅ True Positive |
| **Justification** | Risky sign-in + immediate PIM Global Admin attempt from unknown IP = coordinated attack |
| **Confidence Level** | 🟢 Strong — Identity Protection + Conditional Access + PIM logs all corroborate |
| **Control That Failed** | PIM had no approval requirement — self-activation was permitted without oversight |

---

### 🚨 FP Stress Cases

**FP Case 1 — Admin travelling internationally activating PIM for legitimate work**
- Global Admin on business trip activating PIM from hotel — unknown location triggers risky sign-in
- How to disprove: Contact admin directly. Check if travel was pre-approved and documented. Check if device is managed and compliant. Check post-activation activity — is it consistent with legitimate admin work?
- If confirmed travel + managed device + legitimate activity → FP, update Conditional Access named locations for approved travel, enforce PIM approval regardless

**FP Case 2 — VPN exit node change triggering location anomaly**
- Admin working from home VPN — exit node changed to different country
- How to disprove: Check if VPN is corporate-managed. Check if new IP belongs to corporate VPN range. Check UEBA baseline — is this admin's login pattern consistent with VPN usage?
- If corporate VPN + consistent pattern → FP, add VPN IP ranges to named locations in Conditional Access

---

### 🔍 Detection Failure Mode

| Failure Scenario | How Attacker Evades | Backup Detection |
|---|---|---|
| Attacker uses VPN matching user location | Appears as local login — no risky sign-in flag | UEBA behavioral anomaly — activity pattern deviation |
| Attacker uses approved device (MDM enrolled) | Passes device compliance check | Time-based anomaly — activation at unusual hours |
| Attacker targets account without PIM eligible | Goes for permanent role instead | RBAC audit — flag permanent Global Admin assignments |
| MFA fatigue attack | Floods user with MFA prompts until accepted | Alert on multiple MFA denials in short window |

---

### 🛡️ Mitigation
- [ ] Confirm and disable compromised account
- [ ] Block malicious IP via Named Location
- [ ] Force MFA re-registration for all affected accounts
- [ ] Add PIM approval requirement — require justification + human approver
- [ ] Review all PIM eligible assignments — remove unnecessary eligibility

---

### 🤖 Automation vs Human Boundary

| Action | Who |
|---|---|
| Alert SOC on risky sign-in + PIM attempt | ✅ Playbook |
| Temporarily block IP | ✅ Playbook |
| Confirm scope of compromised accounts | ✅ Human analyst |
| Disable affected accounts | ✅ Human analyst (scope dependent) |
| Restructure PIM approval workflow | ✅ Senior analyst / IAM team |

---

### 🧠 Decision
> Risky sign-in + PIM Global Admin attempt from unknown IP + password spray across 5 accounts = coordinated nation-state attack confirmed. All 5 accounts secured. IP blocked. PIM approval workflow enforced immediately — no more self-activation for privileged roles.

---

### 💼 Business Impact Assessment
| Factor | Detail |
|---|---|
| Data at Risk | Full tenant if Global Admin compromised — energy sector critical infrastructure |
| Financial Impact | Operational disruption + regulatory breach |
| **Risk Before Mitigation** | 🔴 Critical |
| **Risk After Mitigation** | 🟡 Medium |

---

### 📋 Compliance Mapping
| Framework | Control | Status |
|---|---|---|
| QCSF | Privileged Access Management | ✅ |
| NIST CSF | PR.AC-4, DE.CM-3 | ✅ |
| ISO 27001 | A.9.2.3 | ✅ |

---

### 📞 Escalation Path
| Level | Role | Action | Trigger |
|---|---|---|---|
| L1 SOC | Analyst | Triage | Always |
| L2 SOC | Senior Analyst | PIM + Identity investigation | Confirmed attempt |
| L3 IR | IR Lead | Full tenant review | Multiple accounts targeted |

---

### 📚 Lessons Learned
- [ ] *(Fill in after completing scenario)*

### 🔧 What Could Be Done Better
- [ ] *(Fill in after completing scenario)*

---

### 🔗 Peer Review
| Reviewer | Role | Feedback | Date |
|---|---|---|---|
| Ammiel Mejia | Security Infrastructure Sr. Engineer | | |
| Richard | Senior Threat Hunter | | |

---

### 💼 Interview Q&A

**Q: How does PIM reduce attack surface for privileged roles?**
> A: PIM converts permanent role assignments to eligible assignments. An eligible user only has the role when they explicitly activate it, for a defined time window, with justification and optionally requiring approver sign-off. This means even if credentials are compromised, the attacker cannot immediately use privileged access — they must go through the activation workflow, which triggers alerts and requires MFA. Permanent Global Admin assignments are a critical misconfiguration — PIM eliminates them.

**Q: How does Conditional Access integrate with Identity Protection?**
> A: Identity Protection calculates a risk score for each sign-in — Low, Medium, or High — based on signals like leaked credentials, anonymous IP, impossible travel, and unfamiliar location. Conditional Access can consume that risk score as a condition — for example, block access or require MFA when sign-in risk is High. This creates a dynamic access policy that responds to real-time threat signals rather than static rules.

---

### 📢 LinkedIn Post Template
```
🔐 Scenario Complete: Privileged Identity Attack — Detected & Blocked

Simulated a nation-state attacker attempting PIM Global Admin activation
using compromised credentials from an unknown IP.

What I built:
✅ Identity Protection risk policy + Conditional Access integration
✅ PIM approval workflow enforcement
✅ KQL audit log investigation optimized for large tables
✅ FP stress testing — legitimate travel vs. real attack

Key insight: PIM without an approval requirement means any compromised
account can become Global Admin. The approval workflow is the control.

#AZ500 #PIM #ConditionalAccess #IdentityProtection #AzureSecurity #Qatar
```

---
---

## 🔴 Scenario 07 — External Identity Compromise

**Cert:** AZ-500 | **Domain:** Domain 1 — Identity & Access
**Exam Topics:** B2B External Identities, Conditional Access, Access Reviews, MFA
**Status:** 🔴 Not Started

*(Full investigation framework applies — fill in during lab using same structure as above)*

**Key Control That Will Fail:** B2B guest access without Conditional Access enforcement or Access Reviews

---

## 🔴 Scenario 08 — Network Intrusion Attempt

**Cert:** AZ-500 | **Domain:** Domain 2 — Secure Networking
**Exam Topics:** NSG, Azure Firewall, DDoS Protection, Network Watcher, Bastion
**Status:** 🔴 Not Started

*(Full investigation framework applies — fill in during lab using same structure as above)*

**Key Control That Will Fail:** Overly permissive NSG inbound rules — direct internet access to internal resources

---

## 🔴 Scenario 09 — Lateral Movement via Network

**Cert:** AZ-500 | **Domain:** Domain 2 — Secure Networking
**Exam Topics:** Private Endpoints, Service Endpoints, NSG, WAF, Flow Logs
**Status:** 🔴 Not Started

*(Full investigation framework applies — fill in during lab using same structure as above)*

**Key Control That Will Fail:** No network segmentation — flat network allows unrestricted east-west movement

---

## 🔴 Scenario 10 — VM Compromise & Recovery

**Cert:** AZ-500 | **Domain:** Domain 3 — Compute, Storage & Databases
**Exam Topics:** JIT VM Access, Disk Encryption, Defender for Cloud, VM Security
**Status:** 🔴 Not Started

*(Full investigation framework applies — fill in during lab using same structure as above)*

**Key Control That Will Fail:** RDP port 3389 permanently open to internet — JIT not configured

---

## 🔴 Scenario 11 — Storage & Key Vault Attack

**Cert:** AZ-500 | **Domain:** Domain 3 — Compute, Storage & Databases
**Exam Topics:** SAS Tokens, Key Vault, Soft Delete, Purge Protection, Defender for Storage
**Status:** 🔴 Not Started

*(Full investigation framework applies — fill in during lab using same structure as above)*

**Key Control That Will Fail:** Long-lived SAS token with overly broad permissions — no expiry enforcement

---

## 🔴 Scenario 12 — Database Security

**Cert:** AZ-500 | **Domain:** Domain 3 — Compute, Storage & Databases
**Exam Topics:** SQL Advanced Threat Protection, Dynamic Data Masking, Always Encrypted, TDE
**Status:** 🔴 Not Started

*(Full investigation framework applies — fill in during lab using same structure as above)*

**Key Control That Will Fail:** SQL Advanced Threat Protection not enabled — SQL injection attempt goes undetected

---

## 🔴 Scenario 13 — Full SOC Investigation

**Cert:** AZ-500 | **Domain:** Domain 4 — Security Operations
**Exam Topics:** Defender for Cloud, Azure Policy, Logic Apps, Sentinel Cross-Domain Incident
**Status:** 🔴 Not Started

*(Full investigation framework applies — fill in during lab using same structure as above)*

**Key Control That Will Fail:** No cross-domain incident correlation — individual alerts visible but attack chain not connected

---

---

## 🏆 Certification Progress

| Cert | Status | Target Date | Exam Fee |
|---|---|---|---|
| SC-200 | 🔴 In Study | End of Month 1 | ~$165 |
| AZ-500 | 🔴 In Study | End of Month 2-3 | ~$165 |

---

## 💬 SOC Experience Answer

> *"I don't have commercial SOC experience yet, but I've built a structured detection and investigation portfolio using Microsoft Sentinel where I simulated real attack scenarios end to end — brute force, account takeover, C2 beacon detection, privilege escalation — each documented with full alert triage, KQL investigation, TP/FP decision, mitigation, and lessons learned. I can walk you through any of them right now if you'd like."*

---

## ⚡ The Interview Line

> *"I investigate alerts, identify which security control failed, how it was bypassed, and how to fix it."*

---

## 🔗 Connect With Me

> Open to cybersecurity opportunities in Qatar and GCC region.
> Specializing in Microsoft Security stack — Sentinel, Defender, Azure Security.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/hurly-cabalan-9954a1216/)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black)](https://github.com/hurlycabalan/Soc-Investigation)
---

*Last Updated: May 2026 | Version 2.0 — Full SOC Investigation Framework*
