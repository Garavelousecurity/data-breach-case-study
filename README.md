# Data Breach Case Study

## Overview

This project presents a simulated cybersecurity data breach investigation.
The objective is to analyze the incident, identify the root cause, evaluate security risks, and recommend mitigation strategies to prevent similar incidents.

---

## Scenario

A company detected suspicious activity on its internal database server.
Security monitoring tools identified large data transfers occurring during non-business hours.

The organization initiated a security investigation to determine whether a data breach had occurred.

---

## Initial Indicators

During the investigation, the following indicators were identified:

• Multiple failed login attempts
• Successful login from an unknown external IP address
• Unusual database queries executed
• Large data export from the customer database

---

## Log Evidence

Example authentication log:

| Timestamp        | User  | Source IP     | Event         |
| ---------------- | ----- | ------------- | ------------- |
| 2026-03-10 01:22 | admin | 185.210.44.12 | Login Failed  |
| 2026-03-10 01:23 | admin | 185.210.44.12 | Login Failed  |
| 2026-03-10 01:25 | admin | 185.210.44.12 | Login Success |

Database activity log:

| Timestamp        | User  | Activity             |
| ---------------- | ----- | -------------------- |
| 2026-03-10 01:30 | admin | Export Customer Data |

---

## Root Cause Analysis

The investigation determined that the breach occurred due to:

• Weak administrator password
• Lack of Multi-Factor Authentication
• Insufficient monitoring of database access
• No alerts configured for abnormal data exports

An attacker successfully gained access to the administrative account and extracted sensitive customer data.

---

## Impact Assessment

Potential consequences of the breach include:

• Exposure of customer personal data
• Financial loss
• Legal liability
• Reputational damage

Risk Level: **High**

---

## Security Recommendations

The following security improvements are recommended:

1. Implement Multi-Factor Authentication (MFA)
2. Enable database activity monitoring
3. Enforce strong password policies
4. Implement centralized log monitoring using SIEM
5. Restrict administrative privileges using least-privilege principles

---

## Compliance Considerations

The breach may trigger regulatory obligations such as:

• Data breach notification requirements
• GDPR reporting obligations
• Internal security audit procedures

Organizations must notify affected individuals and relevant authorities within the required regulatory timeframe.

---

## Lessons Learned

This case study highlights the importance of:

• strong authentication mechanisms
• proactive monitoring of sensitive systems
• effective incident response planning

Organizations should regularly review security controls and monitoring capabilities to reduce the likelihood of future breaches.

---

## Skills Demonstrated

• Cybersecurity incident investigation
• Root cause analysis
• Risk assessment
• Security governance
• Compliance awareness
