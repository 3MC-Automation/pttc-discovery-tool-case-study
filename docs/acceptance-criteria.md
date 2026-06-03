# Acceptance Criteria: Evidence-Based Program Discovery Workflow

## Purpose

This document defines acceptance criteria for the approved evidence-based program discovery workflow MVP.

The initial intake concept was built to help a non-technical stakeholder group visualize what a guided program discovery tool could do. After stakeholder review and refinement, the approved MVP evolved into a 3-step intake workflow focused on Risk Factor Domain, Risk Factor, and Focus Population.

## MVP Intake Flow

The approved MVP intake flow includes:

1. Risk Factor Domain  
2. Risk Factor  
3. Focus Population  
4. Recommendation Results  

Additional spreadsheet fields support recommendation logic behind the scenes and are not required user inputs.

---

## 1. Risk Factor Domain Selection

### Business Goal

Help users start with a broad prevention context before selecting a specific prevention need.

### Acceptance Criteria

• User can view a clear list of supported risk factor domains.  
• User can select one risk factor domain.  
• Supported domains include Community, Family, School, Individual, and Peer.  
• User cannot continue without selecting a domain.  
• Selected domain controls which risk factors appear in the next step.  
• User can go back and change the selected domain before completing intake.  

---

## 2. Risk Factor Selection

### Business Goal

Help users identify the specific prevention need they want to address.

### Acceptance Criteria

• User sees only risk factor options associated with the selected domain.  
• User can select a risk factor.  
• User cannot continue without selecting a risk factor.  
• If user changes the risk factor domain, previously selected risk factors are cleared or revalidated.  
• The interface clearly communicates available options.  

---

## 3. Focus Population Selection

### Business Goal

Help users identify the population they are trying to support so recommendations better match implementation needs.

### Acceptance Criteria

• User can view available focus population options.  
• User can select a focus population.  
• User cannot continue without selecting a focus population.  
• The selected population value is included in recommendation logic.  
• User can go back and update the selection before viewing results.  

---

## 4. Recommendation Results

### Business Goal

Return relevant program options based on the user’s intake selections and help users understand why those programs may be a fit.

### Acceptance Criteria

• System returns program recommendations based on completed intake inputs.  
• Results prioritize matches across selected domain, risk factor, and focus population.  
• Additional spreadsheet metadata may be used to improve recommendation relevance.  
• Each result displays the program name.  
• Each result includes available context or summary information where source data supports it.  
• Each result includes relevant match indicators where possible.  
• If no strong match exists, the system provides a clear empty-state message instead of showing unclear or misleading results.  
• Results should not claim advanced AI reasoning or RAG-based matching unless that capability is implemented and validated.  

---

## 5. Navigation and Usability

### Business Goal

Make the intake flow simple enough for prevention professionals who may not know which programs to search for in advance.

### Acceptance Criteria

• User can move forward through the intake flow one step at a time.  
• User can move backward to revise previous answers.  
• The interface clearly shows progress through the intake flow.  
• Each step uses plain language and avoids unnecessary technical terminology.  
• Required fields are clear before the user attempts to continue.  
• The workflow avoids showing too many options at once.  

---

## 6. MVP Scope Boundaries

### Business Goal

Protect the MVP from overbuilding while leaving room for future AI-assisted recommendation improvements.

### Acceptance Criteria

• MVP does not require user accounts.  
• MVP does not require saved searches.  
• MVP does not require admin review workflows.  
• MVP does not require RAG-enabled matching.  
• MVP does not require advanced recommendation explanations.  
• MVP must remain functional with partially structured source data.  
• Additional spreadsheet fields may support recommendation logic without becoming user-facing inputs.  
• Future AI or RAG capabilities should be treated as later-phase enhancements.
