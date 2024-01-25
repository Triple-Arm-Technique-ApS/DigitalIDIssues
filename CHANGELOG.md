# Change Log
All notable changes to this Digital ID will be documented in this file.

## [0.1.1] - [Release Date]

### Added
- Default Card Designs for Organization Units. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/4
- Optimization for Card Design Rendering. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/10
- Activation of Retry Mechanism for Printing Client. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/44

### Changed
- Updated Card Printer Details Page with new translations and field name changes. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/35

### Fixed
- Incorrect Dialog shown when blocking a card from the Profile List. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/33
- Issue with the Change Pincode feature in the Mobile App (needs release). https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/42
- Missing Loading State in Block Card Modal. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/29

## 0.1.0 - 1-24-2024
https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/30 https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/18
### Added
- Disabled the "+ access button" when the resource disallows access.
- Removed resources that disallow access from the list when applying access for a person or organizational unit (OU).
- Translations for the frontend.
- Implemented two unit tests to check that "access reference nodes" and "can apply reference nodes" are properly rejected by the backend.
- In the integrator API, the pincode is now returned in plain text (while remaining encrypted in the database).
- Fixed issues in the ARX integration
- Fixed issues with file import, the downloaded template will now work, unless it has been run previously

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
