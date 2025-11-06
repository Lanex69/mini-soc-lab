# Mini SOC Research Testbed

Security Telemetry Engine is a reproducible SOC testbed that generates attack telemetry, correlates Zeek and Wazuh alerts in Elastic, and measures false-positive reduction, detection latency, and alert volume. The environment also integrates a custom Python web-pentest tool to generate realistic network and host telemetry.

---

## Objective

Develop a reproducible and research-driven SOC testbed to:

1. Generate and analyze realistic attack telemetry
2. Detect and correlate multi-stage attacks
3. Measure alert noise and evaluate prioritization methods
4. Explore improvements in detection accuracy and analyst efficiency

---

## Current Lab Architecture

| Component | Role | Status |
|----------|------|--------|
| Parrot OS | Attacker VM (offensive testing) | Completed |
| Windows 10 | Victim VM with Sysmon logging | Completed |
| Wazuh Manager | SIEM and host telemetry analysis | In progress |
| Zeek | Network monitoring and log enrichment | Planned |
| Elastic Stack | Search, log indexing, dashboards | Planned |
## Architecture

![SOC Architecture Diagram](images/architecture.png)


---

## Research Focus Areas

- Alert correlation between network and host telemetry
- Reducing false positives in SOC environments
- Detection latency observations
- Measuring overall alert volume and prioritization gains

Planned evaluation metrics:
- True positives vs. false positives
- Detection latency
- Alert volume before and after correlation
- Severity assignment/priority scoring

---

## Attack Scenarios (Planned)

- SSH brute force
- Directory fuzzing and web reconnaissance
- DNS tunneling simulation
- Privilege escalation attempts

---

## Related Work

Web-Pentest Toolkit (attack generator):  
[https://github.com/Lanex69/vulnerability-scanner](https://github.com/Lanex69/vulnerability-scanner)

---

Lab build continues after scheduled system reset. Updates will be added here as progress continues.
