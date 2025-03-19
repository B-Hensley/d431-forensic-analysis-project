# Digital Forensics Investigation - Class Project | Autopsy

## Overview
This project consists of two parts: 
1. A **hypothetical** digital forensics investigation plan, written as part of my coursework at Western Governors University (WGU), outlining what steps I would take if tasked with investigating a case of unauthorized access to company data.
2. A **practical component** where I used Autopsy, a digital forensics tool, to investigate a disk image and extract evidence of unauthorized access to confidential and proprietary company data. This was part of a simulated lab where I created a case, analyzed the disk image, and uncovered potential violations.

## Part 1: Investigation Plan (Hypothetical Scenario)
In this section, I outlined the steps I would follow to conduct a forensic investigation, which would include:
- **Collaborating with management and the legal department** to ensure the investigation was aligned with company policies.
- **Creating a baseline of access rights** for the suspect (John Smith) to guide anomaly analysis.
- **Collecting volatile data** and ensuring proper preservation of evidence, such as using FTK Imager to create bit-for-bit copies of the workstation.
- **Analyzing network traffic** with Wireshark to identify any unauthorized transmissions.
- **Thorough documentation** of the evidence collected and maintaining chain of custody.

## Part 2: Autopsy Case Analysis (Simulated Lab)
For the practical part of this project, I used **Autopsy** to investigate a disk image (`JSmith_Q1.001`) and uncover potential evidence of John Smith accessing confidential and proprietary information without authorization. The following steps detail the case I created and my findings:

### Step 1: Case Creation in Autopsy
- **Case Name**: I used my student ID (383166240) as the case number for clarity and to track progress.
- **Data Source**: I selected the `JSmith_Q1.001` disk image as the source data for the case.
- **Configuration**: I accepted the default settings to configure ingest and processed the disk image.

### Step 2: Initial Walkthrough of the Disk Image
Upon initial inspection, I discovered the following:
- **Deleted Files**: 12 deleted files were found.
- **Images**: 379 images were found, some of which were of the company's oil rigs and diagrams.
- **Keyword Search**: Using keywords like "Confidential" and "Proprietary", I found 8 results, including documents like:
  - **Confidential**: "Drilling Methodology.pdf", "Business_Strategy.pdf"
  - **Proprietary**: "Drilling Methodology.pdf", "f000128_Drilling_Methodology.pdf"
  
Additionally, there were suspicious, blurry images that appeared to be related to steganography. One deleted file had a website titled "The best way to hide something, is in plain sight. Crypto laundering", raising suspicion that John Smith was using steganography to hide information.

### Step 3: Evidence of Unauthorized Access
Further investigation revealed that John Smith had:
- Accessed confidential and proprietary information without authorization.
- Likely intended to sell this information using Bitcoin transactions, potentially masked using steganography techniques.
- Evidence pointed to the likelihood that he was planning to distribute the data anonymously.

### Conclusion
This investigation, based on the disk image analysis, supported the allegations against John Smith for accessing and potentially selling confidential and proprietary information from the company. The findings also suggest that steganography may have been used to conceal the information, and Bitcoin was being considered as a method to launder the proceeds.

## Tools Used
- **Autopsy**: For analyzing the disk image and uncovering evidence.
- **FTK Imager**: For imaging the disk and preserving evidence.
- **Wireshark**: For network traffic analysis (not utilized in the simulated lab, but part of the original process).

## Key Takeaways
This project helped me understand both the **theoretical and practical aspects** of digital forensics investigations. It emphasized the importance of maintaining a chain of custody, documenting all actions taken, and using forensics tools effectively to analyze and uncover unauthorized access and illicit activities within digital systems.

---

## References
- **Quality Standards for Digital Forensics** (2019, June 18). [https://www.ignet.gov/sites/default/files/files/Quality_Standards_for_Digital_Forensics_2019.pdf](https://www.ignet.gov/sites/default/files/files/Quality_Standards_for_Digital_Forensics_2019.pdf)
