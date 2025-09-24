# 🛡️ OWASP Top 10 for LLM Applications  

This repository provides an overview of the **OWASP Top 10 Security Risks for Large Language Model (LLM) Applications**, including definitions and actionable recommendations for mitigation.  

LLMs (like GPT, Claude, and others) introduce unique security challenges. This guide helps developers, security professionals, and researchers secure their LLM-based applications.  

---

## 📋 Table of Contents  

- [Overview](#overview)  
- [OWASP Top 10 for LLM](#owasp-top-10-for-llm)  
- [How to Use This Guide](#how-to-use-this-guide)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Overview  

The **OWASP Top 10 for LLM Applications** is inspired by the classic OWASP Top 10 but adapted for Large Language Models. It highlights the most critical security risks when building, integrating, or deploying LLM-powered applications.  

---

## 📝 OWASP Top 10 for LLM  

| **#** | **Category** | **Definition** | **Recommendations** |
|-------|--------------|----------------|---------------------|
| **LLM01** | **Prompt Injection** | Malicious inputs manipulate the LLM to execute unintended actions or reveal sensitive data. | Input validation, prompt isolation, restrict sensitive functions, output filtering. |
| **LLM02** | **Insecure Output Handling** | LLM-generated outputs may contain unsafe or malicious content (HTML/JS injection, harmful instructions). | Treat output as untrusted input, escape/encode, use content filters, human review. |
| **LLM03** | **Training Data Poisoning** | Attackers insert malicious data into training datasets causing biased or unsafe model behavior. | Use curated datasets, anomaly detection, versioning & provenance logs, retraining audits. |
| **LLM04** | **Model Denial of Service** | Overloading the LLM to consume excessive resources causing downtime. | Rate-limits, monitor resource spikes, caching, quotas per user/API key. |
| **LLM05** | **Supply Chain Vulnerabilities** | Third-party models, datasets, or libraries introduce vulnerabilities or backdoors. | Vet external components, verify signatures/checksums, update dependencies, security assessments. |
| **LLM06** | **Sensitive Information Disclosure** | LLM reveals confidential or personal data from training data or context. | Apply differential privacy, redact sensitive data, limit RAG scope, monitor outputs for leaks. |
| **LLM07** | **Insecure Plugin/API Integration** | Unsafe integration with plugins or APIs executes unintended actions. | Least-privilege for plugin APIs, validate & restrict calls, log/monitor, allowlists. |
| **LLM08** | **Excessive Agency** | LLM given too much autonomy (executing code or transactions) without controls. | Human-in-the-loop approval, granular permissions, restrict system-level access, RBAC. |
| **LLM09** | **Overreliance on LLM Output** | Blind trust in LLM outputs leads to misinformation or harmful decisions. | User education, cross-verify critical outputs, provide confidence scores, fact-check modules. |
| **LLM10** | **Model Theft** | Unauthorized access or exfiltration of proprietary LLM models. | Encrypt weights/storage, API access controls, watermarking/fingerprinting, monitor anomalies. |

---

## 🚀 How to Use This Guide  

- 📚 **Developers:** Use as a checklist while building LLM-powered apps.  
- 🛡️ **Security Teams:** Integrate these risks into your threat models and penetration tests.  
- 🧪 **Researchers:** Explore new mitigations and share improvements.  

---

## 🤝 Contributing  

Contributions are welcome!  
If you’d like to improve definitions, add recommendations, or share references:  

1. Fork the repo  
2. Create a new branch (`feature/your-feature`)  
3. Submit a pull request  

---

## 📜 License  

This project is licensed under the [MIT License](LICENSE).  

---

### ⭐ Support  

If you find this guide useful, please give it a ⭐ on GitHub to help others discover it!
