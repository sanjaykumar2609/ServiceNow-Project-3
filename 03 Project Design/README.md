# Phase 3 – Project Design

## Project Title

Implement Client Script & UI Policy (Incident)

## Technology

ServiceNow

## Design Overview

The project is designed to control Incident form behavior using UI Policies and Client Scripts.

## UI Policy Design

### UI Policy Name
High Impact Control

### Table
Incident

### Condition
Impact is 1 – High

### Reverse if false
True

## UI Policy Action

### Field
Urgency

### Behavior
Read-only when Impact is High.

## Client Script Design

### 1. onChange Client Script

Name: Auto set urgency for high impact

Field: Impact

Purpose: Automatically set Urgency to High when Impact is High.

### 2. onSubmit Client Script

Name: Prevent save if Assigned To missing

Purpose: Prevent saving a High impact Incident when Assigned To is empty.

### 3. onCellEdit Client Script

Name: Prevent state change via list edit

Field: State

Purpose: Prevent State changes through direct list editing.

## Process Flow

Incident Form
→ Check Impact
→ Apply UI Policy
→ Set Urgency
→ Validate Assigned To
→ Submit Incident

## Expected Design Outcome

The Incident form should provide conditional field behavior, automatic Urgency updates, validation for Assigned To, and restriction of State changes through list editing.
