# SSH Brute-Force Simulation and Detection Using Splunk

## About the Project

This project documents a controlled SSH brute-force simulation and detection exercise conducted in a Kali Linux lab environment. It demonstrates how failed SSH authentication attempts are generated, recorded in Linux authentication logs, and investigated using Splunk.

The objective is to understand SSH authentication security, analyse failed-login activity, and explore how SIEM tools can help identify suspicious authentication behaviour.

## Objectives

- Understand SSH and brute-force attack concepts.
- Configure and verify the SSH service in Kali Linux.
- Generate controlled failed SSH authentication attempts.
- Investigate authentication events in Linux logs.
- Analyse failed-login activity using Splunk Search Processing Language (SPL).
- Configure and verify a Splunk alert for suspicious authentication activity.
- Document commands, results, screenshots, and troubleshooting steps.

## Tools and Technologies

- **Kali Linux** — Lab environment.
- **OpenSSH** — SSH service used for authentication testing.
- **Splunk Enterprise** — Security monitoring and log analysis.
- **Linux utilities** — `systemctl`, `grep`, `tail`, `ip`, and `ssh`.
- **Linux authentication logs** — Evidence for investigating SSH login attempts.

## Methodology

### 1. SSH Service Verification

Checked the SSH service status, started the service, and verified its listening state on TCP port 22.

### 2. Controlled Failed-Login Simulation

Generated failed SSH authentication attempts in the lab to observe the resulting authentication events.

### 3. Authentication Log Analysis

Inspected relevant Linux authentication logs, including `/var/log/auth.log` where available, to identify failed SSH login attempts.

### 4. Splunk Log Investigation

Used Splunk searches to examine SSH authentication events and identify repeated failed-login activity.

### 5. Alert Configuration and Verification

Configured and tested a Splunk alert for suspicious SSH authentication activity. The accompanying report documents the search query, alert configuration, and observed results.

### 6. Service Cleanup

Stopped the SSH service after testing and checked its final status.

## Key Learnings

- SSH service management and port verification.
- Linux authentication-log analysis.
- Identification of repeated failed authentication attempts.
- Splunk searches and alert configuration.
- Troubleshooting service and log-collection issues.
- Security documentation using screenshots and observed evidence.

## Documentation

The accompanying report contains the practical procedure, commands and explanations, terminal screenshots, Splunk searches, alert verification, troubleshooting notes, and conclusions.

**Report:** `SSH_Brute_Force_Attack.pdf`

## Scope and Responsible Use

This exercise was conducted in a controlled virtual lab for educational purposes. Authentication testing should only be performed on systems you own or have explicit permission to assess.

## Future Improvements

- Refine detection logic using failed-login thresholds and time windows.
- Develop additional Splunk dashboards for SSH authentication events.
- Explore defensive controls such as SSH key authentication, access restrictions, and rate limiting.

---

*This project documents my hands-on learning in SSH security, Linux log analysis, and SIEM-based threat detection.*
