# Students for Students Tutor Matching App

Android admin app built for **Students for Students**, a student-run tutoring initiative. It was made to reduce the manual work involved in matching students with tutors through Google Sheets.

> The project grew out of a real problem I had been thinking about for Students for Students: tutor matching was becoming too manual and repetitive. I later developed the idea into a working solution through my **IB Computer Science HL Internal Assessment (IA)**, using the IA process to plan, design, implement, test and evaluate the app. The app was completed before March 2025. I did not use GitHub during the original development, so this repository is a later archive of the project.

## The problem

Tutor requests and tutor availability were being managed manually in spreadsheets. As more requests came in, finding suitable matches and keeping track of them became slow and repetitive.

I built an admin app that kept the existing Google Sheets workflow but made it easier to search requests, review student and tutor details, and move through the matching process.

## What it does

- admin login and input validation
- loads student and tutor requests from Google Sheets through Google Apps Script
- searches requests by ID
- shows grade and subject information
- passes selected students into the matching flow
- handles invalid or missing responses
- supports the wider matching workflow documented in the project report

## Results

The project evaluation recorded:

- matching time reduced to **under 1.5 minutes**
- **90%+ matching success** in the tested scenarios
- a workflow designed to respond to tutoring requests within **48 hours**

These figures come from the original project evaluation.

## Tech

- MIT App Inventor / Blockly
- Android
- Google Apps Script
- Google Sheets
- JSON web responses

## Repository

```text
├── Source/       Sanitized App Inventor block source
├── Product/      Android APK
├── Development/  IB Computer Science HL IA documentation
└── README.md
```

The original App Inventor project used external Google Apps Script endpoints. The live URLs have been removed from the public source and replaced with placeholders. No student data or credentials are included.

The recovered source is the Android client side of the project. The original Apps Script backend code was not part of the archived `.aia` file.

## What the IA Criteria mean

The files in [`Development/`](Development/) are organised using the assessment structure of the **IB Computer Science HL Internal Assessment**. The names `Criterion A`, `Criterion B`, and so on come from the IB coursework, not from this repository.

In this project:

- **Criterion A - Planning:** defines the problem, client, requirements and success criteria
- **Criterion B - Design:** documents the proposed system and interface design; the accompanying Record of Tasks tracks the development process
- **Criterion C - Development:** explains how the solution was implemented and the technical decisions behind it
- **Criterion D - Functionality evidence:** the video demonstrates the finished product working
- **Criterion E - Evaluation:** evaluates the final solution against the original success criteria and reflects on the outcome
- **Appendices:** contain supporting material referenced by the IA documentation

This documentation is useful beyond the coursework itself because it records the full path from identifying the problem through design, implementation and evaluation.

## Source

The most useful implementation files are in [`Source/`](Source/):

- `Screen1.bky` - login and authentication flow
- `StudentRequests.bky` - student data retrieval, search and selection
- `TutorRequests.bky` - tutor data retrieval and search
- `MatchScreen.bky` - selected-student handoff into the matching flow

For the full project process, see [`Development/`](Development/). The archived Android build is in [`Product/`](Product/).

## Running the app

The APK is an archived build and depends on the original external services, so it may no longer work as a standalone app.

```bash
git clone https://github.com/rmuthukumar23/student-matching-automation-system.git
cd student-matching-automation-system
```

The APK is available at `Product/SOS Admin App.apk`.
