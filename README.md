# Windows Event Viewer Log Analysis Lab

## Objective

The purpose of this lab was to analyze Windows Security logs using Event Viewer and investigate successful and failed logon events. This activity helps develop foundational SOC Analyst skills in log analysis and event investigation.

## Tools Used

- Windows Event Viewer

- Windows Security Logs

- Windows 11

---

## Screenshot 1 - Event Viewer Open

Opened Windows Event Viewer and navigated to the Windows Security logs.

![Event Viewer Open](Screenshot%20(1).png)

---

## Screenshot 2 - Security Log Filtered

Filtered the Security log to display Event IDs 4624 and 4625 for investigation.

![Security Log Filtered](Screenshot%20(2).png)

---

## Screenshot 3 - Event ID 4625 Analysis

Event ID 4625 indicates a failed logon attempt.

### Findings

- Event ID: 4625

- Event Type: Failed Logon

- Category: Logon

- Result: Audit Failure

- Host: KenKen

### SOC Analyst Notes

A failed logon event was identified within the Windows Security log. The event was reviewed to determine the time of occurrence and the affected system. Failed logon events can result from incorrect credentials or unauthorized access attempts and should be investigated for unusual activity.

![Event ID 4625](Screenshot%20(3).png)

---

## Screenshot 4 - Event ID 4624 Analysis

Event ID 4624 indicates a successful logon event.

### Findings

- Event ID: 4624

- Event Type: Successful Logon

- Category: Logon

- Result: Audit Success

### SOC Analyst Notes

A successful logon event was identified and reviewed. Successful logon events are useful for validating user authentication activity and establishing timelines during investigations.

![Event ID 4624](Screenshot%20(4).png)

---

## Investigation Summary

During this lab, Windows Security logs were analyzed using Event Viewer. Event ID 4625 was identified as a failed logon attempt, while Event ID 4624 was identified as a successful logon event. The event details, timestamps, and logon information were reviewed to understand authentication activity on the system.

This lab demonstrates foundational SOC Analyst skills including:

- Log analysis

- Event investigation

- Security monitoring

- Authentication event review

- Documentation of findings

## Key Takeaways

- Event ID 4624 = Successful Logon

- Event ID 4625 = Failed Logon

- Security logs provide valuable information for investigations

- Event Viewer is an important tool for SOC analysts

- Reviewing authentication logs helps identify suspicious activity