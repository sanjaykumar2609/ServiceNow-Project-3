# Phase 7 – Project Documentation

## Project Title

Implement Client Script & UI Policy (Incident)

## Technology

ServiceNow

## Project Overview

This project implements UI Policies and Client Scripts on the ServiceNow Incident table to control form behavior, automate field updates, validate Incident data, and restrict State changes through list editing.

## Implemented Features

### 1. High Impact Control UI Policy

The **High Impact Control** UI Policy is configured on the Incident table.

**Condition:** Impact is 1 – High

The policy controls the behavior of Incident fields when a High Impact Incident is selected.

### 2. Urgency UI Policy Action

The Urgency field is configured through a UI Policy Action.

**Behavior:** Urgency becomes read-only when Impact is High.

### 3. Auto Set Urgency Client Script

**Name:** Auto set urgency for high impact

**Type:** onChange

**Field:** Impact

The Client Script automatically sets Urgency to High when Impact is changed to High.

### 4. Assigned To Validation Client Script

**Name:** Prevent save if Assigned To missing

**Type:** onSubmit

The Client Script prevents saving a High Impact Incident when the Assigned To field is empty.

### 5. State Change Restriction Client Script

**Name:** Prevent state change via list edit

**Type:** onCellEdit

**Field:** State

The Client Script prevents State changes through direct list editing.

## Testing Documentation

The implemented features were tested using Incident records.

The following scenarios were tested:

1. Impact changed to High.
2. Urgency automatically changed to High.
3. Urgency became read-only according to the UI Policy.
4. Saving was prevented when Assigned To was empty.
5. State changes through list editing were prevented.
6. Valid Incident records were successfully saved.

## Project Evidence

The project documentation includes evidence of:

- UI Policy configuration
- UI Policy Action configuration
- onChange Client Script
- onSubmit Client Script
- onCellEdit Client Script
- Incident form testing
- Validation messages
- Automatic Urgency behavior
- State list-edit restriction
- Successful testing results

## Documentation Deliverables

The following project materials are prepared:

- Project planning documentation
- Development documentation
- Testing documentation
- ServiceNow configuration screenshots
- Testing screenshots
- GitHub phase-wise project documentation
- Demonstration video

## Final Project Result

The ServiceNow Incident project demonstrates the use of UI Policies and Client Scripts to improve Incident form behavior, automate field updates, validate required information, and control State changes through list editing.

## Conclusion

The project was implemented, tested, and documented using ServiceNow. The completed configuration demonstrates the required UI Policy and Client Script functionality for the Incident table.
