# Verification Code Screen Specifications (Forgot Password Flow) - LTR Layout

## Purpose
- Second step in password reset process
- Verify user identity via code sent to email
- Security checkpoint before allowing password change

## Navigation
- Previous screen: Forgot password screen
- Next screens:
  - Valid code → Password reset screen
  - Back → Returns to forgot password screen

## Overview
Screen for entering 6-digit verification code sent via SMS/email during password reset flow.

## UI Elements

### 1. Code Input Fields
- Six individual input boxes arranged horizontally (LTR direction)
- Auto-advance to next field on valid digit entry
- Auto-focus on first field on screen load
- Keyboard input handling:
  - Accepts numeric input only
  - Backspace moves to previous field
  - Paste support for full code

### 2. Resend Code Button
- Gray button with text: "Resend Code"
- Disabled state with countdown timer (e.g., "1:30")
- Becomes enabled after countdown completes
- On press:
  - Resends verification code
  - Restarts countdown
  - Shows toast: "Verification code resent"

### 3. States

#### Loading State
- Spinner overlay on code submission
- Disables all inputs
- Text: "Verifying..."

#### Success State
- Green checkmark animation
- Brief display confirmation: "Verification successful"
- Automatic transition to password reset screen

#### Error States
- **Invalid Code**:
  - Red border on all input fields
  - Error message: "Invalid verification code"
  - Clear fields after 3 attempts
- **Expired Code**:
  - Red border on all input fields
  - Error message: "Verification code expired"
  - Auto-enable resend button

### 4. Visual Feedback
- **Correct Digit**:
  - Green border on filled field
  - Checkmark icon
- **Incorrect Attempt**:
  - Red border on all fields
  - Shake animation
- **Complete Code**:
  - All fields show green border
  - Automatic submission

### 5. Back Button
- Top-left arrow button
- Label: "Back"
- Returns to previous screen (email/phone input)
- Confirms navigation if code is partially entered

## Technical Requirements
- 6-digit input validation
- Timer service for countdown
- Keyboard event handling
- Screen transition animations
- LTR text and layout support
- Accessibility:
  - Screen reader support
  - High contrast mode
  - Keyboard navigation

## Copy Text (English)
- Title: "Enter Verification Code"
- Subtitle: "Enter the 6-digit code sent to *******0509"
- Resend: "Resend Code"
- Loading: "Verifying..."
- Success: "Verification successful"
- Invalid: "Invalid verification code"
- Expired: "Verification code expired"
- Back: "Back"