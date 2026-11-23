# Awesome-Autonomous-Penetration-Testing-Security-Swarms
# Awesome-Autonomous-Penetration-Testing-Security-Swarms

<FollowUp>
Would you like to **add a dedicated section for open-source cyber range environments & agent benchmarks** (like `CyberSecEval`, `SecBench`, `GHOSTS`, `DetectionLab`) or **generate the next `README.md` repository**?
</FollowUp>
# Awesome-Autonomous-Penetration-Testing-Security-Swarms

# Awesome Autonomous Penetration Testing & Security Swarms 🌟



> **Top Autonomous Penetration Testing Security Swarms (Opensource)**  

> A curated list of the best autonomous penetration testing platforms, continuous security validation tools, and multi-agent security swarms — with a strong focus on **open-source** and self-hostable alternatives.  

> 🌟 **Star if you like it!** 🌟



Autonomous penetration testing and security swarm systems use AI agents (often multi-agent architectures) to plan, recon, exploit, validate, and report on attack paths with minimal human intervention. Commercial platforms such as Horizon3 NodeZero, Pentera, and SafeBreach dominate the enterprise continuous-testing space, while a rapidly growing open-source ecosystem delivers self-hosted multi-agent pentest systems, LLM-driven agents, and swarm frameworks that run inside isolated sandboxes.



This list prioritizes **open-source GitHub projects** while keeping SaaS/hosted platforms clearly separated. **All tools listed are intended strictly for authorized security testing only.**



## Table of Contents



- [SaaS / Hosted Platforms](#saas--hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS / Hosted Platforms



These are popular commercial autonomous penetration testing, breach-and-attack simulation, and continuous security validation platforms (closed-source / hosted):



- **[Horizon3.ai NodeZero](https://www.horizon3.ai/)** — Fully autonomous penetration testing platform that continuously discovers and validates attack paths in enterprise environments.

- **[Pentera](https://www.pentera.io/)** — Automated security validation platform that safely emulates real attacker techniques across the attack surface.

- **[SafeBreach](https://www.safebreach.com/)** — Breach and attack simulation (BAS) platform focused on continuous validation of security controls.

- **[AttackIQ](https://www.attackiq.com/)** — Security control validation and adversary emulation platform aligned with MITRE ATT&CK.

- **[Cymulate](https://cymulate.com/)** — Continuous security validation and exposure management platform.

- **[Picus Security](https://www.picussecurity.com/)** — Breach and attack simulation + autonomous penetration testing capabilities.

- **[Cobalt.io](https://www.cobalt.io/)** — Pentest-as-a-Service platform with human + automation hybrid offerings.

- **[BreachLock](https://www.breachlock.com/)** — Continuous penetration testing and attack surface management.

- **[NetSPI](https://www.netspi.com/)** — Enterprise penetration testing and continuous security assessment services.

- **[HackerOne](https://www.hackerone.com/)** — Leading bug bounty and vulnerability disclosure platform (with emerging autonomous/AI features).



## Open-Source GitHub Projects



Open-source alternatives and tools you can self-host, run locally, or extend. These range from full multi-agent autonomous pentest platforms to specialized LLM-driven agents, security swarms, and supporting frameworks. Emphasis is placed on systems designed for authorized testing with sandbox isolation.



### Multi-Agent Autonomous Penetration Testing Platforms



- **[vxcontrol/pentagi](https://github.com/vxcontrol/pentagi)** (PentAGI)  

  Fully autonomous multi-agent system for complex penetration testing tasks. Specialized agents (planner, researcher, pentester, coder, reporter, etc.) coordinate, run 20+ professional tools (nmap, Metasploit, sqlmap, etc.) inside isolated Docker sandboxes, maintain long-term memory, and produce reports. Supports many LLM providers (cloud + local/Ollama). Web UI, REST/GraphQL APIs. MIT license. Highly active and widely adopted (~35k stars).



- **[Armur-Ai/Pentest-Swarm-AI](https://github.com/Armur-Ai/Pentest-Swarm-AI)**  

  Open-source autonomous AI pentester using a real swarm of concurrent recon, exploit, and report agents. Targets web apps and REST/GraphQL APIs, verifies findings with non-LLM oracles, and supports Claude, Gemini, OpenAI-compatible, and local Ollama models. Designed as an open alternative to certain commercial autonomous testers. AGPL-3.0.



- **[s0ld13rr/pentestcode](https://github.com/s0ld13rr/pentestcode)** (and related forks)  

  Multi-agent AI penetration testing system with persistent engagement state, strategic coordination, and parallel autonomous operations. Lead agent dispatches specialized sub-agents (recon, scanner, enumerator, exploiter, identity/AD, webapp, post-exploit, critic, reporter, etc.). Terminal-focused with support for many LLM providers.



### LLM-Driven Autonomous Pentest Agents



- **[GreyDGL/PentestGPT](https://github.com/GreyDGL/PentestGPT)**  

  Pioneering automated penetration testing agentic framework powered by large language models (USENIX Security 2024). Multi-stage pipeline (recon → exploit → reporting), session persistence, and autonomous operation. Strong research foundation and continued community use.



- **[Vasco0x4/AIDA](https://github.com/Vasco0x4/AIDA)**  

  Turns any LLM into an autonomous pentester. You define the scope; the agent reasons, executes commands inside an isolated Docker container loaded with classic tools (nmap, sqlmap, ffuf, nuclei, etc.), and documents findings with the exact commands used. Human review of results is built into the workflow.



- **Other notable agents**: Projects such as Strix, Shannon, HexStrike AI, and various research prototypes (search for current high-star autonomous pentest agents) that wire LLMs to tool execution loops for recon, exploitation, and reporting.



### Supporting Open-Source Tools & Frameworks



- **OWASP Nettacker** and similar automated security testing frameworks that can serve as building blocks or be orchestrated by agent systems.

- **MCP-based security tool bridges** (e.g., HexStrike-style MCP servers) that expose nmap, nuclei, sqlmap, and other tools to coding/agent frameworks.

- Local LLM + MCP combinations (e.g., Unburden-style assistants) that let agents drive offensive workflows with local models.

- Classic open-source offensive tooling ecosystems (Metasploit, BloodHound, Impacket, etc.) that modern agent platforms typically wrap inside sandboxes.



> **Tip**: For full multi-agent autonomy with strong isolation, start with **PentAGI**. For research-grade or lighter autonomous loops, **PentestGPT** and **AIDA** are excellent entry points. Always run agents inside proper sandboxes/containers and only against systems you are explicitly authorized to test. Prefer projects that enforce human review of findings and maintain clear audit logs.



## How to Contribute



Contributions are welcome and encouraged!



1. Fork the repository

2. Add a new tool under the appropriate section (keep SaaS and Open-Source strictly separate)

3. Use the same format: **Name** — short description + key features + license/link

4. Prefer actively maintained projects with clear documentation, sandbox isolation, and explicit authorized-use guidance

5. Submit a Pull Request



Please keep descriptions neutral and factual. Open-source projects are the primary focus of this list. Do not add tools that appear designed primarily for unauthorized use.



## Disclaimer



This is a community-curated list for informational and educational purposes only.  

**Inclusion does not constitute an endorsement.**  



**Critical legal and ethical notice**: Autonomous penetration testing tools must be used **only** on systems you own or have explicit, written authorization to test. Unauthorized access, scanning, or exploitation is illegal in most jurisdictions and can result in severe civil and criminal penalties. Always obtain proper scope and authorization before running any tool.



Review licenses, security practices, sandboxing behavior, model usage costs, and potential risks carefully. Some projects may have dual licensing, commercial cloud offerings, or require paid API keys. Check the actual LICENSE file and documentation. Agents can execute real commands and make lasting changes — use isolated environments, version control of findings, and human oversight.



The maintainers of this list assume no responsibility for misuse of any listed software.



---



**Made with ❤️ for the open-source security community**  

If this list helped you, please ⭐ the repo!  

**Authorized testing only.**
