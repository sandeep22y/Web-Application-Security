# OWASP Top Ten for Agentic Applications 0.5

This document lists the top 10 security risks for Agentic (autonomous) AI applications, adapted from the OWASP Agentic AI guidance.

| **ID** | **Risk** | **Definition / Description** |
|--------|------------------------------|-------------------------------------------------------------|
| **ASI01** | Agent Behaviour Hijack | Manipulating an agent’s goals or plans to pursue attacker-aligned objectives. |
| **ASI02** | Tool Misuse and Exploitation | Tricking agents into using their tools in harmful or unintended ways. |
| **ASI03** | Identity & Privilege Abuse | Impersonating agents or escalating access through identity or authentication and access-permission weaknesses. |
| **ASI04** | Agentic Supply Chain Vulnerabilities | Introducing insecure models, agents, tools or artefacts that compromise agent integrity. |
| **ASI05** | Unexpected Code Execution (RCE) | Triggering unauthorized or unsafe code execution through agent behaviors. |
| **ASI06** | Memory & Context Poisoning | Corrupting agent memory or context to distort reasoning and decision-making. |
| **ASI07** | Insecure Inter-Agent Communication | Poisoning messages or abusing protocols between agents to alter behavior. |
| **ASI08** | Cascading Failures | Faults or hallucinations propagate through agents, causing compounded failures. |
| **ASI09** | Human-Agent Trust Exploitation | Exploiting over-trust or fatigue in human oversight to enable agent misuse, including model deceptive behaviors. |
| **ASI10** | Rogue Agents | Malicious or compromised agents acting autonomously to deceive, disrupt, or exfiltrate. |

> 📌 *This table highlights the primary security concerns to consider when building and deploying Agentic AI applications.*

