# Privacy Policy Screen Specifications

## Purpose
- Display app's data handling practices
- Explain user privacy protections
- Obtain consent for data processing

## Navigation
- Previous screen: Typically accessed from:
  - Registration flow
  - App settings
  - Profile screen
- Next screens:
  - Accept → Continues registration/settings flow
  - Back → Returns to previous screen

## Layout
- Left-to-Right (LTR) layout
- Title at top with back button
- Scrollable content area
- Accept button fixed at bottom

## Components

### Header
- Back button (left)
- Title: "Privacy Policy" (center)
- No additional actions

### Content Section
- Divided into logical sections:
  1. Data Collection
  2. Data Usage
  3. Data Sharing
  4. User Rights
  5. Contact Information
- Each section has:
  - Section heading (18px bold)
  - Paragraph text (16px regular)
  - Adequate spacing

### Accept Button
- Full-width button at bottom
- Color: Primary brand color
- Text: "I Accept"
- Disabled until user scrolls to bottom
- Shows loading state during submission

## States

### Loading State
- Shows when policy is being loaded
- Skeleton loading for content sections

### Accepted State
- Checkmark animation
- Brief success message
- Auto-redirect after 2 seconds

## Accessibility
- Proper heading hierarchy
- Sufficient text contrast
- Screen reader friendly
- Text size scaling support