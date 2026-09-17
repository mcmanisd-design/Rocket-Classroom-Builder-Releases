**Version 1.0.1**

Rocket Classroom Builder is a free desktop utility for creating and safely updating Google Classroom courses from CSV roster data.

Created by **David McManis**

Rocket Classroom Builder is intended to make Google Classroom rostering simpler for school IT staff without requiring administrators to manually build GAM commands for every course.

> **Source code is not distributed with this release.** Rocket Classroom Builder is free to use under the terms in [TERMS.md](TERMS.md).

## What Rocket Classroom Builder Does

Rocket Classroom Builder can:

- Create Google Classroom courses from CSV roster files.
- Assign teachers to new courses.
- Enroll students.
- Reuse existing live courses instead of creating duplicates.
- Add newly assigned teachers and students when roster files are updated.
- Ignore archived courses when determining whether a new live course should be created.
- Create a new live course when the previous matching course has been archived.
- Run imports manually or automatically once each day at a designated time.
- Work with CSV exports from any SIS or roster system as long as the required headers are present.

Rocket Classroom Builder uses an existing GAM installation to communicate with Google Workspace and Google Classroom.

## Requirements

### Google Workspace

You must have:

- A Google Workspace environment with Google Classroom enabled.
- Permission to perform the required Classroom operations.
- Existing Google accounts for teachers and students being rostered.

### GAM 7

Rocket Classroom Builder requires an existing, configured GAM installation.

GAM 7 must already be:

- Installed.
- Authorized.
- Configured for your Google Workspace environment.
- Able to perform Google Classroom operations.

Rocket Classroom Builder does not install, authorize, or configure GAM.

At startup, Rocket attempts to locate GAM automatically. If GAM cannot be found, you can browse to the GAM executable or type/paste its full path. Rocket validates the selected GAM installation before saving it.

## Required CSV Files

File names do not have to follow a specific naming convention. Rocket identifies the files using their headers.

### Teachers CSV

- `Teacher_id`
- `Teacher_email`

### Students CSV

- `Student_id`
- `Student_email`

### Sections CSV

- `Section_id`
- `Course_name`
- `Teacher_id`
- `Period`
- `Term_name`

### Enrollments CSV

- `Section_id`
- `Student_id`

## ProgressBook

ProgressBook users can obtain compatible CSV files through:

**StudentInformation → Local → Report Designer → Vendor Extract**

Common exports include:

- Clever-Enrollment
- Clever Sections
- Clever-Teachers
- Clever-Students

Other SIS and roster systems are supported as long as the required CSV headers match.

## Safe Sync

Rocket Classroom Builder is designed so roster files can be rerun safely.

When Rocket finds an existing live Classroom for the rostered course, it reuses that Classroom instead of creating another one.

Rocket then:

- Adds teachers who are missing.
- Adds students who are missing.
- Leaves existing teachers and students alone.
- Avoids duplicate memberships.

### Important Safety Limitation

**Version 1.0 does not automatically remove teachers or students from Google Classroom.**

If a teacher or student needs to be removed from an existing Classroom, that change must be made manually.

## Archived Courses

Archived Google Classroom courses are not treated as active courses by Rocket Classroom Builder. If the previous Classroom for a rostered course has been archived, Rocket can create a new live Classroom for the current roster.

## Manual Import

1. Open Rocket Classroom Builder.
2. Confirm that GAM shows as ready.
3. Click **Continue to Upload**.
4. Select the four required CSV files.
5. Review the detected roster information.
6. Review the Classroom preview.
7. Start the import.
8. Review the Results screen.

Rocket reports:

- Courses Created
- Courses Updated
- Teachers Added
- Students Added
- New Issues

## Automatic Import

Rocket Classroom Builder can run one automatic roster import each day at the designated time.

1. Choose the folder that will contain the four current CSV files.
2. Select the daily run time.
3. Use **Run Now** to test the folder and roster.
4. Enable daily automatic import.
5. Save the schedule.
6. Leave Rocket Classroom Builder running.

**Rocket Classroom Builder must remain running for an automatic import to occur.**

Version 1.0 does not install a background service or system daemon. If Rocket is closed at the scheduled time, that scheduled import does not run.

### macOS Folder Permission

Before relying on your first scheduled import:

1. Choose the Automatic Import folder.
2. Click **Run Now**.
3. When macOS asks whether Rocket Classroom Builder may access the folder, choose **Allow**.
4. Confirm that Run Now completes successfully.
5. Enable and save the automatic schedule.

Once permission has been granted, scheduled imports can access that folder normally.

### Automatic Import Folder Safety

The Automatic Import folder should contain one current file for each of the four required CSV types.

Rocket stops the automatic import if:

- A required CSV type is missing.
- More than one recognizable CSV of the same type is present.
- Roster validation finds an issue that should be reviewed manually.

## macOS Installation

Rocket Classroom Builder 1.0 is distributed for Apple Silicon Macs.

1. Download the `.dmg` from the official GitHub Release.
2. Open the DMG.
3. Move Rocket Classroom Builder into **Applications**.
4. Launch Rocket Classroom Builder from Applications.

The initial v1.0 build may not be Apple notarized or code signed. macOS may display a security warning on first launch. If macOS prevents the application from opening, use the appropriate **Privacy & Security** controls in System Settings to approve it.

## Privacy and Data

Rocket Classroom Builder processes roster CSV files locally on the computer running the application.

Google Classroom operations are performed through the locally configured GAM installation.

Administrators should follow their organization's policies for storing and protecting student roster information.

## Disclaimer

Rocket Classroom Builder is provided free of charge as a support and administrative utility.

The software is provided **“as is” and without warranty of any kind**, express or implied. While reasonable efforts have been made to test the software and provide safeguards against unintended changes, no software can be guaranteed to be free from errors or defects.

Users and organizations are responsible for reviewing roster data, maintaining appropriate backups and records, testing the software in their own environment, and verifying the results of operations performed through Rocket Classroom Builder.

To the maximum extent permitted by applicable law, the author shall not be liable for direct, indirect, incidental, special, consequential, or other damages, data loss, account changes, service disruption, or other harm arising from the use of, inability to use, or operation of Rocket Classroom Builder.

Use of Rocket Classroom Builder is at the user's own risk.

Rocket Classroom Builder is an independent utility and is not affiliated with, endorsed by, or sponsored by Google, GAM, ProgressBook, or their respective owners.

See [TERMS.md](TERMS.md) for the complete distribution and use terms.

## Version

**Rocket Classroom Builder 1.0.0**

Created by **David McManis**
