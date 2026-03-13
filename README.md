# Awesome Embodied AI Governance

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated map of standards, regulation, runtime controls, assurance methods,
> and evaluation resources for AI systems that perceive, decide, and act in the
> physical world.

Embodied AI governance begins where model behavior becomes physical action. It
includes conventional machine and robot safety, but also identity, permissions,
human intervention, observability, evidence continuity, software supply-chain
security, and the governance of learning systems that change over time.

**Last reviewed:** June 12, 2026

## Contents

- [Start here](#start-here)
- [Safety standards](#safety-standards)
- [Regulation and public frameworks](#regulation-and-public-frameworks)
- [Runtime policy and authorization](#runtime-policy-and-authorization)
- [Robot identity and communications security](#robot-identity-and-communications-security)
- [Telemetry, provenance, and evidence](#telemetry-provenance-and-evidence)
- [Human oversight and intervention](#human-oversight-and-intervention)
- [Simulation and test environments](#simulation-and-test-environments)
- [Safety and governance evaluation](#safety-and-governance-evaluation)
- [Threat modeling and red teaming](#threat-modeling-and-red-teaming)
- [Incident learning](#incident-learning)
- [Reference implementations](#reference-implementations)
- [Contributing](#contributing)

## Start here

- [ISO Robotics sector](https://www.iso.org/sectors/engineering/robotics) -
  Current ISO robotics standards and work in progress.
- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) -
  Cross-sector framework organized around Govern, Map, Measure, and Manage.
- [EU Artificial Intelligence Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng) -
  Official regulation text, including high-risk system obligations and
  requirements relevant to AI safety components.
- [ROS 2 Security](https://docs.ros.org/en/rolling/Concepts/Intermediate/About-Security.html) -
  Authentication, encryption, integrity, and access control for ROS graphs.
- [EmbodiedGovBench](https://arxiv.org/abs/2604.11174) -
  Governance-oriented evaluation across controllability, policy boundaries,
  recovery, auditability, and upgrade safety.

## Safety standards

Standards often require purchase. Links below point to official abstracts and
catalog entries.

- [ISO 10218-1:2025](https://www.iso.org/standard/73933.html) - Safety
  requirements for industrial robots.
- [ISO 10218-2:2025](https://www.iso.org/standard/73934.html) - Safety
  requirements for industrial robot applications and robot cells.
- [ISO/TS 15066:2016](https://www.iso.org/standard/62996.html) - Collaborative
  robot system and work-environment guidance.
- [ISO 13482:2014](https://www.iso.org/standard/53820.html) - Safety
  requirements for personal care robots.
- [ISO 12100:2010](https://www.iso.org/standard/51528.html) - Machinery risk
  assessment and risk-reduction methodology.
- [ISO 3691-4:2023](https://www.iso.org/standard/83545.html) - Driverless
  industrial trucks, AGVs, and autonomous mobile robot systems.
- [IEC functional safety](https://www.iec.ch/functionalsafety) - Entry point
  for IEC 61508 and sector-specific functional-safety standards.
- [IEC 62443 overview](https://www.iec.ch/blog/understanding-iec-62443) -
  Cybersecurity for industrial automation and control systems.
- [ISO/TR 23482-1:2020](https://www.iso.org/standard/71539.html) - Test methods
  supporting ISO 13482.
- [ISO/TR 23482-2:2019](https://www.iso.org/standard/71627.html) - Application
  guidance supporting ISO 13482.

## Regulation and public frameworks

- [EU Artificial Intelligence Act](https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng) -
  Harmonized rules for AI systems in the European Union.
- [EU Machinery Regulation](https://eur-lex.europa.eu/eli/reg/2023/1230/oj/eng) -
  Safety requirements for machinery, including software and autonomous
  behavior.
- [EU Cyber Resilience Act](https://eur-lex.europa.eu/eli/reg/2024/2847/oj/eng) -
  Cybersecurity obligations for products with digital elements.
- [EU Product Liability Directive](https://eur-lex.europa.eu/eli/dir/2024/2853/oj/eng) -
  Product-liability rules covering software and AI-enabled products.
- [European Commission AI Act portal](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai) -
  Implementation timeline, guidance, and institutional resources.
- [NIST AI RMF 1.0](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf) -
  Voluntary risk-management framework for AI systems.
- [NIST AI RMF Playbook](https://airc.nist.gov/airmf-resources/playbook/) -
  Suggested actions aligned to the AI RMF outcomes.
- [NIST Generative AI Profile](https://doi.org/10.6028/NIST.AI.600-1) -
  Cross-sector companion profile for generative AI risks.
- [NIST Secure Software Development Framework](https://csrc.nist.gov/pubs/sp/800/218/final) -
  Secure software practices relevant to robot and agent control stacks.

## Runtime policy and authorization

- [Open Policy Agent](https://www.openpolicyagent.org/docs/latest/) - General
  policy-as-code engine using Rego.
- [Cedar](https://docs.cedarpolicy.com/) - Authorization policy language and
  evaluator designed for fine-grained permissions.
- [OpenFGA](https://openfga.dev/docs) - Relationship-based authorization
  modeled on Zanzibar-style access control.
- [Casbin](https://casbin.org/docs/overview) - Authorization library supporting
  ACL, RBAC, and ABAC models.
- [SPIFFE and SPIRE](https://spiffe.io/docs/latest/) - Workload identity and
  attestation for distributed systems.
- [in-toto](https://in-toto.io/) - Supply-chain layout and verification for
  software artifacts.
- [Sigstore](https://docs.sigstore.dev/) - Signing and verification for
  software artifacts and identities.
- [SLSA](https://slsa.dev/) - Supply-chain security levels and provenance.
- [The Update Framework](https://theupdateframework.io/) - Resilient software
  update design, important for remote robot fleets.

## Robot identity and communications security

- [ROS 2 security concepts](https://docs.ros.org/en/rolling/Concepts/Intermediate/About-Security.html) -
  DDS-Security-backed identity, encryption, integrity, and access control.
- [ROS 2 security setup](https://docs.ros.org/en/rolling/Tutorials/Advanced/Security/Introducing-ros2-security.html) -
  Practical SROS2 keystore and enclave tutorial.
- [ROS 2 access controls](https://docs.ros.org/en/rolling/Tutorials/Advanced/Security/Access-Controls.html) -
  Permission policies for ROS nodes, topics, and services.
- [SROS2](https://github.com/ros2/sros2) - ROS 2 tooling for keys,
  certificates, and security policies.
- [DDS Security specification](https://www.omg.org/spec/DDS-SECURITY/) -
  Authentication, access control, cryptography, logging, and data tagging for
  DDS systems.
- [ROS 2 security deployment guidelines](https://docs.ros.org/en/rolling/Tutorials/Advanced/Security/Deployment-Guidelines.html) -
  Guidance for distributing and protecting security material.

## Telemetry, provenance, and evidence

- [OpenTelemetry](https://opentelemetry.io/docs/) - Vendor-neutral traces,
  metrics, and logs.
- [OpenTelemetry Python](https://opentelemetry.io/docs/languages/python/) -
  Python APIs and SDK guidance for instrumentation.
- [OpenTelemetry semantic conventions](https://opentelemetry.io/docs/specs/semconv/) -
  Standardized names and attributes for telemetry.
- [W3C PROV overview](https://www.w3.org/TR/prov-overview/) - Data model for
  representing entities, activities, agents, and provenance.
- [OpenLineage](https://openlineage.io/docs/) - Open standard for lineage
  events and integrations.
- [CloudEvents](https://cloudevents.io/) - Common envelope for describing
  events across services and platforms.
- [Merkle transparency log concepts](https://transparency.dev/) - Patterns for
  append-only, publicly verifiable records.

Useful evidence questions:

- Which identity requested, planned, authorized, and executed the action?
- Which policy and model versions were active?
- What observation and uncertainty estimate informed the decision?
- Was human approval bound to the exact action and context?
- Can the record survive a controller restart and be checked for tampering?

## Human oversight and intervention

- [Action-bound approval protocol](https://github.com/microsoft/agent-governance-toolkit/pull/2953) -
  Proposal for binding approval to a specific action, arguments, principal,
  policy, and execution context.
- [NIST AI RMF Playbook](https://airc.nist.gov/airmf-resources/playbook/) -
  Human-AI configuration, roles, responsibilities, and intervention practices.
- [ISO 10218-2:2025](https://www.iso.org/standard/73934.html) - Integration and
  operational safety requirements for industrial robot applications.
- [ROS 2 lifecycle nodes](https://design.ros2.org/articles/node_lifecycle.html) -
  Managed states useful for controlled activation, deactivation, recovery, and
  shutdown.

## Simulation and test environments

- [MuJoCo](https://mujoco.readthedocs.io/) - Fast physics simulation for
  control, state estimation, and contact-rich tasks.
- [Gazebo Sim](https://gazebosim.org/libs/sim/) - Open robotics simulator with
  physics, rendering, sensors, plugins, and message interfaces.
- [NVIDIA Isaac Sim](https://docs.isaacsim.omniverse.nvidia.com/latest/) -
  GPU-accelerated robotics simulation and synthetic data generation.
- [Isaac Lab](https://isaac-sim.github.io/IsaacLab/) - Robot-learning framework
  built on Isaac Sim.
- [Webots](https://cyberbotics.com/doc/guide/index) - General-purpose open
  source robot simulator.
- [robosuite](https://robosuite.ai/docs/overview.html) - MuJoCo-based
  manipulation environments and standardized robot tasks.
- [Safety-Gymnasium](https://safety-gymnasium.readthedocs.io/) - Safe
  reinforcement-learning environments and evaluation tooling.
- [BEHAVIOR-1K](https://behavior.stanford.edu/) - Benchmark and simulation
  environment for 1,000 household activities.

Governance tests should cover more than task success: unauthorized capability
use, restricted zones, stale approvals, identity loss, policy unavailability,
sensor uncertainty, emergency stop, restart recovery, upgrade rollback, and
evidence completeness.

## Safety and governance evaluation

- [EmbodiedGovBench](https://arxiv.org/abs/2604.11174) - Benchmark proposal for
  policy boundaries, recovery, override responsiveness, audit completeness,
  and upgrade safety.
- [AgentSafe](https://arxiv.org/abs/2506.14697) - Safety benchmark for embodied
  vision-language-model agents under hazardous instructions.
- [EAsafetyBench](https://www.ijcai.org/proceedings/2025/0867.pdf) - Embodied
  agent input-safety benchmark and moderation framework.
- [DESPITE](https://arxiv.org/abs/2604.18463) - Deterministic evaluation of
  physical and normative dangers in embodied planning.
- [Safety in Embodied AI](https://arxiv.org/abs/2505.15417) - Survey of risks,
  attacks, defenses, and evaluation methods.
- [Safety of Embodied Navigation](https://arxiv.org/abs/2508.05855) - Survey
  focused on attacks, defenses, robustness, and verification in navigation.
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
- [NIST adversarial machine learning taxonomy](https://csrc.nist.gov/pubs/ai/100/2/e2025/final) -
  Terminology and attack/mitigation taxonomy for predictive and generative AI.
- [Physical-agent risk mapping](https://github.com/microsoft/agent-governance-toolkit/pull/2916) -
  Mapping of agentic risks to systems with actuators and physical effects.

## Incident learning

- [AI Incident Database](https://incidentdatabase.ai/) - Public repository of
  reported AI harms and near harms.
- [OECD AI Incidents Monitor](https://oecd.ai/en/incidents) - International
  incident and hazard reporting resource.
- [CISA ICS advisories](https://www.cisa.gov/news-events/cybersecurity-advisories) -
  Vulnerabilities and incidents affecting industrial control products.
- [NTSB investigation database](https://www.ntsb.gov/Pages/AviationQueryV2.aspx) -
  Investigation model and records useful for studying evidence quality in
  safety-critical systems.

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

## Contributing

Contributions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md)
before opening a pull request.

This list favors:

- Official standards, regulation, and public-sector guidance
- Primary research and maintained open-source projects
- Resources with a clear connection to physical action and control
- Practical material that helps teams design, test, operate, or audit systems

It excludes generic AI ethics lists, unsupported marketing claims, abandoned
projects, and resources with no clear embodied-system relevance.

## Disclaimer

This repository is an engineering research map, not legal or safety
certification advice. Applicable requirements depend on the robot, intended
use, environment, jurisdiction, integration, and risk assessment.
