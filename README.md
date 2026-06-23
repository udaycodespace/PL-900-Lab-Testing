# PL-900 Lab Testing

Testing and validating PL-900 Microsoft Power Platform Fundamentals labs against the current Power Platform experience.

**By:** [@udaycodespace](https://github.com/udaycodespace)

## Objective

This repository documents my hands-on validation of PL-900 labs, including:

* UI changes from current Power Platform releases
* Student blockers encountered during execution
* Missing prerequisites
* Outdated screenshots and navigation paths
* Documentation improvements required for successful completion

The goal is to verify whether each lab can still be completed successfully using the current Microsoft Power Platform experience.

---

## Testing Workflow

1. Execute each lab exactly as documented.
2. Record any blockers encountered.
3. Compare current UI against lab screenshots.
4. Validate expected outcomes.
5. Document changes and observations.
6. Update instructions only when required.

---

## Lab Status

| Lab                                   | Status     | Notes                                                                                                                                 |
| ------------------------------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Lab 00 - Validate Lab Environment     | ✅ Complete | Validated                                                                                                                             |
| Lab 01 - Create a Data Model          | ✅ Complete | Validated                                                                                                                             |
| Lab 02 - Create a Canvas App          | ✅ Complete | Validated ([Live App](https://apps.powerapps.com/play/e/20c6b95d-89fe-eeef-aaa5-335ec2d2c345/a/60babd50-6ee4-4eeb-bcfc-72fbd93abd1f)) |
| Lab 03 - Create a Model-Driven App    | ⏳ Pending  | Not Started                                                                                                                           |
| Lab 04 - Create a Power Automate Flow | ⏳ Pending  | Not Started                                                                                                                           |

---

## Key Observations

### Lab 00

* Environment creation is now required before starting labs.
* Initial sign-in may require MFA registration.
* Additional setup steps were not documented in the original lab.

### Lab 01

* Table creation experience has changed slightly.
* Copilot-generated experiences differ from screenshots.
* Core functionality remains unchanged.

### Lab 02

* Upload file workflow has changed.
* Additional Copilot preview experience introduced.
* Generated app layout differs from screenshots.
* Dataverse integration validated successfully.
* Navigation and form submission tested successfully.
* Published app updates may take time to propagate.

---

## Commit Format

* `Lab XX - Passed`
* `Lab XX - Fixed: Step Y (description)`
* `Lab XX - Needs Investigation`

or

* `docs: validate Lab X and update documentation`
* `docs(validation): add findings and instruction updates`

---

Based on validation of MicrosoftLearning PL-900 lab content and current Power Platform experiences.
