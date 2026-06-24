# Awesome Embodied AI Governance

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated map of research, standards, regulation, runtime controls,
> assurance methods, and evaluation resources for AI systems that perceive,
> decide, and act in the physical world.

Embodied AI governance begins where model behavior becomes physical action. It
includes conventional machine and robot safety, but also identity, permissions,
human intervention, observability, evidence continuity, software supply-chain
security, and lifecycle governance for learning systems that change after
deployment.

**Last reviewed:** June 16, 2026

## Contents

- [Start here](#start-here)
- [Core research and surveys](#core-research-and-surveys)
- [Safety standards](#safety-standards)
- [AI management and assurance standards](#ai-management-and-assurance-standards)
- [Regulation and public frameworks](#regulation-and-public-frameworks)
- [Runtime governance and authorization](#runtime-governance-and-authorization)
- [Robot identity and communications security](#robot-identity-and-communications-security)
- [Supply-chain and update integrity](#supply-chain-and-update-integrity)
- [Telemetry, provenance, and evidence](#telemetry-provenance-and-evidence)
- [Human oversight and intervention](#human-oversight-and-intervention)
- [Simulation and test environments](#simulation-and-test-environments)
- [Safety and governance evaluation](#safety-and-governance-evaluation)
- [Threat modeling and red teaming](#threat-modeling-and-red-teaming)
- [Incident learning](#incident-learning)
- [Reference implementations](#reference-implementations)
- [Curation notes](#curation-notes)
- [Contributing](#contributing)

## Start here

- [ISO Robotics sector](https://www.iso.org/sectors/engineering/robotics) -
  Current ISO robotics standards and work in progress from ISO/TC 299.
- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) -
  Cross-sector AI risk framework organized around Govern, Map, Measure, and
  Manage.
- [EU Artificial Intelligence Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng) -
  Official regulation text, including high-risk system obligations relevant to
  AI safety components in regulated products.
- [European Commission AI Act portal](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) -
  Implementation timeline, guidance, service desk, and AI Office resources.
- [ROS 2 Security](https://docs.ros.org/en/rolling/Concepts/Intermediate/About-Security.html) -
  Authentication, encryption, integrity, and access control for ROS graphs.
- [Harnessing Embodied Agents](https://arxiv.org/abs/2604.07833) - Runtime
  governance framing that separates agent cognition from policy-constrained
  execution oversight.
- [EmbodiedGovBench](https://arxiv.org/abs/2604.11174) - Benchmark proposal for
  controllability, policy boundaries, recovery, auditability, human override,
  and upgrade safety.

## Core research and surveys

- [Embodied AI: Emerging Risks and Opportunities for Policy Action](https://arxiv.org/abs/2509.00117) -
  Policy-oriented risk map for physical harm, surveillance, labor, security,
  and institutional readiness.
- [The Biggest Risk of Embodied AI is Governance Lag](https://arxiv.org/abs/2604.21938) -
  Argument for treating deployment speed, observability, and public-sector
  response capacity as first-order risks.
- [Harnessing Embodied Agents: Runtime Governance for Policy-Constrained Physical Execution](https://arxiv.org/abs/2604.07833) -
  Runtime governance layer for policy enforcement, authorization, audit, and
  intervention around embodied agents.
- [Safety in Embodied AI](https://arxiv.org/abs/2505.15417) - Survey of risks,
  attacks, defenses, benchmarks, and evaluation methods for embodied agents.
- [Safety of Embodied Navigation](https://arxiv.org/abs/2508.05855) - Survey of
  attacks, defenses, robustness, and verification in embodied navigation.
- [SoK: Security and Privacy of Foundation-Model-Powered Robots](https://arxiv.org/abs/2606.16788) -
  Systematization of security and privacy risks in robots using foundation
  models.
- [Trust in LLM-controlled Robotics](https://arxiv.org/abs/2601.02377) - Survey
  of security threats and trust issues in language-model-controlled robots.
- [Vision-Language-Action Safety](https://arxiv.org/abs/2604.23775) - Survey of
  safety threats, evaluations, and mitigation directions for VLA models.
- [Foundation Models in Robotics](https://arxiv.org/abs/2604.15395) - Broad
  review of robotic foundation models, useful for understanding the governed
  system stack.
- [Open X-Embodiment](https://robotics-transformer-x.github.io/) - Cross-robot
  dataset and RT-X model work that motivates governance for transferable robot
  policies.
- [Physical AI: A Primer for Policymakers on AI-Robotics Convergence](https://cset.georgetown.edu/publication/physical-ai/) -
  Policy primer on AI-robotics convergence, supply chains, competitive dynamics,
  and public-policy considerations.

## Safety standards

Standards often require purchase. Links below point to official abstracts,
catalog entries, or standards-body resources.

- [ISO 10218-1:2025](https://www.iso.org/standard/73933.html) - Safety
  requirements for industrial robot design before integration.
- [ISO 10218-2:2025](https://www.iso.org/standard/73934.html) - Safety
  requirements for industrial robot applications and robot cells.
- [ISO/TS 15066:2016](https://www.iso.org/standard/62996.html) - Collaborative
  robot system and work-environment guidance.
- [ISO 13482:2014](https://www.iso.org/standard/53820.html) - Current published
  safety requirements for personal care robots, expected to be replaced by the
  ISO/FDIS 13482 revision.
- [ISO/FDIS 13482](https://www.iso.org/standard/83498.html) - Final draft
  second edition covering service robots for personal and professional use.
- [ISO 12100:2010](https://www.iso.org/standard/51528.html) - Machinery risk
  assessment and risk-reduction methodology.
- [ISO 13849-1:2023](https://www.iso.org/standard/73481.html) - Safety-related
  parts of control systems, including software-related design guidance.
- [IEC 62061:2021](https://webstore.iec.ch/en/publication/59927) - Functional
  safety requirements for safety-related machine control systems.
- [ISO 13850:2015](https://www.iso.org/standard/59970.html) - Emergency stop
  function requirements and design principles for machinery.
- [IEC 61508 functional safety](https://www.iec.ch/functionalsafety) - General
  functional-safety framework for electrical, electronic, and programmable
  electronic safety-related systems.
- [IEC 62443 overview](https://www.iec.ch/blog/understanding-iec-62443) -
  Cybersecurity for industrial automation and control systems.
- [ISA/IEC 62443 series](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) -
  Industrial automation and control security requirements and processes.
- [ISO 3691-4:2023](https://www.iso.org/standard/83545.html) - Driverless
  industrial trucks, AGVs, and autonomous mobile robot systems.
- [ISO/TR 23482-1:2020](https://www.iso.org/standard/71539.html) - Test methods
  supporting ISO 13482.
- [ISO/TR 23482-2:2019](https://www.iso.org/standard/71627.html) - Application
  guidance supporting ISO 13482.
- [UL 4600](https://ulse.org/focus-areas/travel-safety/autonomous-vehicles/) -
  Safety case standard for fully autonomous products, including validation of
  machine-learning autonomy functions.
- [ISO 26262:2018](https://www.iso.org/standard/68383.html) - Functional safety
  for road-vehicle electrical and electronic systems.
- [ISO 21448:2022](https://www.iso.org/standard/77490.html) - Safety of the
  intended functionality for road vehicles, including performance insufficiency
  and foreseeable misuse.
- [ISO/SAE 21434:2021](https://www.iso.org/standard/70918.html) - Road-vehicle
  cybersecurity engineering over the lifecycle.

## AI management and assurance standards

- [ISO/IEC 42001:2023](https://www.iso.org/standard/42001) - AI management
  system requirements for organizations developing, providing, or using AI.
- [ISO/IEC 23894:2023](https://www.iso.org/standard/77304.html) - Guidance for
  AI-related risk management.
- [ISO/IEC 22989:2022](https://www.iso.org/standard/74296.html) - AI concepts
  and terminology.
- [ISO/IEC 23053:2022](https://www.iso.org/standard/74438.html) - Framework for
  describing AI systems using machine learning.
- [ISO/IEC 42005:2025](https://www.iso.org/standard/42005) - AI system
  impact assessment guidance.
- [IEEE 7000-2021](https://standards.ieee.org/standard/7000-2021.html) -
  Process standard for addressing ethical concerns during system design.
- [Goal Structuring Notation](https://scsc.uk/gsn) - Assurance-case notation
  used to structure safety and security arguments with evidence.
- [OMG Structured Assurance Case Metamodel](https://www.omg.org/spec/SACM/) -
  Standard metamodel for exchanging structured assurance cases.

## Regulation and public frameworks

- [EU Artificial Intelligence Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng) -
  Risk-based AI regulation covering prohibited practices, high-risk systems,
  GPAI models, transparency, logging, human oversight, robustness, and
  post-market monitoring.
- [European Commission AI Act portal](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) -
  Official implementation timeline; as of June 2026, embedded high-risk product
  rules are listed as applying from 2 August 2028 after the AI omnibus political
  agreement.
- [EU Machinery Regulation](https://eur-lex.europa.eu/eli/reg/2023/1230/oj/eng) -
  Health and safety requirements for machinery, including software and evolving
  autonomous behavior.
- [EU Cyber Resilience Act](https://eur-lex.europa.eu/eli/reg/2024/2847/oj/eng) -
  Horizontal cybersecurity obligations for products with digital elements.
- [EU Product Liability Directive](https://eur-lex.europa.eu/eli/dir/2024/2853/oj/eng) -
  Defective-product liability rules covering software and AI-enabled products.
- [EU General Product Safety Regulation](https://eur-lex.europa.eu/eli/reg/2023/988/oj/eng) -
  Consumer product safety regime relevant to connected and AI-enabled physical
  products.
- [NIST AI RMF 1.0](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf) -
  Voluntary framework for trustworthy and responsible AI risk management.
- [NIST AI RMF Playbook](https://airc.nist.gov/airmf-resources/playbook/) -
  Suggested actions aligned to the AI RMF outcomes.
- [NIST Generative AI Profile](https://doi.org/10.6028/NIST.AI.600-1) -
  Companion profile for generative AI risks and risk-management actions.
- [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework) -
  Cybersecurity governance and risk-management framework.
- [NIST Secure Software Development Framework](https://csrc.nist.gov/pubs/sp/800/218/final) -
  Secure software development practices relevant to robot and agent control
  stacks.
- [NIST adversarial machine-learning taxonomy](https://csrc.nist.gov/pubs/ai/100/2/e2025/final) -
  Taxonomy and terminology for adversarial ML attacks and mitigations.
- [CISA Zero Trust Maturity Model](https://www.cisa.gov/zero-trust-maturity-model) -
  Identity, device, network, workload, data, visibility, automation, and
  governance maturity model.
- [NISTIR 8228](https://csrc.nist.gov/pubs/ir/8228/final) - Cybersecurity and
  privacy risk management considerations for IoT devices.
- [ENISA Good Practices for Security of IoT in Smart Manufacturing](https://www.enisa.europa.eu/publications/good-practices-for-security-of-iot) -
  Industrial IoT security guidance and threat scenarios for manufacturing.
- [NHTSA Standing General Order on Crash Reporting](https://www.nhtsa.gov/laws-regulations/standing-general-order-crash-reporting) -
  US crash-reporting regime for ADS and Level 2 ADAS-equipped vehicles.
- [NHTSA Voluntary Safety Self-Assessment](https://www.nhtsa.gov/automated-driving-systems/voluntary-safety-self-assessment) -
  Public disclosure index for ADS safety self-assessments.
- [FAA Roadmap for AI Safety Assurance](https://www.faa.gov/media/82891) -
  Aviation safety-assurance roadmap for AI and machine learning.
- [International AI Safety Report 2026](https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026) -
  International expert assessment of advanced AI capabilities, risks, and
  safeguards, including agentic risks.

## Runtime governance and authorization

- [Open Policy Agent](https://www.openpolicyagent.org/docs/latest/) - General
  policy-as-code engine using Rego.
- [Cedar](https://docs.cedarpolicy.com/) - Authorization policy language and
  evaluator designed for fine-grained permissions.
- [OpenFGA](https://openfga.dev/docs) - Relationship-based authorization
  modeled on Zanzibar-style access control.
- [Casbin](https://casbin.org/docs/overview) - Authorization library supporting
  ACL, RBAC, ABAC, and related access-control models.
- [Kubernetes admission control](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/) -
  Pattern for policy checks at resource mutation boundaries.
- [ROS 2 lifecycle nodes](https://design.ros2.org/articles/node_lifecycle.html) -
  Managed node states useful for controlled activation, deactivation, recovery,
  and shutdown.
- [Action-bound approval protocol](https://github.com/microsoft/agent-governance-toolkit/pull/2953) -
  Proposal for binding human approval to a specific action, arguments,
  principal, policy, and execution context.
- [Physical-agent risk mapping](https://github.com/microsoft/agent-governance-toolkit/pull/2916) -
  Mapping of agentic risks to systems with actuators and physical effects.

Useful runtime questions:

- Which principal is asking the system to act?
- Which capability boundary, environment, and safety envelope apply?
- Which policy version authorized the action?
- Is the approval bound to the exact command, object, location, and time?
- What happens if policy service, identity provider, telemetry, or network
  connectivity fails?
- Can the system move to a known safe state without the model cooperating?

## Robot identity and communications security

- [ROS 2 security concepts](https://docs.ros.org/en/rolling/Concepts/Intermediate/About-Security.html) -
  DDS-Security-backed identity, encryption, integrity, and access control.
- [ROS 2 security setup](https://docs.ros.org/en/rolling/Tutorials/Advanced/Security/Introducing-ros2-security.html) -
  Practical SROS2 keystore and enclave tutorial.
- [ROS 2 access controls](https://docs.ros.org/en/rolling/Tutorials/Advanced/Security/Access-Controls.html) -
  Permission policies for ROS nodes, topics, and services.
- [ROS 2 security deployment guidelines](https://docs.ros.org/en/rolling/Tutorials/Advanced/Security/Deployment-Guidelines.html) -
  Guidance for distributing and protecting security material.
- [SROS2](https://github.com/ros2/sros2) - ROS 2 tooling for keys,
  certificates, and security policies.
- [DDS Security specification](https://www.omg.org/spec/DDS-SECURITY/) -
  Authentication, access control, cryptography, logging, and data tagging for
  DDS systems.
- [SPIFFE and SPIRE](https://spiffe.io/docs/latest/) - Workload identity and
  attestation for distributed systems.
- [FIDO Device Onboard](https://fidoalliance.org/specifications/download-iot-specifications/) -
  Device onboarding specification useful for fleet identity provisioning.

## Supply-chain and update integrity

- [SLSA](https://slsa.dev/) - Supply-chain security levels and provenance.
- [in-toto](https://in-toto.io/) - Supply-chain layout and verification for
  software artifacts.
- [Sigstore](https://docs.sigstore.dev/) - Signing and verification for
  software artifacts and identities.
- [The Update Framework](https://theupdateframework.io/) - Resilient software
  update design for remote fleets and edge devices.
- [Uptane](https://uptane.org/) - Secure software update framework designed for
  automotive electronic control units and vehicle fleets.
- [SPDX](https://spdx.dev/) - Open SBOM standard for software components,
  provenance, security, and related references.
- [CycloneDX](https://cyclonedx.org/) - BOM standard for software, hardware,
  AI/ML, cryptography, services, and operations transparency.
- [OpenSSF Scorecard](https://scorecard.dev/) - Automated checks for open-source
  project supply-chain hygiene.

## Telemetry, provenance, and evidence

- [OpenTelemetry](https://opentelemetry.io/docs/) - Vendor-neutral traces,
  metrics, and logs.
- [OpenTelemetry semantic conventions](https://opentelemetry.io/docs/specs/semconv/) -
  Standardized names and attributes for telemetry.
- [W3C PROV overview](https://www.w3.org/TR/prov-overview/) - Data model for
  representing entities, activities, agents, and provenance.
- [OpenLineage](https://openlineage.io/docs/) - Open standard for lineage
  events and integrations.
- [CloudEvents](https://cloudevents.io/) - Common envelope for describing
- [Nobulex](https://github.com/arian-gogani/nobulex) - Ed25519-signed, JCS-canonical (RFC 8785) action receipts for AI agents. Pre/post execution bilateral receipts, hash-chained, independently verifiable without operator trust. EU AI Act Article 12 compliance primitive.
  events across services and platforms.
- [Transparency.dev](https://transparency.dev/) - Patterns for append-only,
  publicly verifiable records.
- [C2PA specifications](https://spec.c2pa.org/specifications/specifications/2.4/index.html) -
  Content provenance standards useful for images, video, and sensor-derived
  media.

Useful evidence questions:

- Which identity requested, planned, authorized, and executed the action?
- Which policy, model, prompt, map, and controller versions were active?
- What observations and uncertainty estimates informed the decision?
- Was human approval bound to the exact action and context?
- Were safety interlocks, overrides, and emergency stops observed?
- Can the record survive a controller restart and be checked for tampering?
- Can audit records be replayed in simulation without leaking sensitive data?

## Human oversight and intervention

- [NIST AI RMF Playbook](https://airc.nist.gov/airmf-resources/playbook/) -
  Human-AI configuration, roles, responsibilities, and intervention practices.
- [ISO 10218-2:2025](https://www.iso.org/standard/73934.html) - Integration and
  operational safety requirements for industrial robot applications and cells.
- [ISO 13850:2015](https://www.iso.org/standard/59970.html) - Emergency stop
  function requirements and design principles.
- [ROS 2 lifecycle nodes](https://design.ros2.org/articles/node_lifecycle.html) -
  Managed states useful for controlled activation, deactivation, recovery, and
  shutdown.
- [NHTSA Standing General Order on Crash Reporting](https://www.nhtsa.gov/laws-regulations/standing-general-order-crash-reporting) -
  Example of regulator-facing incident reporting tied to automated driving
  oversight.
- [FAA Roadmap for AI Safety Assurance](https://www.faa.gov/media/82891) -
  Assurance planning for AI in aviation, a useful comparison domain for
  high-assurance embodied systems.

Oversight should be tested as behavior, not documented as intent: loss of
operator attention, delayed takeover, stale approval, unavailable supervisor,
ambiguous command, control-room handoff, network partition, and emergency-stop
recovery all deserve explicit scenarios.

## Simulation and test environments

- [MuJoCo](https://mujoco.readthedocs.io/) - Fast physics simulation for
  control, state estimation, and contact-rich tasks.
- [Gazebo Sim](https://gazebosim.org/libs/sim/) - Open robotics simulator with
  physics, rendering, sensors, plugins, and message interfaces.
- [NVIDIA Isaac Sim](https://docs.isaacsim.omniverse.nvidia.com/latest/) -
  GPU-accelerated robotics simulation and synthetic data generation.
- [Isaac Lab](https://isaac-sim.github.io/IsaacLab/) - Robot-learning framework
  built on Isaac Sim.
- [Webots](https://cyberbotics.com/doc/guide/index) - General-purpose
  open-source robot simulator.
- [robosuite](https://robosuite.ai/docs/overview.html) - MuJoCo-based
  manipulation environments and standardized robot tasks.
- [Safety-Gymnasium](https://safety-gymnasium.readthedocs.io/) - Safe
  reinforcement-learning environments and evaluation tooling.
- [BEHAVIOR-1K](https://behavior.stanford.edu/) - Benchmark and simulation
  environment for 1,000 household activities.
- [AI2-THOR](https://ai2thor.allenai.org/) - Interactive 3D household
  environments for embodied AI agents.
- [Habitat](https://aihabitat.org/) - Embodied AI simulator and benchmark suite
  for navigation and interaction.
- [ManiSkill](https://maniskill.readthedocs.io/) - GPU-accelerated robotic
  manipulation benchmark and learning environments.
- [RoboCasa](https://robocasa.ai/) - Simulation framework for everyday robotics
  tasks in diverse kitchen environments.
- [CARLA](https://carla.org/) - Open simulator for autonomous driving research.
- [nuPlan](https://www.nuscenes.org/nuplan) - Planning benchmark and dataset for
  autonomous driving.

Governance tests should cover more than task success: unauthorized capability
use, restricted zones, stale approvals, identity loss, policy unavailability,
sensor uncertainty, emergency stop, restart recovery, upgrade rollback, and
evidence completeness.

## Safety and governance evaluation

- [EmbodiedGovBench](https://arxiv.org/abs/2604.11174) - Benchmark proposal for
  policy boundaries, recovery, override responsiveness, audit completeness, and
  upgrade safety.
- [AGENTSAFE](https://arxiv.org/abs/2506.14697) - Safety benchmark for embodied
  VLM agents under hazardous and jailbroken instructions.
- [SafeAgentBench](https://arxiv.org/abs/2412.13178) - Safe task-planning
  benchmark for embodied LLM agents, with the ThinkSafe safety-checking module.
- [EAsafetyBench](https://www.ijcai.org/proceedings/2025/0867.pdf) - Embodied
  agent input-safety benchmark and moderation framework.
- [IS-Bench](https://arxiv.org/abs/2506.16402) - Interactive safety benchmark
  for VLM-driven embodied agents in household tasks.
- [DESPITE](https://arxiv.org/abs/2604.18463) - Deterministic evaluation of
  physical and normative dangers in embodied planning.
- [ForesightSafety Bench](https://arxiv.org/abs/2602.14135) - Frontier-risk
  benchmark that includes embodied robot control scenarios.
- [Generating Robot Constitutions and Benchmarks for Semantic Safety](https://arxiv.org/abs/2503.08663) -
  Constitution and benchmark generation for semantic robot safety.
- [ASIMOV benchmark for Gemini Robotics](https://deepmind.google/blog/gemini-robotics-15-brings-ai-agents-into-the-physical-world/) -
  Google DeepMind benchmark collection for semantic safety in robotics.
- [SafeVLA](https://arxiv.org/abs/2503.03480) - Safety alignment approach for
  vision-language-action models via constrained learning.
- [Safety Guardrails for LLM-Enabled Robots](https://arxiv.org/abs/2503.07885) -
  Defense work motivated by RoboPAIR-style robotic jailbreak attacks.
- [Safety-Gymnasium](https://github.com/PKU-Alignment/safety-gymnasium) -
  Reference implementation for safe reinforcement-learning evaluation.
- [SafeBench](https://safebench.github.io/) - Scenario-based safety evaluation
  for autonomous driving systems.

## Threat modeling and red teaming

- [MITRE ATLAS](https://atlas.mitre.org/) - Adversarial threat knowledge base
  for AI-enabled systems.
- [OWASP Agentic AI Threats and Mitigations](https://genai.owasp.org/resource/agentic-ai-threats-and-mitigations/) -
  Threats created by autonomous planning, tool use, memory, and delegation.
- [OWASP Secure Agent Playbook](https://github.com/OWASP/secure-agent-playbook) -
  Open engineering guidance for designing and operating secure agents.
- [NIST adversarial machine-learning taxonomy](https://csrc.nist.gov/pubs/ai/100/2/e2025/final) -
  Terminology and taxonomy for predictive and generative AI attacks and
  mitigations.
- [MIT AI Risk Repository](https://airisk.mit.edu/) - Living taxonomy of AI
  risks across academic, industry, and policy frameworks.
- [RoboPAIR](https://arxiv.org/abs/2410.13691) - Jailbreaking attack for
  LLM-controlled robots across simulated, gray-box, and black-box settings.
- [BadRobot](https://arxiv.org/abs/2407.20242) - Voice-interaction attack
  paradigm for making embodied LLM agents violate physical safety constraints.
- [POEX](https://arxiv.org/abs/2412.16633) - Policy-executable jailbreak attacks
  against LLM-based robots.
- [Semantic Denial of Service in LLM-Controlled Robots](https://arxiv.org/abs/2604.24790) -
  Attack class that degrades robot operation through semantic inputs.
- [Environmental indirect prompt injection against embodied AI](https://www.universityofcalifornia.edu/news/misleading-text-physical-world-can-hijack-ai-enabled-robots) -
  Research summary on misleading physical-world text hijacking vision-language
  robot behavior.
- [RoboJailBench](https://arxiv.org/abs/2605.19328) - Benchmark for adversarial
  attacks and defenses in embodied AI.
- [RedVLA](https://arxiv.org/abs/2604.22591) - Physical red teaming for
  vision-language-action models.

## Incident learning

- [AI Incident Database](https://incidentdatabase.ai/) - Public repository of
  reported AI harms and near harms.
- [OECD AI Incidents Monitor](https://oecd.ai/en/incidents) - International AI
  incident and hazard monitor for evidence-based policy.
- [MIT AI Incident Tracker](https://airisk.mit.edu/ai-incident-tracker) -
  AIID-based incident tracker classified by risk, cause, harm, and severity.
- [OSHA robot fatality search](https://www.osha.gov/ords/imis/AccidentSearch.search?Fatal=fatal&acc_keyword=%22Robot%22&keyword_list=on) -
  US workplace accident records involving robots.
- [CISA ICS advisories](https://www.cisa.gov/news-events/ics-advisories) -
  Vulnerabilities and mitigations affecting industrial control and operational
  technology products.
- [Mobile Industrial Robots CISA advisory](https://www.cisa.gov/news-events/ics-advisories/icsa-21-280-02) -
  Example advisory for vulnerabilities affecting mobile industrial robots and
  fleet software.
- [NTSB Uber automated test vehicle investigation](https://www.ntsb.gov/investigations/Pages/HWY18MH010.aspx) -
  Investigation page for the 2018 fatal automated-driving crash in Tempe,
  Arizona.
- [NTSB accident report HAR-19/03](https://www.ntsb.gov/investigations/accidentreports/reports/har1903.pdf) -
  Final report highlighting safety culture, risk assessment, oversight, and
  operator monitoring issues in an automated-driving test program.
- [NHTSA Standing General Order on Crash Reporting](https://www.nhtsa.gov/laws-regulations/standing-general-order-crash-reporting) -
  Example of mandatory operational incident reporting for automated vehicles.
- [Towards a common reporting framework for AI incidents](https://www.oecd.org/en/publications/towards-a-common-reporting-framework-for-ai-incidents_f326d4ac-en.html) -
  OECD reporting criteria for AI incidents and hazards.
- [AI Incidents: Key Components for a Mandatory Reporting Regime](https://cset.georgetown.edu/publication/ai-incidents-key-components-for-a-mandatory-reporting-regime/) -
  CSET proposal for incident-reporting data fields.

## Reference implementations

- [Governed Embodied Agent Lab](https://github.com/carloshvp/governed-embodied-agent-lab) -
  Small runnable environment for action policy, human approval, telemetry, and
  tamper-evident evidence in a simulated robot task.
- [Microsoft Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit) -
  Policy enforcement, identity, sandboxing, telemetry, and reliability
  components for autonomous agents.
- [AgenTrust examples](https://github.com/agentrust-io/examples) - Integration
  examples for governed and provable agent execution.
- [Industrial embodied-AI governance example](https://github.com/agentrust-io/examples/tree/main/industrial-embodied-ai) -
  Evidence-continuity and identity considerations for industrial physical AI.
- [ROS 2 SROS2](https://github.com/ros2/sros2) - Security tooling for ROS 2
  keys, certificates, and policies.
- [Safety-Gymnasium](https://github.com/PKU-Alignment/safety-gymnasium) -
  Safe reinforcement-learning environments and evaluation tools.
- [OpenTelemetry Collector](https://opentelemetry.io/docs/collector/) -
  Vendor-neutral telemetry collector for traces, metrics, and logs.

## Curation notes

This list favors resources that help answer at least one governance question:

- Can the system be bounded by explicit capability, place, time, object, and
  actor constraints?
- Can a human or independent controller stop or downgrade action authority?
- Can the system prove what policy, model, data, prompt, and controller version
  produced an action?
- Can safety and security claims be supported with repeatable evidence?
- Can incidents and near misses be reported, triaged, replayed, and learned
  from across a fleet?

The list does not try to catalog every robotics paper, benchmark, or product.
General robotics resources belong here only when they are directly useful for
governance, assurance, safety evaluation, policy enforcement, incident learning,
or secure operation.

## Contributing

Contributions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md)
before opening a pull request.

This list favors:

- Official standards, regulation, and public-sector guidance
- Primary research and maintained open-source projects
- Resources with a clear connection to physical action and control
- Canonical source links over mirrors, PDFs of paid standards, or commentary
