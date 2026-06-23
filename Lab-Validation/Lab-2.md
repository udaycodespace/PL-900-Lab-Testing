# Lab 2 - Create a Canvas App

## Exercise 1 - Create an App from a Template

### Status

Validated Successfully

The exercise was completed successfully using the current Power Apps experience. The generated application loaded correctly, preview mode worked, and new record creation functionality was available without errors.

---

## Finding 1 - Create Page UI Changed

### Old Instructions

Navigation:

Create
→ Start from data
→ Upload file

### Current Experience

Navigation:

Create
→ Scroll to Start from data section
→ Upload file

The Upload file option still exists but is no longer immediately visible on the Create page and requires scrolling.

### Impact

Low

Students may initially think the Upload file option has been removed.

### Documentation Update

Add a note indicating that the Upload file tile is located further down the Create page and may require scrolling.

---

## Finding 2 - Additional Copilot Table Preview Screen

### Old Instructions

Upload file
→ Create app

### Current Experience

Upload file
→ Copilot-generated table preview
→ Create app

After uploading Room Reservations.xlsx, Power Apps generates a Dataverse table preview before allowing app creation.

### Impact

Low

Students may believe an additional configuration step is required.

### Documentation Update

Add screenshot and instructions for the table preview screen.

---

## Finding 3 - Power Apps Studio Startup Experience Changed

### Old Instructions

Create app
→ App opens

### Current Experience

Create app
→ Power Apps Studio opens
→ Copilot panel automatically displayed

The Copilot panel is opened automatically when the app is generated.

### Impact

Low

Students unfamiliar with Copilot may think further action is required before continuing.

### Documentation Update

Add note explaining that the Copilot panel can be ignored for this exercise.

---

## Finding 4 - Generated Application Layout Differs

### Old Instructions

Screenshots show an older generated layout.

### Current Experience

Generated app contains:

* Search box
* Gallery
* Detail form
* New button
* Edit button
* Delete button

The layout differs visually from older screenshots but functionality remains equivalent.

### Impact

Low

Students comparing against screenshots may think their app was generated incorrectly.

### Documentation Update

Add note that generated layouts may vary depending on Power Apps version.

---

## Finding 5 - New Record Form Works Correctly

### Validation Performed

Preview mode launched successfully.

Selecting:

* New

opened a blank form without errors.

Observed controls:

* Date Picker
* Dropdown controls
* Text fields
* Save button
* Cancel button

### Result

New record creation flow functions correctly.

### Impact

None

No blocker identified.

---

## Exercise 1 Summary

### Result

Validated Successfully

### Student Blockers

None

### UI Differences

1. Upload file location changed.
2. Copilot table preview screen added.
3. Copilot side panel automatically opens.
4. Generated application layout differs from screenshots.

### Missing Documentation

1. Updated Create page navigation.
2. Table preview step.
3. Copilot panel explanation.
4. Screenshot refresh.

### Overall Impact

Low

Exercise remains fully functional with only minor UI changes.

# Exercise 2 - Build and Edit a Canvas App

## Status

Validated Successfully

The Facility Request canvas app was created successfully from the Dataverse table. Navigation between screens functioned correctly, the New Room screen was added successfully, and records were saved into the Room Dataverse table.

---

## Finding 6 - Generated Facility Requests App Layout Differs

### Old Instructions

Expected screenshots show an older generated canvas app layout.

### Current Experience

The generated application contains:

* Facility Requests gallery on the left
* Detail form on the right
* New button
* Edit button
* Delete button
* Search box

The visual layout differs slightly from screenshots provided in the lab guide.

### Impact

Low

Functionality remains identical.

### Documentation Update

Refresh screenshots to match the current Power Apps generated app experience.

---

## Finding 7 - Dataverse Table Naming Difference

### Old Instructions

Search for:

Facility Requests

### Current Experience

Environment contains:

* Facility Request
* Room
* Room Reservation

The generated app may display singular table names depending on environment configuration.

### Impact

Low

Students may not immediately recognize the correct table.

### Documentation Update

Clarify that singular or plural table names may appear depending on environment setup.

---

## Finding 8 - New Room Screen Creation Works Correctly

### Validation Performed

Successfully created:

* Header and Footer screen
* Renamed screen to New Room Screen
* Added Edit Form
* Connected form to Room table
* Set form Default Mode to New

### Result

Functionality works as documented.

### Impact

None

No blocker identified.

---

## Finding 9 - Additional Room Fields May Appear

### Old Instructions

Remove:

* Import Sequence Number
* Time Zone Rule Version Number
* Record Created On

### Current Experience

The generated form only contained business-related fields:

* Room Name
* Building
* Campus
* Floor
* Conference Room

The system columns referenced in the lab were not present.

### Impact

Low

Students may spend time searching for fields that no longer appear.

### Documentation Update

Add note that these fields only need to be removed if they are automatically added to the form.

---

## Finding 10 - Submit Button Successfully Saves Records

### Validation Performed

Created multiple Room records using:

SubmitForm(Form2);
Navigate('Facility Requests screen')

Observed records successfully saved into the Room Dataverse table.

Example records created:

* UDAY
* UDAY
* UDAY
* UDAY

Verified directly in Dataverse Table > Room.

### Result

Submit functionality works correctly.

### Impact

None

No blocker identified.

---

## Finding 11 - Navigation Works Correctly

### Validation Performed

Selecting:

New Room

navigates to:

New Room Screen

Selecting:

Submit

returns user to:

Facility Requests screen

using:

NewForm(Form2); Navigate('New Room Screen')

and

SubmitForm(Form2); Navigate('Facility Requests screen')

### Result

Navigation functions as expected.

### Impact

None

No blocker identified.

---

## Finding 12 - Published App May Display Cached Version

### Current Experience

After saving changes, the shared application initially continued displaying the previous version.

Power Apps displayed:

"A new version of this app is coming. We'll let you know when it's available."

The published version required additional time to refresh.

### Impact

Medium

Students may believe their changes were not saved or published.

### Documentation Update

Add note indicating that published apps may take several minutes to reflect newly published changes.

---

## Exercise 2 Summary

### Result

Validated Successfully

### Student Blockers

None

### UI Differences

1. Generated app layout differs from screenshots.
2. Table names may appear in singular form.
3. System fields may no longer be added automatically.
4. Published app may show cached version temporarily.

### Missing Documentation

1. Updated generated app screenshots.
2. Clarification on Room table selection.
3. Clarification regarding optional system fields.
4. Note regarding published app propagation delays.

### Overall Impact

Low

Exercise remains fully functional. All required objectives, including Dataverse integration, screen creation, navigation, form submission, and data persistence, were completed successfully.
