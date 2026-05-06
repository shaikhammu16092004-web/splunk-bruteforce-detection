
# 🔐 Splunk Brute Force Detection Project

# splunk-bruteforce-detection
Splunk SIEM project for detecting brute force attacks using Windows logs

## 📌 Overview
This project demonstrates how to detect brute force attacks using Splunk SIEM by analyzing Windows Security logs.

## 🛠️ Tools Used
- Splunk Enterprise
- Windows Event Logs

## 🔍 Key Event IDs
- 4624 → Successful Login
- 4625 → Failed Login

## 📊 Dashboard Features
- Top Event Codes
- Failed Login Attempts
- Event Trends Over Time
- Source-based Log Analysis

## 🚨 Detection Logic
Multiple failed login attempts from same account indicate potential brute force attack.

## 📸 Screenshots
<img width="1920" height="1040" alt="Splunk" src="https://github.com/user-attachments/assets/56febfc1-fb00-4b30-8e39-78c1448f7e35" />
<img width="1920" height="1040" alt="Splunk1" src="https://github.com/user-attachments/assets/bf3b6d0a-c956-487b-8f8b-d57d72e869af" />



## 📌 Sample SPL Query
index=windowslogs EventCode=4625
| stats count by Account_Name
| sort - count

## 🎯 Skills Gained
- Log Analysis
- SPL (Search Processing Language)
- SIEM Monitoring
- Threat Detection
  
