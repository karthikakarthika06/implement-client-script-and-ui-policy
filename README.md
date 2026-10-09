# Implement Client Script & UI Policy (Incident)

## Project Overview
This project demonstrates how to implement Client Scripts and UI Policies
in ServiceNow to improve Incident form behavior and data validation.

## Objectives
- Implement Client Scripts in ServiceNow.
- Configure UI Policies for Incident forms.
- Make the Assignment Group field mandatory when Impact is High.
- Validate Incident data before saving.
- Improve data accuracy and user experience.

## Technologies Used
- ServiceNow
- JavaScript
- Client Scripts
- UI Policies
- Incident Management

## Project Implementation

### 1. UI Policy
*Name:* High Impact Control  
*Table:* Incident  
*Condition:* Impact is 1 - High

*UI Policy Action:*
- Field Name: Assignment group
- Mandatory: True
- Reverse if false: True

*Expected Result:*  
When Impact is High, the Assignment Group field becomes mandatory.
When Impact is not High, the mandatory setting is reversed.

### 2. Client Script
Client Scripts execute JavaScript on the client side of ServiceNow.
They help control form behavior and validate user input.

Types used in this project:
- onChange
- onSubmit
- onCellEdit

### 3. Testing
- Open the Incident form.
- Set Impact to High.
- Check that Assignment Group becomes mandatory.
- Change Impact to another value.
- Verify that the mandatory behavior is reversed.
- Test Client Scripts with valid and invalid inputs.

## Expected Outcome
The Incident form applies the required field rules and validation.
This helps users enter complete and accurate Incident information.

## Conclusion
This project demonstrates the use of ServiceNow Client Scripts
and UI Policies to improve Incident form functionality and data quality.
