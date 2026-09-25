# Phase 2 – Requirement Analysis

## Project Title

Implement Client Script & UI Policy (Incident)

## Technology

ServiceNow

## Problem Statement

Incident records require consistent and accurate data entry for effective triage, routing, and resolution.

Manual checking can result in incomplete, inconsistent, or incorrect information.

## Project Requirements

The project requires the implementation of UI Policies and Client Scripts on the ServiceNow Incident table.

### Functional Requirements

1. Create a UI Policy named **High Impact Control**.
2. Configure the UI Policy condition:
   - Table: Incident
   - Impact is 1 – High
3. Configure a UI Policy Action for the **Urgency** field.
4. Make Urgency read-only when Impact is High.
5. Create an **onChange Client Script** named:
   - Auto set urgency for high impact
6. Automatically set Urgency to High when Impact is High.
7. Create an **onSubmit Client Script** named:
   - Prevent save if Assigned To missing
8. Prevent saving when Impact is High and Assigned To is empty.
9. Create an **onCellEdit Client Script** named:
   - Prevent state change via list edit
10. Prevent State changes through direct list editing.
11. Test all configured behaviors.

## Required Incident Fields

- Impact
- Urgency
- Assigned To
- State

## Expected Outcome

The Incident form should provide conditional field behavior, automatic Urgency updates, validation for Assigned To, and restriction of State changes through list editing.
