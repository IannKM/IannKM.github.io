---
title: "Introduction to Secure DevOps"
excerpt_separator: "<!--more-->"
---

# Threat Hunting in Microsoft Sentinel

**Author:** Ian Mutai
**Course:** adc-soa02-25023  
**Course:** Security Operations Analyst - C2 - 2025  
**Certification:** Microsoft Certified: Security Operations Analyst Associate (SC-200)  

---

## Threat Hunting Concepts in Microsoft Sentinel

Threat hunting involves proactively searching through your environment for threats or activities that haven't been previously detected. It is a continuous process that follows a cyclical approach:

1. **Hypothesis:** Plan what to hunt for, including where and how.  
2. **Execution:** Conduct the hunt.  
3. **Response:** Address anomalies and findings.  
4. **Improvement:** Enhance detection capabilities and set up new monitoring.  

### Documentation Requirements  
All threat hunting activities should be documented, including:  
- **What, How, and Why**  
- **Input and Output**  
- **Steps to replicate the hunt**  
- **Next steps**  


🔗 [Click to View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/W2SLPTDN?sharingId=149F627F90730DC1)  

---

### 1. **Threat Hunting with Microsoft Sentinel**

Microsoft Sentinel provides tools to streamline the hunting process:  

#### Built-in Queries  
Predefined queries guide the hunting process and uncover issues that may not trigger alerts individually but warrant investigation over time.  

#### Bookmarks  
Preserve relevant queries and results, and add contextual notes or tags for future reference.  

#### Investigation Graph  
A visual tool to identify entities involved in attacks and their relationships. Features include:  
- Entity contextual information (relationships, account usage, data flow).  
- Alert timeline and correlation review for multi-alert incidents.  

#### Hunting Livestream  
Test queries against live events and receive notifications for matches. Use cases:  
1. Test new queries in real-time.  
2. Generate threat notifications.  
3. Launch investigations.  

🔗 [Click to View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/NV5GS6KF?sharingId=149F627F90730DC1)  

---

## 2. **Using Search Jobs in Microsoft Sentinel**

Search jobs enable hunting across large datasets and long time periods. Archived logs can be restored for inclusion.  

**Supported Log Types:**  
- Analytics logs  
- Basic logs  
- Auxiliary logs  

🔗 [Click to View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/URBJTY23?sharingId=149F627F90730DC1)  

---

### 3. **Advanced Hunting with Notebooks**

Jupyter Notebooks in Microsoft Sentinel allow for advanced hunting with:  
- **Browser-based interface:** Enter and run queries/code, view results.  
- **Kernel:** Parses and executes code.  

Notebooks support live code, equations, visualizations, and explanatory text.  

🔗 [Click to View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/URBTAPA3?sharingId=149F627F90730DC1)  

---

## SC-200: Perform Threat Hunting in Microsoft Sentinel

🔗 [Click to View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/QSNY5HLE?sharingId=149F627F90730DC1)  