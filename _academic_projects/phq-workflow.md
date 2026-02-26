---
layout: page
title: "PHQ-2 / PHQ-9 Screening Workflow Reliability Analysis"
short_title: "PHQ Screening Reliability"
featured: true
order: 2
---

Analyzed the reliability of depression screening and follow-up processes in a primary care setting, focusing on structural workflow failure points rather than clinical outcomes alone.

## Context

CMS quality measures require routine depression screening (PHQ-2 followed by PHQ-9 when indicated) and documented follow-up plans. In practice, completion rates and follow-up adherence vary due to workflow complexity rather than clinical disagreement.

The objective of this project was to analyze the screening process as a system and identify where reliability degrades.

## System Mapping

The full workflow was decomposed from patient intake through:

- Intake documentation
- PHQ-2 administration
- PHQ-9 escalation logic
- Provider review
- Follow-up documentation
- Referral and care coordination

Each transition point was analyzed for task ownership, dependency, and failure sensitivity.

## Hierarchical Task Analysis (HTA)

A formal HTA was constructed to:

- Identify nested task dependencies  
- Clarify conditional branching (e.g., PHQ-2 positive → PHQ-9 required)  
- Surface hidden coordination steps  
- Reveal where omission errors were most likely  

The HTA made explicit where screening success depends on cross-role coordination rather than a single actor.

## Reliability Risks Identified

Structural risks included:

- Task ambiguity between intake staff and providers  
- Conditional escalation steps dependent on manual interpretation  
- EHR interface friction  
- Documentation lag affecting quality reporting  

The key insight was that screening compliance is less a knowledge problem and more a process integrity problem.

## Design Implications

Improving outcomes would likely require:

- Standardized task sequencing  
- Clear ownership assignment  
- Interface simplification  
- Reduced reliance on memory-dependent transitions  

The analysis reframed depression screening as a workflow reliability issue rather than a purely clinical adherence issue.
