# Phase 5 – Project Development

## Project Title

Implement Client Script & UI Policy (Incident)

## Technology

ServiceNow

## Development Overview

The project was developed using ServiceNow to control Incident form behavior through UI Policies and Client Scripts.

The implementation focuses on conditional field behavior, automatic Urgency updates, data validation, and restricting State changes through direct list editing.

## ServiceNow Incident Table

The configurations were implemented on the **Incident** table.

### Fields Used

- Impact
- Urgency
- Assigned To
- State

## 1. UI Policy – High Impact Control

### Name

High Impact Control

### Table

Incident

### Condition

Impact is 1 – High

### Purpose

The UI Policy controls the behavior of Incident fields when the Impact field is set to High.

## 2. UI Policy Action – Urgency

### Field

Urgency

### Behavior

The Urgency field is made read-only when Impact is High.

### Purpose

This helps control the Urgency field when a High Impact Incident is selected.

## 3. onChange Client Script

### Name

Auto set urgency for high impact

### Type

onChange

### Field

Impact

### Purpose

Automatically sets the Urgency field to High when the Impact field is changed to High.

## 4. onSubmit Client Script

### Name

Prevent save if Assigned To missing

### Type

onSubmit

### Purpose

Prevents saving the Incident when:

- Impact is High
- Assigned To is empty

This provides validation before the Incident record is submitted.

## 5. onCellEdit Client Script

### Name

Prevent state change via list edit

### Type

onCellEdit

### Field

State

### Purpose

Prevents State changes when an Incident is edited directly through list editing.

## Development Process

The development was completed using the following sequence:

1. Prepared the ServiceNow Incident environment.
2. Created the High Impact Control UI Policy.
3. Configured the Urgency UI Policy Action.
4. Created the onChange Client Script for automatic Urgency.
5. Created the onSubmit Client Script for Assigned To validation.
6. Created the onCellEdit Client Script for State change restriction.
7. Tested the implemented configurations using Incident records.
8. Captured configuration and testing screenshots.
9. Prepared the project documentation and demonstration.

## Implementation Summary

| Component | Purpose |
|---|---|
| High Impact Control UI Policy | Controls Incident behavior when Impact is High |
| Urgency UI Policy Action | Makes Urgency read-only when Impact is High |
| Auto set urgency for high impact | Automatically sets Urgency to High |
| Prevent save if Assigned To missing | Prevents saving when Assigned To is missing |
| Prevent state change via list edit | Prevents State changes through list editing |

## Development Outcome

The ServiceNow Incident configuration was implemented with UI Policies and Client Scripts to provide conditional field behavior, automatic Urgency updates, validation, and restriction of State changes through list editing.
