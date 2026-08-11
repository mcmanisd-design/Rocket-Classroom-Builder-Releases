# Rocket Classroom Builder — Quick Start

**Version 1.0.0**

## 1. Install and Configure GAM

Rocket Classroom Builder requires a working GAM 7 installation.

GAM 7 must already be installed, authorized, and configured for your Google Workspace environment. Rocket does not install or configure GAM.

## 2. Open Rocket Classroom Builder

Launch Rocket Classroom Builder.

Rocket will attempt to locate GAM automatically. If GAM is not found:

- Browse to the GAM executable, or
- Type/paste the full GAM executable path.

Rocket will test GAM before saving the location.

## 3. Prepare Four CSV Files

### Teachers

`Teacher_id, Teacher_email`

### Students

`Student_id, Student_email`

### Sections

`Section_id, Course_name, Teacher_id, Period, Term_name`

### Enrollments

`Section_id, Student_id`

The filenames do not matter. Rocket identifies the files using their headers.

## 4. Run Your First Import

1. Click **Continue to Upload**.
2. Select all four CSV files.
3. Review the detected roster and Classroom preview.
4. Start the import.
5. Review Courses Created, Courses Updated, Teachers Added, Students Added, and New Issues.

## 5. Rerunning Rosters Is Safe

Rocket reuses an existing live Classroom rather than creating another one.

Missing teachers and students are added. Existing memberships are not duplicated.

**Rocket 1.0 does not remove memberships.** Teachers and students who should be removed must be removed manually from Google Classroom.

## 6. Automatic Import

1. Choose your roster folder.
2. Choose the daily run time.
3. Click **Run Now** and verify the import.
4. Enable daily automatic import.
5. Click **Save Schedule**.
6. Leave Rocket Classroom Builder running.

Rocket runs the current roster files in that folder when the selected time arrives.

If Rocket is closed, the scheduled import cannot run.

### macOS Users

Before relying on the first scheduled import, click **Run Now** once.

When macOS asks for permission to access the selected CSV folder, choose **Allow**.

Once folder access has been granted, scheduled imports can use that folder automatically.

## 7. Archived Classrooms

Archived Classrooms do not prevent Rocket from creating the next live Classroom.

Rocket ignores archived courses when determining whether an active course already exists.

## Important

Rocket Classroom Builder is a free support utility provided **as is and without warranty**.

Administrators are responsible for reviewing source roster data, testing the software in their environment, and verifying changes made to their Google Classroom environment.

Use of the software is at the user's own risk.

The application is free to use, but the source code is proprietary and is not distributed with the release. See `TERMS.md`.

## Three Things to Remember

**GAM must already work.**

**Rocket 1.0 adds roster memberships but never removes them automatically.**

**Rocket must remain open for scheduled imports.**
