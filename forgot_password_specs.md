# Forgot Password Email Input Screen Specifications

## Purpose
- Initiate password reset process
- Verify user identity via registered email
- First step in password recovery flow

## Navigation
- Previous screen: Login screen (via "Forgot password?" link)
- Next screens:
  - Valid email → Verification code screen
  - Back → Returns to login screen

## Layout
- Left-to-Right (LTR) layout for English text
- Vertical stack of components with appropriate spacing

## Components

### Email Input Field
- Position: Top of screen
- Width: 90% of parent container
- Auto-focus: Enabled on screen load
- Keyboard:
  - Submit behavior: Enter key triggers "Send Code" action
- Placeholder text: "Email"
- Text direction: LTR
- Input type: email

### Send Code Button
- Position: Below email input field
- Width: 100% of parent container
- Color: Blue (#2563EB)
- Text: "Send Code"
- Disabled state: When email is empty or invalid
- Loading state: Spinner with disabled interaction during API call

### Back to Login Link
- Position: Below Send Code button
- Text: "Back to Login"
- Color: Secondary color (#6B7280)
- Action: Navigates back to login screen

## States

### Error States
1. Invalid Email Format:
   - Red border around input field (#DC2626)
   - Error message below field: "Invalid email format"
   
2. Unregistered Email:
   - Red border around input field (#DC2626)
   - Error message below field: "Email not registered"

### Loading State
- Button shows loading spinner
- All inputs and buttons disabled
- Text changes to "Sending..."

### Success State
- Success message displayed: "Code sent successfully"
- Checkmark icon next to message
- Email input field disabled
- Button changes to secondary state

## Visual Feedback
- Success animation (checkmark) when code is dispatched
- Haptic feedback on successful submission
- Button press animation

## Accessibility
- Screen reader support for all text and states
- Proper contrast ratios for text and interactive elements
- Keyboard navigation support