# Login Screen Specifications

## Purpose
- Entry point for registered users to access the app
- Validates user credentials and initiates authenticated session

## Navigation
- Previous screen:
  - Splash screen (first launch)
  - Forgot password screen (if returning)
  - Registration screen (if returning)
- Next screens:
  - Successful login → Home screen
  - Forgot password → Password recovery flow
  - Sign up → Registration flow

## Layout
- Left-to-Right (LTR) layout for English text
- Vertical stack of components with 16px spacing
- Form width: 90% of container
- Logo positioned above form fields (150px top margin)

## Components

### Email/Phone Input
- Position: Top of form
- Width: 90% of parent container
- Placeholder: "Email or phone number"
- Input type: text with dynamic keyboard (email/number)
- Auto-capitalize: none
- Auto-correct: off
- Text direction: LTR
- Validation: Real-time format checking

### Password Field
- Position: Below email/phone input
- Width: 90% of parent container
- Placeholder: "Password"
- Input type: password (with eye icon toggle)
- Minimum 8 characters validation
- Show password strength meter

### Login Button
- Position: Below password field
- Width: 100% of parent container
- Color: #1976D2 (primary blue)
- Text: "Sign In"
- Disabled state: When form is invalid
- Loading state: Spinner during authentication

### Secondary Actions
1. "Forgot password?" link
   - Position: Below login button
   - Color: #6B7280 (secondary)
   - Action: Navigates to forgot password

2. "Don't have an account? Sign up" link
   - Position: Below forgot password link
   - Color: #2563EB (primary)
   - Action: Navigates to signup

## States

### Error States
1. Invalid Email/Phone:
   - Red border (#DC2626)
   - Error message: "Invalid format"

2. Wrong Credentials:
   - Red border on both fields
   - Error message: "Incorrect email/password"

3. Account Locked:
   - Special icon + "Account temporarily locked"
   - Contact support CTA

### Loading State
- Button shows loading spinner
- All inputs disabled
- Text changes to "Authenticating..."
- No interaction during API call

### Success State
- Checkmark animation
- Success message: "Login successful"
- Auto-redirect to home after 1.5s

## Visual Feedback
- Button press animation
- Field focus highlights
- Haptic feedback on errors/success

## Accessibility
- Screen reader support for all text
- Proper contrast ratios
- Keyboard navigation support
- Large touch targets (min 48x48px)