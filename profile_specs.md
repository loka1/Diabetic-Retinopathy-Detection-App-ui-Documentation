# Profile Screen Specifications

## Purpose
- View and manage user account details
- Configure app preferences and settings
- Access account management options

## Navigation
- Previous screen: Home screen (via profile button)
- Next screens:
  - Edit profile → Profile editing view
  - Settings → Preferences screen
  - Logout → Returns to login screen

## 1. User Picture
- Circular shape, 120px diameter
- Positioned at top center of screen
- White border (2px thick)
- Subtle shadow (2px)

## 2. User Information
- Name: 24px font size, bold, black
- Email: 16px font size, gray (#666666)
- Spacing between elements: 8px
- Left-aligned (for LTR interface)

## 3. Edit Profile Button
- Pencil icon in top right corner
- Primary color (#3f51b5)
- 40px size
- No text

## 4. Settings Section
### Notification Preferences
- Toggle switch with "Enable Notifications" text
- Sub-options (Email notifications, App notifications)

### Language Selection
- Dropdown with options:
  - English (default)
  - Arabic

### Theme Options
- 3 visual options:
  - Light (default)
  - Dark
  - Auto (follow system)

## 5. Account Management
### Change Password
- Simple button leading to password change form
- Requires current password verification

### Delete Account
- Red button with trash icon
- Leads to confirmation dialog

## 6. Logout Button
- Red color (#f44336)
- At bottom of screen
- Full width (100%)
- "Log Out" text (18px)

## 7. Loading States
- Circular progress indicator for time-consuming operations
- 30% background dimming

## 8. Error/Success States
- Snackbar messages at bottom of screen:
  - Success: Green background (#4caf50)
  - Error: Red background (#f44336)
- Auto-dismiss after 3 seconds

## 9. Confirmation Dialogs
- Appears for:
  - Account deletion
  - Logout
- Contains:
  - Confirmation message
  - "Yes" button (red)
  - "No" button (gray)
- Cannot be dismissed by clicking outside

## Design Notes
- All text in English
- Left-to-right (LTR) text direction
- Margins: 16px all sides
- Vertical spacing between sections: 24px