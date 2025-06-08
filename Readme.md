# Diabetic Retinopathy Detection App Documentation

## Application Overview
A mobile application for early detection of diabetic retinopathy using AI analysis of retinal images. The app guides users through image capture, analysis, and result interpretation.

**Key Features:**
- Secure user authentication
- Retinal image upload and analysis
- AI-powered diagnosis with risk assessment
- Historical results tracking
- Educational resources

## Screen Specifications

### App Entry Flow
1. [Splash Screen](splash_screen_specs.md)
2. [Guest Home Screen](guest_home_screen_specs.md)

### Authentication Flow
3. [Login Screen](login_screen_specs.md)
4. [Sign Up Screen](signup_specs.md)
2. [Forgot Password](forgot_password_specs.md)
3. [Verification Code](verification_code_specs.md)
4. [Change Password](change_password_specs.md)

### Main Application
5. [Home Screen](home_screen_specs.md) (After login)
6. [Image Upload](image_upload_screen_specs.md)
7. [Analysis Results](analysis_result_screen_specs.md)
8. [Archive/History](archive_history_screen_specs.md)

### Additional Screens
9. [Profile](profile_specs.md)
10. [FAQ](faq_screen_specs.md)
11. [Privacy Policy](privacy_policy_screen_specs.md)
12. [Terms of Use](terms_of_use_screen_specs.md)
13. [Contact Us](contact_us_screen_specs.md)

## Technical Specifications
- **Platform:** iOS and Android
- **Languages:** English (LTR support)
- **Design System:**
  - Colors: Primary (#1976D2), Secondary (#4CAF50), Error (#DC2626)
  - Typography: Standard mobile fonts
  - Spacing: 8px grid system

## Development Notes
- All screens follow consistent LTR layout conventions
- Accessibility compliance: WCAG 2.1 AA
- Performance targets:
  - Image upload < 5MB
  - Analysis time < 30 seconds

## Version History
- v1.0 (Current): Initial release with core functionality
- v1.1 (Planned): Doctor consultation integration