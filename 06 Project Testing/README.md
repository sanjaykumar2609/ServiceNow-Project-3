# Phase 6 – Project Testing

## Project Title

Implement Client Script & UI Policy (Incident)

## Technology

ServiceNow

## Testing Overview

The implemented UI Policies and Client Scripts were tested using the ServiceNow Incident table.

The testing focused on verifying conditional field behavior, automatic Urgency updates, Assigned To validation, and State change restrictions.

## Test Case 1 – High Impact Selection

### Action

Change the Incident Impact field to High.

### Expected Result

The High Impact Control UI Policy is triggered.

### Result

Passed.

## Test Case 2 – Automatic Urgency Update

### Action

Set Impact to High.

### Expected Result

Urgency is automatically set to High.

### Result

Passed.

## Test Case 3 – Urgency UI Policy

### Action

Set Impact to High and check the Urgency field.

### Expected Result

The Urgency field becomes read-only according to the UI Policy Action.

### Result

Passed.

## Test Case 4 – Assigned To Validation

### Action

Set Impact to High and leave Assigned To empty, then attempt to save the Incident.

### Expected Result

The record is prevented from being saved.

### Result

Passed.

## Test Case 5 – State List Edit Restriction

### Action

Attempt to change the Incident State through direct list editing.

### Expected Result

The State change is prevented by the onCellEdit Client Script.

### Result

Passed.

## Test Case 6 – Valid Incident Save

### Action

Provide the required information and save a valid Incident record.

### Expected Result

The Incident record is successfully saved.

### Result

Passed.

## Testing Summary

| Test Case | Feature Tested | Expected Result | Status |
|---|---|---|---|
| 1 | High Impact Control | UI Policy is triggered | Passed |
| 2 | Automatic Urgency | Urgency becomes High | Passed |
| 3 | Urgency UI Policy Action | Urgency becomes read-only | Passed |
| 4 | Assigned To Validation | Save is prevented | Passed |
| 5 | State List Editing | State change is prevented | Passed |
| 6 | Valid Incident Save | Record saves successfully | Passed |

## Testing Outcome

All planned test scenarios were completed successfully. The ServiceNow Incident configuration demonstrated the expected behavior of the UI Policy and Client Scripts.

## Testing Evidence

Screenshots of the ServiceNow configuration and test results will be included as project documentation and evidence.
