---
title: "Create detections and perform investigations using Microsoft Sentinel"
excerpt_separator: "<!--more-->"
---

# Microsoft Sentinel Security Operations Project

## Author: Ian Mutai  
**Week 10 Assignment**  
**Course:** Security Operations Analyst - C2 - 2025  
**Certification:** Microsoft Certified: Security Operations Analyst Associate (SC-200)

---

## 🔍 Project Overview

This assignment demonstrates the application of Microsoft Sentinel to detect, investigate, and respond to cybersecurity threats. It showcases how to use analytics, playbooks, automation, and incident management in Microsoft Sentinel.

---

## ✅ Objectives

- Create detections using Microsoft Sentinel Analytics
- Automate responses with Playbooks
- Investigate incidents with built-in tools
- Normalize data with ASIM
- Monitor and visualize threats
- Manage content using the Content Hub

---

## 📌 Modules & Highlights

### 1. **Threat Detection with Sentinel Analytics**
Microsoft Sentinel Analytics helps you detect, investigate, and remediate cybersecurity threats. You can analyse historical data collected from your workstations, servers, networking devices, firewalls, intrusion prevention, sensors, and so on. Microsoft Sentinel Analytics analyses data from various sources to identify correlations and anomalies. 

🔗 [View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/4GYPA3NK?sharingId=149F627F90730DC1)

📸 *Screenshot:*  
![Threat Detection](screenshots/threat-detection.png)

---

### 2. **Automation in Microsoft Sentinel**
One of Microsoft Sentinel primary purposes is to automate any recurring and predictable enrichment, response, and remediation tasks that are the responsibility of your Security Operations Centre and personnel (SOC/SecOps). Automation rules allow users to centrally manage the automation of incident handling. Automation rules also allow you to automate responses for multiple analytics rules at once. 
A playbook is a collection of response and remediation actions and logic that can be run from Microsoft Sentinel as a routine. A playbook can help automate and orchestrate your threat response. Playbooks in Microsoft Sentinel are based on workflows built in Azure Logic Apps, a cloud service that helps you schedule, automate, and orchestrate tasks and workflows across systems throughout the enterprise.


🔗 [View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/FMLNHLCX?sharingId=149F627F90730DC1)

📸 *Screenshot:*  
![Automation](screenshots/automation.png)

---

### 3. **Playbook-based Threat Response**
Security playbooks are collections of procedures based on Azure Logic Apps that run in response to an alert. You can run these security playbooks manually in response to your investigation of an incident or you can configure an alert to run a playbook automatically. 
Azure Logic Apps is a cloud service that automates the operation of your business processes. You use a graphical design tool called the Logic Apps Designer to arrange prebuilt components into the sequence you need. You can also use the code view and write your automated process in the JSON file.
Logic apps use connectors to connect to hundreds of services. A connector is a component that provides an interface to an external service.

🔗 [View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/ZB377DY2?sharingId=149F627F90730DC1)

📸 *Screenshot:*  
![Playbook Response](screenshots/playbook-response.png)

---

### 4. **Incident Management**
Incident management is the complete process of incident investigation, from incident creation to in-depth investigation and resolution. Alerts - Analytics rules generate alerts when they detect important security events. You can configure alerts to generate incidents. Incidents - Microsoft Sentinel creates incidents from analytics rule alerts. Events - Microsoft Sentinel stores events in a Log Analytics workspace. These events contain the details of security-related activity that you want Microsoft Sentinel to monitor.
Analytics rules - Analytics rules detect important security events and generate alerts. Incident evidence consists of the security event information and related Microsoft Sentinel assets that identify threats in the Microsoft Sentinel environment. Incident entity refers to a network or user resource that's involved with an event. The investigation graph lets you view timelines and relationships between incident resources.


🔗 [View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/URDHFED3?sharingId=149F627F90730DC1)

📸 *Screenshot:*  
![Incident Management](screenshots/incident-management.png)

---

### 5. **Behavioral Analytics**
As Microsoft Sentinel collects logs and alerts from all the connected data sources, it analyses and builds baseline behavioural profiles of your organization’s entities (users, hosts, IP addresses, applications etc.). The analysis is across the time and peer group horizon. Investigation Priority Score”. The score determines the probability of a specific user performing a specific activity based on behavioural learning of the user and their peers. Activities identified as the most abnormal receive the highest scores (on a scale of 0-10).
Types of entities are currently identified in Microsoft Sentinel:

User account, Host, IP address, Malware, File, Process, cloud application, Domain name (DNS), Azure resource, File (FileHash), Registry key, Registry value, Security group, URL, IoT device, Mailbox, Mail cluster, Mail message, Submission mail.

Timeline presents a story about entity-related events, helping you understand the entity's activity within a specific time frame.

Entity insights are queries defined by Microsoft security researchers to help your analysts investigate more efficiently and effectively. The insights are presented as part of the entity page, and provide valuable security information on hosts and users, in the form of tabular data and charts. Having the information here means you don't have to detour to Log Analytics. The insights include data regarding sign-ins, Group Additions, Anomalous Events and more, and include advanced ML algorithms to detect anomalous behavior. The insights are based on the following data types: Syslog, securityEvent, Audit Logs, Sign-in Logs, Office Activity, BehaviorAnalytics (UEBA)


🔗 [View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/URD8UKG3?sharingId=149F627F90730DC1)

📸 *Screenshot:*  
![Behavioral Analytics](screenshots/behavioral-analytics.png)

---

### 6. **Data Normalization with ASIM**
Data normalization in Microsoft Sentinel allows for the standardization of data across multiple data sources.

The Advanced Security Information Model (ASIM) is a layer that is located between these diverse sources and the user. ASIM provides a seamless experience for handling various sources in uniform, normalized views, by providing the following functionality:

•	Cross source detection. Normalized analytics rules work across sources, on-premises and cloud, and detect attacks such as brute force or impossible travel across systems, including Okta, AWS, and Azure.  
•	Source agnostic content. The coverage of both built-in and custom content using ASIM automatically expands to any source that supports ASIM, even if the source was added after the content was created. For example, process event analytics support any source that a customer may use to bring in the data, such as Microsoft Defender for Endpoint, Windows Events, and Sysmon.  
•	Support for your custom sources, in built-in analytics  
•	Ease of use. After an analyst learns ASIM, writing queries is simpler as the field names are always the same.

ASIM includes the following components: 1. Normalized schemas- Cover standard sets of predictable event types that you can use when building unified capabilities. 2. Parsers - Map existing data to the normalized schemas using KQL functions. 3. Content for each normalized schema- Includes analytics rules, workbooks, hunting queries, and more. Content for each normalized schema works on any normalized data without the need to create source-specific content.
Data Collection Rules (DCRs) provide an ETL-like pipeline in Azure Monitor, allowing you to define the way that data coming into Azure Monitor should be handled. two types of data collection rules in Azure Monitor: a) Standard DCR. Used with different workflows that send data to Azure Monitor. Workflows currently supported are Azure Monitor agent and custom logs. b) Workspace transformation DCR. Used with a Log Analytics workspace to apply ingestion-time transformations to workflows that don't currently support DCRs. Transformations in a data collection rule (DCR) allow you to filter or modify incoming data before it's stored in a Log Analytics workspace


🔗 [View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/NVLAHLDF?sharingId=149F627F90730DC1)

📸 *Screenshot:*  
![Data Normalization](screenshots/data-normalization.png)

---

### 7. **Log Analytics & Visualization**
The Log Analytics workspace is a repository that stores data and configuration information. 

Azure Data Explorer, which is also known as Kusto, is a log analytics cloud platform optimized for ad-hoc big data queries.


🔗 [View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/E5XDMA3P?sharingId=149F627F90730DC1)

📸 *Screenshot:*  
![Log Analytics](screenshots/log-analytics.png)

---

### 8. **Content Management via Content Hub**
Content hub: - Microsoft Sentinel solutions are packages of Microsoft Sentinel content or Microsoft Sentinel API integrations, which fulfill an end-to-end product, domain, or industry vertical scenario in Microsoft Sentinel.

Use the Microsoft Sentinel Content hub to centrally discover and install out-of-the-box (built-in) content. The Microsoft Sentinel Content Hub provides in-product discoverability, single-step deployment, and enablement of end-to-end product, domain, and/or vertical out-of-the-box solutions and content in Microsoft Sentinel.  
Microsoft Sentinel solutions are:  
•	Packaged content are collections of one or more pieces of Microsoft Sentinel content, such as data connectors, workbooks, analytics rules, playbooks, hunting queries, watchlists, parsers, and more.  
•	Integrations include services or tools built using Microsoft Sentinel or Azure Log Analytics APIs that support integrations between Azure and existing customer applications, or migrate data, queries, and more, from those applications into Microsoft Sentinel.  

You can also use solutions to install packages of out-of-the-box content in a single step, where the content is often ready to use immediately.


🔗 [View Badge](https://learn.microsoft.com/api/achievements/share/en-us/ianM-1267/9YBWL25U?sharingId=149F627F90730DC1)

📸 *Screenshot:*  
![Content Hub](screenshots/content-hub.png)

---

## 🏁 Conclusion

This assignment reinforces the hands-on use of Microsoft Sentinel in a real-world SecOps context, utilizing detection, automation, investigation, and content management capabilities to maintain a proactive cybersecurity posture.

---

