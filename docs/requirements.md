# Requirements: PTTC Discovery Tool

## Purpose

This document defines the functional and product requirements for the PTTC Discovery Tool MVP.

The goal of the MVP is to provide a 3-step guided intake workflow that helps substance misuse prevention professionals identify relevant evidence-based prevention programs based on prevention context, specific risk factor needs, and focus population.

## Product Context

The PTTC Discovery Tool supports a prevention technology initiative connected to the SAMHSA-funded Prevention Technology Transfer Center Network.

Existing program data sources were not consistently structured. Some sources included partial program information, while the most complete database functioned more like a static repository than a decision-support tool. It contained program information, but did not guide users toward the best-fit programs for their specific needs.

The product needed to help users move from:

> “I need the right prevention program.”

to:

> “Here are relevant programs based on my prevention context.”

## MVP Requirements

## 1. Guided Intake Flow

The system must provide a structured 3-step intake experience that guides users through the highest-value inputs needed to support program discovery.

The approved MVP intake flow must include:

1. Risk Factor Domain  
2. Risk Factor  
3. Focus Population  

Additional spreadsheet fields should support recommendation logic behind the scenes, without requiring users to manually filter every available program attribute.

The intake flow should help users make selections without requiring deep prior knowledge of every available evidence-based program.

## 2. Risk Factor Domain Selection

The system must allow users to select a broad risk factor domain before selecting a specific risk factor.

Supported domains should include:

• Community  
• Family  
• School  
• Individual  
• Peer  

The selected domain should determine which risk factor options are shown in the next step.

## 3. Risk Factor Selection

The system must display risk factor options based on the domain selected by the user.

The user should select the risk factor that best represents the prevention need they want to address.

This requirement protects usability and recommendation quality by keeping the intake focused and preventing users from being overwhelmed by every available data field.

## 4. Focus Population Selection

The system must allow users to select the focus population relevant to their prevention planning needs.

This input should help narrow recommendation logic and improve program fit.

## 5. Recommendation Logic

The system must use the intake inputs to return relevant program recommendations.

MVP recommendation logic should prioritize:

• Matching the selected risk factor domain  
• Matching the selected risk factor  
• Supporting the selected focus population  
• Using additional spreadsheet metadata behind the scenes where available  
• Returning programs that meet at least one meaningful match condition  

The MVP should use structured intake inputs to improve relevance without overpromising advanced AI matching before the source data can support it reliably.

## 6. Results Display

The system must present recommended programs in a clear results view.

Each result should help users understand why a program may be relevant.

At minimum, the results view should support:

• Program name  
• Relevant match indicators  
• Brief program context or summary, where available  
• Clear next step or review action  

## 7. MVP Scope Control

The MVP must focus on validating the guided intake workflow and basic recommendation structure.

The following items are out of MVP scope:

• RAG-enabled recommendation logic  
• Advanced program explanation generation  
• Admin review workflows  
• Program registry management  
• User accounts  
• Saved searches  
• Recommendation analytics  
• Feedback-based recommendation tuning  

These items may be considered in later phases after the MVP validates the core workflow.

## Non-Functional Requirements

## Usability

The workflow should be simple enough for prevention professionals who may not already know which programs to search for.

The interface should avoid overwhelming users with too many choices at once.

## Clarity

The system should use plain language wherever possible.

Prevention terminology should be structured in a way that supports user decision-making rather than adding cognitive load.

## Maintainability

The recommendation logic should be structured so future enhancements, including RAG-enabled matching, can be added later without rebuilding the entire intake flow.

## Data Practicality

Because existing source data is inconsistently structured, the MVP should rely on clear, controlled intake inputs and spreadsheet-supported metadata rather than assuming all source data can support advanced matching immediately.

## User Stories

## User Story 1: Guided Program Discovery

As a prevention professional, I want to answer guided intake questions so I can find programs that better match my prevention needs.

## User Story 2: Risk Factor Domain Selection

As a user, I want to select a broad risk factor domain so I can narrow the next set of options to the most relevant risk factors.

## User Story 3: Risk Factor Selection

As a user, I want to select a specific risk factor so the system can recommend programs aligned with the prevention need I want to address.

## User Story 4: Focus Population

As a user, I want to select a focus population so recommendations better match the group I am serving.

## User Story 5: Recommendation Results

As a user, I want to see recommended programs in a clear results view so I can understand which options may be a good fit and why.

## Product Constraints

• MVP must remain budget-conscious  
• MVP must not depend on fully normalized source data  
• MVP must avoid advanced AI recommendation claims before validation  
• Intake flow must remain simple enough for non-technical users  
• Requirements must be clear enough for developer implementation  
• Additional spreadsheet fields should support recommendation logic without becoming user-facing intake burden  

## Success Criteria

The MVP should be considered successful if it:

• Provides a clear 3-step guided intake experience  
• Helps users move from broad prevention needs to more relevant program options  
• Reduces reliance on manual program search  
• Uses spreadsheet-supported metadata to improve output relevance  
• Creates a foundation for future AI-assisted recommendation logic  
• Gives developers clear requirements and acceptance criteria  
• Protects MVP scope from unnecessary complexity
