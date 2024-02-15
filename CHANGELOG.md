# Change Log
All notable changes to this Digital ID will be documented in this file.

## 0.1.4 - 15-02-2024

### Added
- Feature to disable Keycloak Admin UI, enhancing security and reducing potential unauthorized access. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/31
- Integration of Serilog for sending logs to Loki, improving logging capabilities and system monitoring. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/61
- Capability to crop pictures directly within the mobile app, awaiting release, to enhance user experience and provide better control over profile image presentation. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/63
- Functionality for operators to submit requests on behalf of users, streamlining the process and improving operational efficiency. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/64


## 0.1.3 - 14-02-2024

### Fixed
- Second person signing in becomes system owner, resolving potential security and access control issues. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/66
- Issue where a person is moved to entity root if the user already exists with the same identity provider ID property but is in a different group, ensuring correct group association. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/69
- Unable to remove nodes due to card design package reference nodes blocking, enhancing system flexibility and user control over their configurations. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/71

## 0.1.2 - 08-02-2024

### Added
- Refinement of default filters for node types with expiry to enhance user experience. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/37
- Display of profile pictures in square format for a unified visual approach. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/54
- Linking of existing card design package to Organization Unit for streamlined management. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/53
- Simplification of Person Details view, including the addition of Edit and Print Card buttons for enhanced usability.  https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/55
- Display of the newest requests and cards at the top of tables, ensuring immediate visibility of recent items.  https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/26

### Changed
- Renamed "Send to Print Card" button in Print Card Slide-Over for clearer action indication.  https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/56

### Fixed
- Incorrect navigation of "See All" links on Dashboard Tiles, ensuring accurate redirection. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/36
- Missing groups in card design package retrieval for printing, guaranteeing inclusion of all necessary elements. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/39
- Incorrect timestamps for events, aligning them accurately with the actual time events occurred. https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/9
- Minor bugs in the ui
- Unable to Assign Access from UI Under Organization Unit.  https://github.com/Triple-Arm-Technique-ApS/DigitalIDIssues/issues/60

## 0.1.1 - 1-2-2024

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
