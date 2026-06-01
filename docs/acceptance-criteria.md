# Acceptance Criteria: PTTC Discovery Tool

## Purpose

This document defines acceptance criteria for the refined PTTC Discovery Tool MVP.

The initial intake concept was built to help a non-technical stakeholder group visualize what a guided program discovery tool could do. After that early concept created alignment, the intake flow was refined into a clearer MVP structure based on prevention logic, usability needs, and technical feasibility.

## MVP Intake Flow

The refined MVP intake flow includes:

1. Risk Factor Domain  
2. Priority Risk Factors  
3. Developmental Timing  
4. Prevention Type  
5. Recommendation Results  

---

## 1. Risk Factor Domain Selection

### Business Goal

Help users start with a broad prevention context before selecting more specific priority risk factors.

### Acceptance Criteria

• User can view a clear list of supported risk factor domains.  
• User can select one risk factor domain.  
• Supported domains include Community, Family, School, Individual, and Peer.  
• User cannot continue without selecting a domain.  
• Selected domain controls which priority risk factors appear in the next step.  
• User can go back and change the selected domain before completing intake.  

---

## 2. Priority Risk Factor Selection

### Business Goal

Help users identify the specific risk factors most relevant to their prevention planning needs without overwhelming them.

### Acceptance Criteria

• User sees only the priority risk factors associated with the selected domain.  
• User can select up to three priority risk factors.  
• User cannot select more than three priority risk factors.  
• User can deselect a selected risk factor.  
• User cannot continue without selecting at least one priority risk factor.  
• If user changes the risk factor domain, previously selected priority risk factors are cleared or revalidated.  
• The interface clearly communicates the selection limit.  

---

## 3. Developmental Timing Selection

### Business Goal

Help users narrow program recommendations based on the developmental timing or age range most relevant to their prevention context.

### Acceptance Criteria

• User can view available developmental timing options.  
• User can select the developmental timing option that best matches the population or planning context.  
• User cannot continue without selecting a developmental timing option.  
• The selected timing value is included in recommendation logic.  
• User can go back and update the selection before viewing results.  

---

## 4. Prevention Type Selection

### Business Goal

Help users clarify the type of prevention approach they are seeking so recommendations better match their intended intervention strategy.

### Acceptance Criteria

• User can view available prevention type options.  
• User can select the prevention type that best matches their needs.  
• User cannot continue without selecting a prevention type.  
• The selected prevention type is included in recommendation logic.  
• User can go back and update the selection before viewing results.  

---

## 5. Recommendation Results

### Business Goal

Return relevant program options based on the user’s intake selections and help users understand why those programs may be a fit.

### Acceptance Criteria

• System returns program recommendations based on completed intake inputs.  
• Results prioritize matches across selected priority risk factors, developmental timing, and prevention type.  
• Each result displays the program name.  
• Each result includes available context or summary information where source data supports it.  
• Each result includes relevant match indicators where possible.  
• If no strong match exists, the system provides a clear empty-state message instead of showing unclear or misleading results.  
• Results should not claim advanced AI reasoning or RAG-based matching unless that capability is implemented and validated.  

---

## 6. Navigation and Usability

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

## 7. MVP Scope Boundaries

### Business Goal

Protect the MVP from overbuilding while leaving room for future AI-assisted recommendation improvements.

### Acceptance Criteria

• MVP does not require user accounts.  
• MVP does not require saved searches.  
• MVP does not require admin review workflows.  
• MVP does not require RAG-enabled matching.  
• MVP does not require advanced recommendation explanations.  
• MVP must remain functional with partially structured source data.  
• Future AI or RAG capabilities should be treated as later-phase enhancements.
