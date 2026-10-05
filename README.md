# SBT-DF204 Case Study 1
## Investigating Harassment Email Traffic with Wireshark

### Overview

This repository contains the supporting material for **SBT-DF204 Computer Forensics Case Studies – Case Study 1: Investigating Harassment Email Traffic with Wireshark**.

The investigation examined the supplied `nitroba.pcap` network capture to reconstruct web activity connected to a reported harassment communication.

The analysis focused on preserving the evidence, identifying the client system, locating the relevant HTTP submission, examining browser and device information, reconstructing the activity in UTC, and assessing whether the available evidence supported attribution to a student in Chemistry 109.

The original evidence was preserved and all forensic analysis was performed using a working copy.

---

## Objectives

The main objectives of the investigation were to:

- Preserve the supplied network capture.
- Create a forensic working copy.
- Verify evidence integrity using SHA-256 hashing.
- Identify the client and web service involved.
- Locate the relevant HTTP POST request.
- Examine the submitted harassment message.
- Identify the source MAC address.
- Examine HTTP cookie and browser evidence.
- Recover identity-related information from the browser session.
- Compare the supported identity with the Chemistry 109 roster.
- Reconstruct the relevant activity using UTC timestamps.
- Produce an evidence-based attribution assessment.
- Clearly state the limitations of the available evidence.

---

## Laboratory and Tools Used

The investigation used:

- Kali Linux
- VMware Workstation
- Wireshark
- `wget`
- `sha256sum`
- `grep`
- `nano`
- Standard Linux file-management utilities
- PDF viewer

Wireshark was the primary forensic tool used for packet filtering, packet inspection, HTTP analysis, Ethernet/MAC examination and TCP stream reconstruction.

---

## Evidence Integrity

The SHA-256 value calculated for both the original PCAP and forensic working copy was:

```text
2b77a9eaefc1d6af163d1ba793c96dbccacb04e6befdf1a0b01f8c67553ec2fb
