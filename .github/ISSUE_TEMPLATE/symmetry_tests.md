---
name: "Symmetry Integration User Test Report"
about: "Template for reporting integration user test results"
title: "[Integration Test] - <Short Description of the Test>"
labels: "integration-test"
assignees: ""
---

## Integration User Test Report

### Test Details
- **Test Name:** 
- **Test Date:** 
- **Tester Name:** 
- **Source System:** (e.g., Application A)
- **Destination System:** (e.g., Application B)

### Initial State of the Source System
<!-- Describe the initial state in detail -->
- **State Description:** 
  - Example: 3 People without any access
- **Data Details:** 
  - Person 1: No cards
  - Person 2: One disabled cards, one active card
  - Person 3: Two active cards

### Expected Outcome in the Destination System
<!-- Describe the expected result after integration -->
- **Expected Outcome Description:** 
  - Example: No export is performed to the destination system

### Steps to Reproduce
1. Remove the bookmark file
2. Start the Symmetry integration service
3. Stop the service after the bookmark file appears in the .data folder
4. 

### Actual Outcome in the Destination System
<!-- Describe what actually happened -->
- **Actual Outcome Description:** 
  - Example: No export was performed / Export was performed incorrectly

### Observations
<!-- Any additional observations or notes -->

### Screenshots / Videos
<!-- Attach any relevant screenshots or video recordings -->

### Severity
<!-- Choose the appropriate severity level -->
- [ ] Critical
- [ ] High
- [ ] Medium
- [ ] Low

### Additional Information
<!-- Any other information that might be useful -->

### Suggestions / Recommendations
<!-- Any recommendations or suggestions based on the test results -->

### Checklist
- [ ] Initial state of the source system is clear and complete
- [ ] Expected outcome is documented
- [ ] Steps to reproduce are clear and complete
- [ ] Actual outcome is documented
- [ ] Severity is selected
- [ ] Relevant media (screenshots/videos) are attached
- [ ] Additional observations are noted