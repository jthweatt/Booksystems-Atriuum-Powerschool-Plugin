# Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/)
and this project adheres to [Semantic Versioning](http://semver.org/).

## [1.3.0] - 2024-05-22

### Added

- Added teacher query to export School Teachers and Library Media Specialists.

## [1.2.0] - 2022-08-24

### Added

- Added logic to export section's room number and teacher's full name (last, first) if populated.
- Added placeholder for preferred name in needed in furure revisions. Query currently exports null for field.

## [1.1.1] - 2021-09-30

### Fixed

- Corrected the script for the students named query to return only fully enrolled students. Script will now only return rows where student.enroll_status = 0. This eliminates the issue of provisional enrollments being exported until the provision is cleared.

### Fixed

- Corrected the script for the students named query to not return duplicate rows for the same homeroom course with different terms. Script will now only return rows where student.student_statenumber is not null and cc.termid matches the year specified in the script file.

## [1.1.0] - 2021-08-03

### Added

- Added logic to the students named query to return the column "Home_room" as a concattenated string of the Homeroom teacher's section number and last name as "#### lastname".

## [1.0.0] - 2021-07-20

- Initial release build.
