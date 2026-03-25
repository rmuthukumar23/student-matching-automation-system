# Student Peer Matching App

**CS IB Computer Science IA Project**  

An Android application developed for *Students for Students*, a student-run tutoring organization. The app automates matching students who need academic support with available student tutors, replacing a manual Google Sheets workflow. It reduces manual matching time to under 1.5 minutes, manages user authentication, and integrates directly with Google Sheets.

## Project Structure

The repository separates documentation, development artifacts, and the final app:

Peer-match-SOS/  
├─ Development/ – IB CS IA documentation and development files  
│  ├─ Appendix A.pdf – Interview notes with the client  
│  ├─ Appendix B.pdf – Additional reference material  
│  ├─ Criterion_A_Planning.pdf  
│  ├─ Criterion_B_Design.pdf  
│  ├─ Criterion_B_RecordofTasks.pdf  
│  ├─ Criterion_C_Development.pdf  
│  ├─ Criterion_D.mp4 – Video demonstration of the app  
│  └─ Criterion_E_Evaluation.pdf  
└─ Product/  
   └─ SOS Admin App.apk – Android application to install on devices  

Start in the `Development/` folder to review planning, design, development, and evaluation materials. Use `Product/` to access and run the final app.

## How It Works

**Authentication:** Admins log in using credentials managed in an external database.  
**Data Integration:** Student and tutor details are imported from Google Sheets.  
**Matching Algorithm:** The app automatically pairs students with tutors using compatibility criteria.  
**Updating Records:** Matched pairs are assigned unique IDs and written back to Google Sheets.  
**Interface & Communication:** Admins can view unmatched students, matched tutors, and unmatched tutors. Bulk emails can be sent directly from the app.  

This workflow ensures tutoring requests are responded to within 48 hours without manual intervention.

## Features

- Secure login and authentication  
- Automated student-tutor matching (≥90% success rate)  
- Google Sheets integration for importing and updating data  
- Lists of unmatched students, matched tutors, and unmatched tutors  
- Bulk email functionality  
- Intuitive graphical interface based on client feedback  
- Error handling for invalid data input  
- Reduced manual matching time to under 1.5 minutes  

## Technology Stack

- Platform: Android  
- Development Tool: MIT App Inventor (visual block-based programming)  
- Data Integration: Google Sheets via Web API  

## Installation

1. Clone the repository:  
   `git clone git@github.com:rmuthukumar23/student-peer-matching.git`  
2. Install the APK on an Android device:  
   - Navigate to `Product/SOS Admin App.apk`  
   - Enable installation from unknown sources on your Android device  
   - Install the app  

## Usage Guide

1. Log in as admin  
2. Import student and tutor data from Google Sheets  
3. View unmatched students and available tutors  
4. Run the matching algorithm to pair students with tutors  
5. Update Google Sheets with matchup IDs  
6. Send bulk emails to tutors or students as needed
