# Splash Screen Specifications

## Purpose
- First screen users see when opening the app
- Displays branding while app initializes
- Provides smooth transition to login/home screen

## Layout
- Full-screen with app logo centered
- Loading indicator below logo
- Background: Solid brand color (#1976D2)

## Components

### App Logo
- Size: 150x150 pixels
- Position: Center of screen (vertical & horizontal)
- Animation: Gentle fade-in (500ms)

### Loading Indicator
- Circular progress spinner
- Color: White
- Size: 32x32 pixels
- Position: 40px below logo

### Version Info
- Small text at bottom: "v1.0" 
- Color: White with 70% opacity
- Size: 12px

## Timing
- Minimum display time: 2 seconds
- Maximum display time: 5 seconds (if loading takes longer)
- Transition animation: 300ms fade to next screen

## States

### Loading State
- Spinner rotating
- No interaction possible

### Error State
- If initialization fails:
  - Spinner stops
  - Error message appears
  - Retry button appears

## Navigation
- Next screen:
  - Successful load → Guest home screen (if not authenticated)
  - Successful load → Home screen (if authenticated)
  - Error → Stays on splash with retry option

## Technical Notes
- No network requests during splash
- Cache critical assets to ensure fast loading
- Ensure smooth 60fps animations