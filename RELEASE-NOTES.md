# Rocket Classroom Builder 1.0.0 — Release Notes

## Initial Release

Rocket Classroom Builder 1.0.0 is the first public release of the free Rocket Classroom rostering utility.

Created by **David McManis**

## Features

- CSV-based Google Classroom creation using Teachers, Students, Sections, and Enrollments data.
- Safe Sync that reuses existing live Classrooms instead of duplicating them.
- Adds newly assigned teachers and newly enrolled students.
- Archived course rollover so an archived Classroom does not prevent creation of the next live course.
- GAM automatic detection, browse selection, typed/pasted executable path, validation, and saved configuration.
- Automatic Import using one roster folder and one daily run time.
- **Run Now** and Last Run status.
- Results reporting for Courses Created, Courses Updated, Teachers Added, Students Added, and New Issues.

## Safety Behavior

Rocket Classroom Builder 1.0 is intentionally conservative when modifying existing Google Classrooms.

It adds missing roster memberships but does **not automatically remove teachers or students**.

Membership removals must be performed manually in version 1.0.

## macOS Notes

The initial macOS release targets Apple Silicon Macs.

macOS may require permission before Rocket can read an Automatic Import folder. Mac users should use **Run Now** once after selecting the roster folder and approve folder access when prompted.

Rocket Classroom Builder 1.0 may be distributed without Apple code signing/notarization. macOS may therefore require the administrator to manually approve the application on first launch.

## Known Limitations

- GAM must be installed and configured separately.
- Rocket does not install, authorize, or configure GAM.
- Automatic Import runs only while Rocket Classroom Builder remains open.
- Automatic Import supports one folder and one daily time.
- Version 1.0 does not automatically remove teachers or students.
- The macOS v1 release targets Apple Silicon.
- Windows support is included in the application design but was not fully validated at the time of the initial macOS release.

## Distribution

Rocket Classroom Builder is distributed as a compiled application free of charge.

The application source code is proprietary and is not included in the public release.

See `TERMS.md` for permitted use and distribution terms.

## Disclaimer

Rocket Classroom Builder is provided free of charge as a support utility, **as is and without warranty**.

Users are responsible for testing the software in their environment, reviewing roster data, and verifying resulting Google Classroom changes.

To the maximum extent permitted by applicable law, the author shall not be liable for damages, data loss, account changes, service disruption, or other harm arising from the use of or inability to use Rocket Classroom Builder.

## Version

**Rocket Classroom Builder 1.0.0**

Author: **David McManis**
