# Rocket Classroom Builder v1.1.0
**Smarter Scheduling. Simpler Experience.**

Rocket Classroom Builder v1.1.0 introduces a redesigned interface and new scheduling features that make managing Google Classroom rosters easier than ever.

This release focuses on simplicity, flexibility, and automation while preserving the core functionality that makes Rocket Classroom Builder a useful, free tool for school IT departments.

## What's New

### 🚀 A Completely Redesigned Interface

Rocket Classroom Builder now features a clean, modern dark interface designed to make classroom management easier.

- Simple, three-step workflow: **Choose Files → Choose Terms → Start Syncing**
- Larger buttons, clearer navigation, and improved readability
- Modern dark theme with streamlined controls
- Less clutter, with technical information available when needed
- Easier access to manual and automatic imports

### 📅 Term-Based Synchronization

You now have control over which academic terms Rocket Classroom Builder synchronizes.

Independently enable or disable:

- **All Year (AY)**
- **1st Semester (1)**
- **2nd Semester (2)**

For example, schools can synchronize All Year and 1st Semester classes during the fall, then switch to All Year and 2nd Semester classes in the spring.

Courses belonging to disabled terms are skipped without modifying their existing Google Classrooms.

### ⏰ Automatic Term Scheduling

Take the guesswork out of semester transitions.

Administrators can now assign optional start and end dates to each academic term.

- Configure synchronization dates for individual terms.
- Automatically include or exclude terms based on the current date.
- Leave dates blank to synchronize an enabled term anytime.
- Save settings for future imports.
- Apply the same term settings to manual and automatic synchronization.

Set up your academic year once, and Rocket Classroom Builder can automatically follow your schedule whenever imports run.

### ✨ Simplified Import Experience

The updated interface makes it easier to choose between running an immediate import and configuring daily automatic synchronization.

Your existing automatic import functionality remains available, including saved roster folders and scheduled run times.

## Improvements

- Improved organization of synchronization settings.
- Simplified access to optional date scheduling.
- Clearer visual indicators for selected academic terms.
- Reduced unnecessary instructions and technical clutter.
- Preserved existing Classroom duplicate protection and roster synchronization functionality.
- Maintained compatibility with existing CSV roster workflows.

## Important Notes

**Automatic Imports:** Rocket Classroom Builder must remain running for scheduled imports to execute.

**macOS Folder Permissions:** Before your first scheduled import, use Run Now and approve access to your selected roster folder when macOS prompts you.

**Term Filtering:** Disabling a term or moving outside its scheduled date range does not automatically archive, delete, or modify existing Google Classrooms.

**GAM Requirement:** A properly installed and authorized GAM environment is required. Each organization must configure GAM using its own Google Workspace credentials.

## Upgrading from v1.0.1

Version 1.1.0 is designed to retain existing functionality while adding new scheduling controls and the redesigned interface.

After upgrading, review your selected academic terms and optional synchronization dates before running your first import.

We recommend performing an initial manual test before enabling automatic synchronization.

## Availability

Rocket Classroom Builder is provided **free of charge** as a support utility for schools and Google Workspace administrators.

The software is provided **“AS IS,” without warranties of any kind**. The developers and distributors are not responsible for data loss, unintended changes, service disruptions, or other damages arising from its use, to the extent permitted by applicable law.

Administrators should review their roster data and test synchronization settings before making changes to production Google Classroom environments.

---

**Rocket Classroom Builder v1.1.0**

*Making Google Classroom management simpler, one school at a time.*

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
