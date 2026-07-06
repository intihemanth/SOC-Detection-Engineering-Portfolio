<html><body>
<!--StartFragment--><html><head></head><body>
<h1>🛡️ SOC &amp; Detection Engineering Portfolio</h1>
<p><strong>Hemanth Inti</strong> · SOC Analyst L2 · MSSP-based SOC Operations</p>
<p><a href="https://linkedin.com/in/inti-hemanth/"><img src="https://img.shields.io/badge/LinkedIn-inti--hemanth-0A66C2?style=flat-square&amp;logo=linkedin&amp;logoColor=white" alt="LinkedIn"></a>
<img src="https://img.shields.io/badge/Focus-Detection%20Engineering-critical?style=flat-square" alt="Focus">
<img src="https://img.shields.io/badge/KQL-Primary-blue?style=flat-square" alt="KQL">
<img src="https://img.shields.io/badge/YARA--L-Secondary-blueviolet?style=flat-square" alt="YARA--L"></p>

<hr>
<h2>👋 About Me</h2>
<p>I'm a SOC Analyst L2 with ~3 years of experience in 24x7 enterprise security operations at an MSSP, working across Microsoft Defender XDR, Microsoft Sentinel, Google SecOps (Chronicle), and Proofpoint. This repository is where I document detection logic, threat research, and incident response methodology outside of client-specific work — built to demonstrate practical detection engineering thinking, not just tool familiarity.</p>
<h3>🧰 Stack</h3>
<p><img src="https://img.shields.io/badge/-Microsoft%20Defender%20XDR-0078D4?style=flat-square&amp;logo=microsoft&amp;logoColor=white" alt="Defender XDR">
<img src="https://img.shields.io/badge/-Microsoft%20Sentinel-0078D4?style=flat-square&amp;logo=microsoft&amp;logoColor=white" alt="Sentinel">
<img src="https://img.shields.io/badge/-Google%20SecOps%20(Chronicle)-4285F4?style=flat-square&amp;logo=google&amp;logoColor=white" alt="Chronicle">
<img src="https://img.shields.io/badge/-Proofpoint-E31937?style=flat-square" alt="Proofpoint">
<img src="https://img.shields.io/badge/-Entra%20ID-0078D4?style=flat-square&amp;logo=microsoft&amp;logoColor=white" alt="Entra ID">
<img src="https://img.shields.io/badge/-Wiz-611BBD?style=flat-square" alt="Wiz">
<img src="https://img.shields.io/badge/-Google%20Threat%20Intelligence-4285F4?style=flat-square&amp;logo=google&amp;logoColor=white" alt="GTI">
<img src="https://img.shields.io/badge/-ServiceNow-00C7D4?style=flat-square&amp;logo=servicenow&amp;logoColor=white" alt="ServiceNow">
<img src="https://img.shields.io/badge/-JIRA-0052CC?style=flat-square&amp;logo=jira&amp;logoColor=white" alt="JIRA"></p>
<h3>🎓 Certifications</h3>
<p><img src="https://img.shields.io/badge/CompTIA-Security%2B%20(SY0--701)-EE0000?style=flat-square" alt="Security+">
<img src="https://img.shields.io/badge/Microsoft-SC--200-0078D4?style=flat-square" alt="SC-200">
<img src="https://img.shields.io/badge/Google-Professional%20Security%20Operations%20Engineer-4285F4?style=flat-square" alt="Google SOE">
<img src="https://img.shields.io/badge/Google-Associate%20Cloud%20Engineer-4285F4?style=flat-square" alt="Google ACE">
<img src="https://img.shields.io/badge/Microsoft-AZ--900-0078D4?style=flat-square" alt="AZ-900">
<img src="https://img.shields.io/badge/AWS-Certified%20Cloud%20Practitioner-FF9900?style=flat-square" alt="AWS CCP"></p>
<hr>
<h2>🎯 What This Repo Demonstrates</h2>
<p>This isn't a collection of copy-pasted queries — every piece here reflects my own reasoning about <em>why</em> a detection is written the way it is, what it maps to in MITRE ATT&amp;CK, and where the false-positive tradeoffs live. Everything referencing real-world incidents draws only from <strong>publicly reported</strong> threat intel; no client data, proprietary employer detection logic, or confidential information appears anywhere in this repo.</p>
<h2>🗂️ Repository Structure</h2>
<pre><code>soc-detection-portfolio/
├── detections/            # Standalone KQL / YARA-L detection rules, one technique per folder
│   ├── oauth-token-abuse/
│   ├── impossible-travel/
│   └── living-off-the-land/
├── campaign-analysis/      # Deep-dives on named, publicly reported threat campaigns
│   ├── klue-oauth-supply-chain/
│   └── unc3886-singapore-telco/
├── methodology/            # General IR/detection frameworks and process writeups
│   └── multi-vector-ir-recovery/
├── threat-intel-notes/      # Shorter trend/summary writeups synthesizing public CTI
│   └── 2026-07-supply-chain-trends.md
└── homelab/                # Attack simulations (Atomic Red Team) + logs + detections validated end-to-end
    └── atomic-red-team-t1550/
</code></pre>

Folder | What's inside
-- | --
detections/ | Each folder = one technique. Contains a detection.kql and/or detection.yaral query plus a README.md with MITRE mapping, tuning notes, and a sample log.
campaign-analysis/ | Named, publicly reported campaigns broken down into TTPs, cited IOCs, and matching detection logic.
methodology/ | Process-level writeups — incident response frameworks, remediation workflows, and the reasoning behind them (not tied to a specific named campaign). 
threat-intel-notes/ | Periodic shorter-form trend summaries across multiple public sources.
homelab/ | Simulated attacks (via Atomic Red Team or similar) with raw logs and the detection logic that catches them — fully self-contained, zero client dependency.


<h2>📌 A Note on Sourcing</h2>
<p>Any IOC, technique detail, or campaign fact referenced in this repo is drawn from and cited to public vendor/CTI reporting (e.g., Microsoft, Mandiant, CrowdStrike blogs). Detection logic is my own, written to be illustrative of the technique rather than copied from any employer's internal rule set.</p>
<hr>
<p><strong>📫 Connect with me on <a href="https://linkedin.com/in/inti-hemanth/">LinkedIn</a></strong> — I write a running series on practitioner-level SOC analysis and detection engineering there too.</p>
</body></html><!--EndFragment-->
</body>
</html>

