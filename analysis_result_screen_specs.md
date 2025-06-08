# Analysis Result Screen Specifications

## Purpose
- Displays diabetic retinopathy analysis results
- Provides risk assessment and recommendations
- Allows saving/sharing results

## Navigation
- Previous screen: Image upload screen
- Next screens:
  - Save → Archive/history screen
  - Share → Device sharing options
  - Home → Returns to main dashboard

## Layout
- Right-to-Left (RTL) layout for Arabic text
- Split view (50/50):
  - Left: Original image
  - Right: Analysis overlay
- Result summary (below images)
- Action buttons (above footer)
- Fixed footer navigation (consistent across app)

### Footer Navigation
1. **Home Button**
   - Icon: Home
   - Text: "الرئيسية"
   - Active state: Outline icon (not current screen)

2. **New Upload Button**
   - Icon: Camera/upload
   - Text: "رفع طلب جديد"
   - Position: Center

3. **More Button**
   - Icon: Menu
   - Text: "المزيد"

## Components

### Image Comparison
- **Slider Control**
  - Thumb style: Circular knob
  - Track: 4px width
  - Default position: Center
  - Smooth transition animation

- **View Options**
  - Heatmap toggle (on/off)
  - Zoom controls (+/- buttons)
  - Pan gestures enabled
  - Fullscreen mode

### Findings Section
1. **Risk Level Indicator**
   - Color-coded (green/yellow/red)
   - Percentage value (0-100%)
   - Icon matching severity

2. **Affected Areas**
   - List of detected issues
   - Each item shows:
     - Region name
     - Severity (1-5 stars)
     - Confidence percentage

3. **Detailed Findings**
   - Scientific terminology
   - Layman's explanation
   - Visual markers on image

### Recommendations
- **Urgency Level**
  - Color-coded badge
  - Text description
  - Suggested timeframe

- **Actions**
  1. Primary: "Consult Doctor"
  2. Secondary: "Re-analyze"
  3. Tertiary: "Save Results"

- **Follow-up Steps**
  - Medication suggestions
  - Lifestyle changes
  - Monitoring instructions

## States

### Loading State
- Skeleton loading for images
- Progress indicator
- "Processing Results..." text

### Error State
- Error icon
- "Failed to load results" text
- Retry button

### Saved State
- Success animation
- "تم الحفظ بنجاح" toast
- Auto-archive option

## Visual Feedback
- Heatmap transitions
- Interactive elements hover states
- Button press animations
- Smooth view transitions

## Accessibility
- Screen reader support
- High contrast mode
- Keyboard navigation
- Text size scaling