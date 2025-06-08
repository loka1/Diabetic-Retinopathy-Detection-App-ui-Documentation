# Terms of Use Screen Specifications

## Purpose
- Display app's terms and conditions
- Explain user rights and responsibilities
- Obtain agreement to terms

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
- Title: "Terms of Use" (center)
- No additional actions

### Content Section
- Divided into numbered clauses:
  1. Acceptance of Terms
  2. User Responsibilities
  3. Intellectual Property
  4. Limitations of Liability
  5. Governing Law
- Each clause has:
  - Clause number and title (18px bold)
  - Paragraph text (16px regular)
  - Adequate spacing between clauses

### Accept Button
- Full-width button at bottom
- Color: Primary brand color
- Text: "I Accept"
- Disabled until user scrolls to bottom
- Shows loading state during submission

## States

### Loading State
- Shows when terms are being loaded
- Skeleton loading for content sections

### Accepted State
- Checkmark animation
- Brief success message: "Terms accepted"
- Auto-redirect after 2 seconds

## Accessibility
- Proper heading hierarchy
- Sufficient text contrast (4.5:1 minimum)
- Screen reader friendly structure
- Support for text resizing