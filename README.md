# Respond and Recover from a Data Breach

## Objective

The **Respond and Recover from a Data Breach** lab focused on performing a complete cloud security incident response within Google Cloud Platform (GCP). The primary objective was to investigate an active security breach, identify critical vulnerabilities using Security Command Center, remediate compromised cloud resources, strengthen access controls, secure firewall configurations, and validate compliance with PCI DSS standards. This capstone exercise demonstrated an end-to-end cloud security remediation workflow commonly performed by Cloud Security Analysts and SOC teams.

### Skills Learned

- Cloud security incident investigation and remediation.
- Vulnerability analysis using Google Cloud Security Command Center.
- Secure Compute Engine recovery using VM snapshots.
- Cloud Storage access control remediation.
- Firewall hardening and network security implementation.
- PCI DSS compliance validation.
- Security posture assessment and risk mitigation.
- Practical cloud incident response workflow.

### Tools Used

- Google Cloud Platform (GCP)
- Google Cloud Security Command Center (SCC)
- Compute Engine
- Cloud Storage
- Google Cloud Firewall
- Identity-Aware Proxy (IAP)
- PCI DSS Compliance Reports
- Google Cloud Logging

## Steps

### Step 1: Investigate the Security Incident

Began the incident response process by reviewing active security findings within **Google Cloud Security Command Center**. Analyzed vulnerabilities affecting Compute Engine instances, Cloud Storage buckets, and firewall configurations to determine the root causes of the simulated data breach and identify remediation priorities.

---

### Step 2: Recover the Compromised Virtual Machine

Stopped the compromised virtual machine and deployed a clean replacement from a trusted snapshot. Configured the new instance with improved security settings, including **Secure Boot**, removal of the public IP address, restricted service account access, and secure network tagging before permanently removing the compromised system.

---

### Step 3: Secure Cloud Storage Resources

Remediated insecure Cloud Storage configurations by preventing public access, enabling **Uniform Bucket-Level Access**, and removing unnecessary public permissions. These changes ensured that sensitive data could only be accessed through authorized IAM policies.

---

### Step 4: Harden Firewall Security

Created a new firewall rule to restrict SSH access exclusively to **Google Cloud Identity-Aware Proxy (IAP)** source ranges. Removed overly permissive firewall rules allowing unrestricted SSH, RDP, and ICMP traffic to significantly reduce the external attack surface.

---

### Step 5: Improve Network Visibility

Enabled firewall logging for critical network rules to enhance security monitoring and provide greater visibility into allowed and denied traffic. Logging supports incident investigations, compliance requirements, and continuous monitoring activities.

---

### Step 6: Validate Security Compliance

Generated an updated **PCI DSS Compliance Report** using Security Command Center to verify that the identified high and medium severity vulnerabilities had been successfully remediated and that the cloud environment met the required security controls.

---

### Step 7: Complete the Capstone Lab

Successfully completed the full cloud incident response lifecycle by investigating the breach, recovering compromised resources, remediating security misconfigurations, strengthening cloud defenses, and validating compliance through security reporting.

## Lab Completion

**Ref 1: Google Cloud Skills Boost Lab Completion**

![Lab Completion](images/lab-completion.png)

*Assessment Score: **100%** — Successfully completed the cloud security incident response capstone by investigating, remediating, recovering, and validating cloud security controls.*

## Key Takeaway

This capstone lab provided practical experience performing an end-to-end cloud security incident response using Google Cloud Platform. It combined vulnerability assessment, infrastructure recovery, access control remediation, firewall hardening, compliance validation, and security monitoring into a realistic enterprise scenario. The skills demonstrated in this lab closely align with responsibilities performed by **Cloud Security Analysts**, **SOC Analysts**, and **Blue Team** professionals responsible for protecting production cloud environments.
```
