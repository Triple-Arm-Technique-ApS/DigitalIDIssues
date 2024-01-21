# Change Log
All notable changes to this Digital ID will be documented in this file.

## [Unreleased]
https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/30 https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/18
### Added
- Disabled the "+ access button" when the resource disallows access.
- Removed resources that disallow access from the list when applying access for a person or organizational unit (OU).
- Translations for the frontend.
- Implemented two unit tests to check that "access reference nodes" and "can apply reference nodes" are properly rejected by the backend.
- In the integrator API, the pincode is now returned in plain text (while remaining encrypted in the database).
- Fixed issues in the ARX integration

### Changed
- Excluded the encrypted pincode from being returned to the frontend; replaced with a `hasPincode` property.

## 0.0.13 - 1-19-2024

### Added
- Translations for all events.
- Implemented Image Cropper.
- Added a warning in the file upload component for files larger than 10 MB.
- Increased the payload for internal gRPC clients to 50 MB.
- Added "Processed Cards Request" under the Requests Page.
- Added "Pending Ready For Pickup" tile to the dashboard.

### Changed
- Renamed "Smart Cards" to "Credentials".
- Decreased the height of the row on the persons detail page.
- Organized the values on the persons detail page by relevance.
- Updated the UI of the card list on the profile page.
- Enhanced date input fields to include time for more specific intervals.

### Fixed
- Ensured inactive cards are not shown on one's card unless specifically requested on the profile page.
