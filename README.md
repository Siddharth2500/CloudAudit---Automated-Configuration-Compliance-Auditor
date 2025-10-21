# 🚀 CloudAudit — Automated Configuration & Compliance Auditor

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg?logo=python&logoColor=white)  
![Tool](https://img.shields.io/badge/Compliance-Auditor-FF5252.svg?logo=shield)  
![Features](https://img.shields.io/badge/Features-Config-Checks-4CAF50.svg?logo=gear)  
![Reports](https://img.shields.io/badge/Reports-JSON-2196F3.svg?logo=json)  
![CI/CD](https://img.shields.io/badge/CI/CD-Ready-2088FF.svg?logo=githubactions)  
![Dependencies](https://img.shields.io/badge/Dependencies-None-green.svg?logo=python)

**CloudAudit** is a **Python 3** tool designed to scan cloud resource configurations and evaluate them against predefined rules for encryption, TLS, and public access. It’s built for cloud engineers and compliance teams, offering a lightweight and extensible way to audit infrastructure settings.

-----------

## 🛠 Tech & Languages

| Layer        | Tech / Format              | Purpose                              |
|--------------|----------------------------|--------------------------------------|
| Language     | **Python 3.10+**           | Main codebase                        |
| Core Logic   | JSON parsing + rule engine | Evaluate configurations              |
| Reports      | **JSON**                   | Output summary of audit results      |
| Execution    | Script / Colab / Notebook  | Flexible usage environment           |
| Logging      | Console output             | Quick human-readable feedback        |

---

## 🌐 Architecture

Flow:  
1. Step 1 – Load configuration JSON file containing cloud resources  
2. Step 2 – For each resource: check encryption enabled, TLS version, and public access flag  
3. Step 3 – Aggregate results and generate `audit_report.json` with compliant / non-compliant breakdown  
4. The report is ready to feed into CI/CD gates or dashboards  

---

## ▶️ Run CloudAudit

```bash
python cloudaudit.py --input data/configurations.json --output data/audit_report.json
