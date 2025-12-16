# IFRAD AI Framework
Validated technical blueprints for IFRAD's AI framework. Includes system architecture v2.0, predictive algorithms (HES), integration standards, and ethical guidelines. Designed for Uganda's unconnected last mile to reduce stockouts through localized edge computing and human-in-the-loop protocols.
Status: Technical validation complete (Nov 2025) | Pilot: Planned 2026 Partners: International Foundation for Recovery and Development (IFRAD), Uganda Ministry of Health, Kyambogo University Funding: Elrha Humanitarian Innovation Fund (UK FCDO)

# Overview
This repository contains the validated technical specifications, ethical guidelines, and architectural blueprints for an offline-first AI Supply Chain Framework designed for humanitarian settings in Uganda.Current cloud-based supply chain tools fail in the 89% of facilities that face unreliable connectivity. This framework shifts predictive intelligence from the cloud to the edge, enabling sophisticated demand forecasting on mobile devices without requiring constant internet access.3

# Repository Contents
1. Core Technical Specifications: The system architecture details the offline-first approach using SQLite in WAL mode and the sync logic between facilities and national hubs. The predictive demand algorithms explains the tiered forecasting system (Rule-based for local devices, Hierarchical Exponential Smoothing for district planning). Offline workflow contains UX/UI wireframes and logic for solo-staff operations.
2. Governance & Ethics (critical for policy): The ethical guidelines contain protocols for Human-in-the-Loop AI. Includes the "Local Edits Always Win" policy that empowers frontline workers to override algorithms during outbreaks. The fraud prevention handbook is the break-glass protocols for maintaining data integrity in low-supervision environments.
3. Impact & Evidence: Baseline report conatins empirical findings from 10 health facilities in Karamoja and Nakivale Refugee Settlement (n=64 data points). Value for money assessment contain economic model projecting a 40% reduction in stockout duration and a 1:4 cost-benefit ratio.

# Key Innovations
The connectivity blind spot solution: Standard systems treat connectivity as a given. We treat it as a luxury.
Edge Computing: Algorithms run locally on Android devices.
Infrastructure-aware: We found a strong correlation (r=-0.695) between storage capacity and stockouts. Our algorithms treat physical storage as a hard constraint.
Local Edits Always Win: We solve the black box problem by ensuring algorithms never overrule clinical judgment. If a nurse overrides a forecast due to a disease outbreak, the system accepts it immediately and flags it for later analysis—it does not block the transaction.

# Tech Stack
Mobile: Android (Kotlin), Room Database (SQLite)
Forecasting: Python (hierarchicalforecast), Scikit-learn
Integration: Interoperability standards for DHIS2, eLMIS, and eAFYA

# Contact
Principal Investigator: Gideon Abako (International Foundation for Recovery & Development)
Email: abakogideon@gmail.com
