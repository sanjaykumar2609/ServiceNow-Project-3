# Phase 4 – Project Planning

## Project Title

Implement Client Script & UI Policy (Incident)

## Technology

ServiceNow

## Project Goal

To implement and test UI Policies and Client Scripts that control Incident form behavior and improve data validation.

## Project Activities

| Activity | Description |
|---|---|
| 1. Project Setup | Prepare the ServiceNow Incident application/environment |
| 2. UI Policy Creation | Create the High Impact Control UI Policy |
| 3. UI Policy Action | Configure the Urgency field behavior |
| 4. onChange Script | Automatically set Urgency when Impact is High |
| 5. onSubmit Script | Validate Assigned To before saving |
| 6. onCellEdit Script | Prevent State changes through list editing |
| 7. Testing | Test each implemented feature |
| 8. Documentation | Record configuration, screenshots, and results |
| 9. Demonstration | Prepare the final project demonstration video |

## Implementation Plan

### Step 1
Create the **High Impact Control** UI Policy for the Incident table.

### Step 2
Configure the **Urgency UI Policy Action**.

### Step 3
Create the **Auto set urgency for high impact** onChange Client Script.

### Step 4
Create the **Prevent save if Assigned To missing** onSubmit Client Script.

### Step 5
Create the **Prevent state change via list edit** onCellEdit Client Script.

### Step 6
Test all configurations using Incident records.

### Step 7
Capture screenshots of the configuration and testing results.

### Step 8
Prepare the final project documentation and demonstration video.

## Testing Plan

The following scenarios will be tested:

1. Impact is changed to High.
2. Urgency is automatically set to High.
3. Urgency behavior is controlled by the UI Policy.
4. Saving is prevented when Assigned To is missing.
5. State changes through list editing are prevented.
6. Valid Incident records can be successfully saved.

## Expected Deliverables

- ServiceNow project implementation
- Configuration screenshots
- Testing screenshots
- Project documentation
- GitHub repository with phase-wise project files
- Project demonstration video

## Project Timeline

| Phase | Work |
|---|---|
| Planning | Define requirements and implementation steps |
| Development | Configure UI Policy and Client Scripts |
| Testing | Test all required scenarios |
| Documentation | Prepare project records and screenshots |
| Demonstration | Record and submit project demo |

## Final Outcome

A working ServiceNow Incident configuration that demonstrates UI Policy and Client Script functionality through implementation, testing, documentation, and demonstration.
