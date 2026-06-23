Lab says:
Select MOD Administrator account

Actual experience:
User must manually create Dataverse connection before trigger can be configured.

# Lab 4 Validation

## Validation Status

PARTIAL PASS

## Tasks Completed

### Exercise 1 - Create Automated Cloud Flow

* Successfully accessed Power Automate Maker Portal.
* Switched environment to Dev One.
* Created flow named **Notify on High Priority Request**.
* Selected **When a row is added, modified or deleted (Microsoft Dataverse)** trigger.

### Exercise 2 - Configure Flow

* Trigger initially displayed **Invalid Parameters**.
* Created a new Dataverse connection reference.
* Successfully connected Microsoft Dataverse.
* Configured trigger:

  * Change Type = Added
  * Scope = Organization
* Identified that the correct table name is **Facility Request** instead of **Facility Requests**.
* Added **Get a row by ID** action.
* Configured Dataverse table reference successfully.
* Retrieved Priority choice values from the Facility Request table:

  * Low = 277570000
  * Medium = 277570001
  * High = 277570002
  * Urgent = 277570003
* Added condition to check:

  * Priority = High
  * OR
  * Priority = Urgent

### Exercise 3 - Email Notification Configuration

* Reached Send an Email (V2) configuration step.
* Unable to create Office 365 Outlook connection.
* Email action could not be configured or tested.

## Validation Checks

* Verified flow creation process.
* Verified Dataverse trigger configuration.
* Verified Dataverse connection creation.
* Verified Facility Request table access.
* Verified Get a Row by ID action.
* Verified condition configuration using Priority values.
* Flow design completed up to email notification step.

## Observations

* Power Automate UI differs slightly from lab screenshots.
* Trigger initially reports Invalid Parameters until a Dataverse connection reference is created.
* Lab instructions reference **Facility Requests** while the environment contains **Facility Request**.
* Copilot suggestions were not reliable for flow configuration and manual configuration was required.
* Current experience requires additional connection setup not fully reflected in screenshots.

## Issues Found

### Issue 1 - Table Name Mismatch

* Lab instructions reference **Facility Requests**.
* Environment contains **Facility Request**.
* Using the plural table name causes Dataverse trigger errors.

### Issue 2 - Office 365 Outlook Connection Failure

* Unable to create Outlook connection for Send an Email (V2).

* Error encountered:

  OwaUserHasNoMailboxAndNoLicenseAssignedException

* Outlook Web Access also reports mailbox/license issues.

### Impact

* Flow creation can be completed.
* Dataverse trigger and condition logic can be configured.
* Email notification functionality cannot be validated using the provided training account.

### Workaround

* Await confirmation from lab administrator regarding mailbox licensing.
* Alternative test account with Exchange Online mailbox may be required.

## Result

Lab completed up to the email notification stage.

Flow trigger, Dataverse integration, and condition logic were successfully configured.

Final email notification testing is currently blocked by Exchange Online mailbox licensing limitations in the provided training environment.
