# Forensic Methodology – Technical Documentation

---

## 1. Forensic Principles Applied

The investigation followed established digital forensic best practices:

- Preservation of original evidence
- Forensic imaging prior to analysis
- Cryptographic integrity validation
- Controlled examination environment
- Artifact-based reconstruction
- Cross-source correlation

All examinations were conducted in a read-only or controlled forensic environment to prevent contamination.

---

## 2. Evidence Preservation and Integrity

### 2.1 Chain of Custody (General Procedure)

Although this public version does not include identifying details, the original investigation included:

- Device intake documentation
- Timestamped acquisition logs
- Examiner identification
- Evidence labeling
- Storage documentation

Each device was handled using evidence-handling precautions to preserve forensic integrity.

---

### 2.2 Forensic Imaging – Windows Workstation

Tool: FTK Imager  

Procedure:

1. Physical disk acquisition performed.
2. Image generated in forensic format.
3. SHA256 cryptographic hash calculated at acquisition.
4. Hash verified post-acquisition.
5. Working copy created for analysis.
6. Original image preserved unmodified.

Integrity validation ensured evidentiary reliability.

---

### 2.3 Logical Extraction – iOS Device

Tool: iLEAPP  

Procedure:

1. Device unlocked with authorized credentials.
2. Logical acquisition performed.
3. Application databases extracted.
4. Email configuration artifacts parsed.
5. Messaging application SQLite databases analyzed.
6. File system metadata reviewed.

Due to encryption architecture of modern iOS devices, full physical acquisition was not performed.

---

## 3. Artifact Analysis Procedures

### 3.1 Email Artifact Examination

Focus areas:

- Account configuration files
- Local mail storage databases
- SMTP-related metadata
- Sent mail artifacts
- Draft artifacts
- Account creation timestamps
- Account deletion indicators

Email-related artifacts were correlated with system event logs to determine temporal alignment.

---

### 3.2 Messaging Application Analysis

Process:

1. Extraction of messaging databases (SQLite).
2. Review of message tables.
3. Identification of deletion gaps.
4. Correlation of message timestamps with device usage logs.
5. Audio artifact extraction and metadata review.

Observed discontinuities were analyzed to assess potential message deletion.

---

### 3.3 File System and Metadata Analysis

Tools: Autopsy  

Analysis included:

- File system structure examination
- Deleted file recovery attempts
- EXIF metadata inspection
- MAC timestamp analysis (Modified, Accessed, Created)
- Timeline view correlation
- Keyword searching
- File signature validation

Metadata was used to reconstruct handling activity during the relevant timeframe.

---

### 3.4 Third-Party Platform Indicators

Artifacts reviewed:

- Browser history records
- Cookie data
- Session artifacts
- Cached content
- Stored credentials (where accessible)

No validated evidence of completed outbound email campaign execution was recovered from local artifacts.

---

## 4. Timeline Reconstruction Methodology

Timeline reconstruction involved:

- Aggregation of file system timestamps
- Email account metadata timestamps
- Messaging application event timestamps
- Browser history events
- Account deletion indicators

Artifacts were normalized into a unified chronological sequence.

This approach allowed identification of:

- Account creation events
- File handling activity
- Potential preparatory actions
- Account deactivation events

No artifacts indicating confirmed outbound transmission were identified in correlation analysis.

---

## 5. Limitations of Examination

The following technical limitations were present:

- Encrypted segments of iOS file system inaccessible without advanced acquisition tools.
- No server-side email provider logs available.
- No direct SMTP header analysis possible without external provider cooperation.
- Cloud synchronization artifacts limited to locally stored data.

All conclusions are restricted to artifacts accessible within examined devices.

---

## 6. Forensic Standards Alignment

The methodology aligns conceptually with:

- Evidence preservation principles
- Hash-based verification practices
- Artifact-based forensic reconstruction
- DFIR investigative workflow standards

This case demonstrates applied digital forensic methodology in a real-world threat assessment scenario.

---

## 7. Professional Note

This document represents the technical methodology applied during the investigation.  

All identifying elements have been removed.  

No raw evidence files, sensitive material, or personally identifiable data are included in this repository.
