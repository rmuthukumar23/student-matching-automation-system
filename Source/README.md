# Source

This folder contains a sanitized copy of the main MIT App Inventor block files recovered from the original `Student4Student.aia` project.

The project was built before March 2025 and uploaded to GitHub later. GitHub was not used during the original development.

## Files

- `Screen1.bky` - login, validation and authentication response handling
- `StudentRequests.bky` - loads student requests, parses JSON, searches by ID and selects a student
- `TutorRequests.bky` - loads tutor requests, parses JSON and searches by ID
- `MatchScreen.bky` - receives the selected student and loads their details

The app used Google Apps Script endpoints for authentication and spreadsheet data. Those live URLs were hard-coded in the original App Inventor project, so they have been removed from the public copy and replaced with `example.invalid` placeholders.

No credentials or student records are included here.

The `.aia` archive contained the Android client. The original Google Apps Script backend code was not included, so this is not the complete deployed system.
