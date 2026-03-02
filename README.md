# Digital Forensic Case Study  
## Threat Assessment – Potential Non-Consensual Data Exposure

---

## Professional Disclosure

This case study is derived from an actual digital forensic engagement conducted by the author in a private professional capacity.

All personally identifiable information (PII), sensitive data, account identifiers, device details, and contextual elements have been fully anonymized and redacted in strict compliance with applicable data protection regulations, including the Brazilian General Data Protection Law (LGPD – Law No. 13.709/2018).

This publication is intended exclusively for educational and professional portfolio purposes. No protected personal data is disclosed.

---

## 1. Executive Summary

This investigation involved the forensic examination of a mobile iOS device and a Windows 11 workstation in response to a reported threat of non-consensual dissemination of sensitive personal content.

The primary objectives were:

- Identify evidence of account creation and configuration related to potential dissemination.
- Determine whether automated or scheduled email distribution was established.
- Verify whether any transmission of sensitive material occurred.
- Reconstruct a reliable timeline of relevant events.

The examination revealed artifacts consistent with preparatory actions; however, no conclusive evidence of successful dissemination was identified within the analyzed devices.

---

## 2. Scope of Examination

The forensic scope included:

- Forensic imaging and validation
- Email artifact examination
- Messaging application artifact analysis
- File system metadata review
- Deleted file recovery
- Timeline reconstruction
- Cross-device correlation analysis

No external provider subpoena or cloud provider server-side acquisition was performed as part of this engagement.

---

## 3. Evidence Acquisition

### 3.1 Windows Workstation

- Forensic disk image acquired using industry-standard imaging procedures.
- Cryptographic hash verification performed (SHA256).
- Integrity preserved throughout examination process.

### 3.2 iOS Mobile Device

- Logical extraction performed.
- Application artifacts parsed.
- Email configurations and account metadata analyzed.
- Messaging application databases reviewed.

Due to encryption architecture inherent to iOS systems, certain protected partitions were inaccessible without advanced acquisition techniques.

---

## 4. Methodology

The investigation adhered to established digital forensic principles:

- Preservation of original evidence
- Read-only forensic analysis environment
- Hash-based integrity verification
- Artifact-based reconstruction
- Correlated multi-source timeline analysis

### Tools Utilized

- Autopsy (disk artifact analysis)
- FTK Imager (forensic acquisition)
- iLEAPP (iOS artifact parsing)
- Log and metadata analysis utilities

All examinations were conducted within controlled forensic environments.

---

## 5. Findings

### 5.1 Email Account Artifacts

- Evidence of creation of multiple email accounts within the relevant timeframe.
- Metadata consistent with configuration activity.
- Subsequent deletion of at least one account identified.
- No confirmed SMTP transmission artifacts or sent-message logs recovered locally.

---

### 5.2 Messaging Artifacts

- Partial conversation fragments identified.
- Gaps in message continuity consistent with manual deletion.
- Audio artifacts referencing potential exposure intent recovered.

---

### 5.3 Sensitive File Artifacts

- Sensitive image files identified on the mobile device.
- File system metadata consistent with handling activity during the relevant timeframe.
- No forensic artifacts confirming bulk upload or distribution located within examined devices.

---

### 5.4 Third-Party Platform Indicators

- References to mass email platform usage identified in account artifacts.
- No evidence of active campaign deployment or confirmed outbound transmission discovered.
- Metadata suggests account deactivation prior to any confirmed dissemination event.

---

## 6. Timeline Reconstruction

Correlated analysis across devices indicates the following sequence:

1. Creation of email accounts.
2. Preparation of digital content.
3. Local storage of sensitive files.
4. Account deletion activity.
5. No confirmed outbound transmission event identified within device artifacts.

Timeline reconstruction was based on file system metadata, application logs, and recovered artifacts.

---

## 7. Conclusions

Based on the available forensic artifacts:

- Preparatory actions for potential dissemination were identified.
- No conclusive evidence confirms that dissemination occurred.
- Account deletion activity suggests possible abandonment of intent.
- Findings are limited to locally accessible device artifacts.

This assessment does not exclude the theoretical possibility of external transmission via unexamined systems or services.

---

## 8. Limitations

- Encrypted system areas restricted deeper artifact recovery.
- No server-side email provider logs were available.
- Analysis limited to devices voluntarily submitted for examination.

---

## 9. Technical Competencies Demonstrated

This case demonstrates applied competency in:

- Cross-platform forensic analysis (iOS & Windows)
- Email artifact reconstruction
- Metadata timeline analysis
- Messaging database examination
- Digital evidence handling
- Threat-based forensic assessment
- Report structuring for legal context

---

## 10. Ethical and Legal Compliance

All identifying information has been permanently removed.  
No sensitive images, raw evidence files, or device identifiers are included in this repository.

This case study reflects methodology and investigative reasoning only.

---

For professional inquiries:  
LinkedIn: https://www.linkedin.com/in/onyalan-almeida-609a931b2/
Email: professional contact available upon request
