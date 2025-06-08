# Contact Us Screen Specifications

## Purpose
- Allow users to submit questions/feedback
- Provide official contact information
- Offer customer support access

## Navigation
- Previous screen: Typically accessed from:
  - FAQ screen
  - App menu
  - Profile settings
- Next screens:
  - Submit → Returns to previous screen with confirmation
  - Back → Returns to previous screen

## Layout
- Left-to-Right (LTR) layout
- Form fields in vertical stack
- Fixed submit button at bottom
- Contact information below form

## Components

### Contact Form
1. **Name Field**
   - Placeholder: "Your Name"
   - Input type: text
   - Required validation

2. **Email Field**
   - Placeholder: "Email Address"
   - Input type: email
   - Validation for email format

3. **Subject Field**
   - Placeholder: "Subject"
   - Input type: text
   - Dropdown for common subjects:
     - General Inquiry
     - Technical Support
     - Feedback
     - Other

4. **Message Field**
   - Placeholder: "Your Message"
   - Multiline text input
   - Minimum 10 characters
   - Maximum 500 characters
   - Character counter

### Submit Button
- Full width
- Color: Primary brand color
- Text: "Send Message"
- Disabled until form is valid
- Loading state during submission

### Contact Information
- Displayed below form
- Includes:
  - Email: support@retinopathyapp.com
  - Phone: +1 (555) 123-4567
  - Business hours: Mon-Fri, 9AM-5PM

## States

### Loading State
- Spinner on submit button
- Disabled form fields during submission

### Success State
- Confirmation message: "Message sent successfully"
- Form fields cleared
- Brief checkmark animation

### Error State
- Error message: "Failed to send message"
- Retry button appears
- Form data preserved

## Accessibility
- Proper form labels
- Keyboard navigation between fields
- Screen reader support
- Error messages with ARIA attributes