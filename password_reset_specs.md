# Password Reset Screen Specifications (English)

## Purpose
- Final step in password recovery flow
- Set new secure password for account
- Complete authentication process

## Navigation
- Previous screen: Verification code screen
- Next screens:
  - Success → Login screen
  - Cancel → Returns to login screen

## Layout
- Left-to-Right (LTR) layout for English text
- Vertical stack of components with appropriate spacing
- Consistent with existing auth flow design language

## Components

### New Password Input Field
- Position: Top of screen
- Width: 90% of parent container
- Auto-focus: Enabled on screen load
- Placeholder text: "New password"
- Input type: password
- Password strength meter below field (visual indicator)
  - Weak: Red (less than 8 chars, no complexity)
  - Medium: Yellow (8+ chars, some complexity)
  - Strong: Green (12+ chars with mixed case, numbers, symbols)
- Text direction: LTR

### Confirm Password Field
- Position: Below new password field
- Width: 90% of parent container
- Placeholder text: "Confirm password"
- Input type: password
- Text direction: LTR

### Password Requirements Checklist
- Position: Below password fields
- Dynamic validation showing:
  - "Minimum 8 characters" - ✓/✗
  - "Upper and lower case letters" - ✓/✗
  - "At least one number" - ✓/✗
  - "At least one special character" - ✓/✗
- Updates in real-time as user types

### Reset Password Button
- Position: Below checklist
- Width: 100% of parent container
- Color: Green (#10B981)
- Text: "Reset Password"
- Disabled state: When passwords don't match or requirements not met
- Loading state: Spinner with "Updating..." text

## States

### Error States
1. Weak Password:
   - Red border around new password field (#DC2626)
   - Error message: "Password too weak"
   
2. Password Mismatch:
   - Red border around confirm password field (#DC2626)
   - Error message: "Passwords don't match"

### Loading State
- Button shows loading spinner
- All inputs disabled
- Button text changes to "Updating..."

### Success State
- Success message: "Password updated successfully"
- Checkmark animation
- Auto-redirect to login screen after 3 seconds
- Visual feedback: Brief green flash overlay

## Keyboard Navigation
- Tab order: New password → Confirm password → Reset button
- Enter key:
  - In fields: Moves to next field
  - On button: Triggers reset action
- Escape key: Blurs current field

## Accessibility
- Screen reader support for all text and states
- ARIA labels for password requirements
- Proper contrast ratios (4.5:1 minimum)
- Focus states for all interactive elements