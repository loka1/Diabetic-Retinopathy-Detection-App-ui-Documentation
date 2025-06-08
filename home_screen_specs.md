# Home Screen (After Login) Specifications

## Purpose
- Main dashboard after successful login
- Provides quick access to key app features
- Displays recent analyses and notifications

## Navigation
- Previous screen: Login screen
- Next screens:
  - Image upload → New analysis flow
  - Archive → History view
  - Profile → Account management
  - FAQ → Help section

## Layout
- Right-to-Left (RTL) layout for Arabic text
- App bar with user avatar and notifications (fixed top)
- Welcome message section below app bar
- Quick action buttons (primary CTAs)
- Recent analyses section (scrollable)
- Fixed footer navigation (present on all post-login screens)

### Footer Navigation
1. **Home Button**
   - Icon: Home
   - Text: "Home"
   - Action: Returns to home screen
   - Active state: Filled icon when on home

2. **New Upload Button**
   - Icon: Camera/upload
   - Text: "New Scan"
   - Action: Opens image upload screen
   - Position: Center (prominent)

3. **More Button**
   - Icon: Menu
   - Text: "More"
   - Action: Opens side menu with:
     - Profile
     - History
     - FAQ
     - Settings
     - Logout

## Components

### App Bar
- User avatar (circular, 40px diameter)
- Position: Top right
- Notification badge (red dot for new)
- App title/text logo (left aligned)

### User Greeting
- Text: "Welcome [Name]"
- Subtext: "How are you today?"
- Text direction: RTL
- Typography:
  - Title: 24px bold
  - Subtext: 16px regular

### Quick Actions
1. **Upload New Image Button**
   - Text: "Upload New Image"
   - Color: #4CAF50 (primary green)
   - Icon: Camera/upload
   - Size: Full width with 16px margins

2. **View Archive Button**
   - Text: "View Archive"
   - Color: #1976D2 (secondary blue)
   - Icon: History
   - Size: Full width with 16px margins

3. **FAQ Link**
   - Text: "FAQ"
   - Color: #6B7280 (tertiary)
   - Icon: Question mark
   - Position: Below buttons

### Recent Analyses Section
- Title: "Recent Analyses"
- Layout: Horizontal scrollable list
- Item components:
  - Thumbnail (80x80px rounded corners)
  - Date (DD/MM format, 12px)
  - Risk level indicator (color-coded badge)
  - Tap area: Entire card

## States

### Empty State
- Illustration (magnifying glass + eye)
- Text: "No previous analyses"
- CTA button: "ابدأ بتحميل صورتك الأولى"
  - Color: Primary green
  - Icon: Upload
  - Centered below illustration

### Loading State
- Skeleton loading for recent analyses
- Placeholder cards (3 items)
- Shimmer animation

### Error State
- Error icon
- Text: "Could not load data"
- Retry button

## Visual Feedback
- Button press animations
- Card hover/focus states
- Smooth scrolling behavior
- Loading transitions

## Accessibility
- Screen reader support
- Proper contrast ratios
- Keyboard navigation
- Large touch targets