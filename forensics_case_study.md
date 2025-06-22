# Forensics Case Study: Autopsy Workflow

This case study documents a basic digital forensic investigation using **Autopsy**, a GUI-based open-source tool for analyzing hard drives and smartphones.

## 🧰 Tools Used

- Autopsy (v4.19+)
- Sample disk image (.E01 or raw .dd)
- Windows 10 Host
- VirtualBox/Kali (optional for validation)

## 🎯 Objective

To examine a sample disk image, recover deleted files, analyze user activity, and document findings with screenshots and timeline reconstruction.

## 🧪 Investigation Steps

1. **Set up a new case in Autopsy**  
   - Case name: `Forensics_Training_Case_01`
   - Add data source: sample `.dd` image  
   - Use all default ingest modules

2. **Initial Observations**  
   - File system detected: NTFS  
   - Partitions found: 1 primary  
   - Notable findings: deleted `.docx` files, suspicious browser history

3. **Timeline Creation**  
   - File creation and deletion events  
   - Last activity timestamps  
   - Access to suspicious URLs around 03:45 AM

4. **Artifacts Extracted**  
   - Web history (Chrome): visited suspicious phishing domains  
   - Recent documents: resume, passwords.txt  
   - Recycle Bin: recovered deleted Excel with financial data

5. **Screenshots and Evidence Hashes**  
   - [Insert screenshots here]  
   - SHA256: `d6f8b...` for passwords.txt  
   - MD5: `aa12...` for disk image

## 🧾 Report Summary

- Evidence of data exfiltration and user intent to conceal actions  
- Report stored in `/Reports/Forensics_Case_Report.pdf`

## 🔒 Chain of Custody

Maintained using standard case file logs. No tampering or modifications were made outside of Autopsy ingestion and analysis modules.

---

**Note:** This repo is for educational and demonstration purposes. No real user data was used.