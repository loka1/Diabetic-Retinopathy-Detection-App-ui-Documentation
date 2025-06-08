# Image Upload Screen Specifications

## Purpose
- Capture/select retinal images for analysis
- Prepare images for diabetic retinopathy detection
- Collect optional metadata about the scan

## Navigation
- Previous screen: Home screen (via "New Scan" button)
- Next screens:
  - Successful upload → Analysis results
  - Cancel → Returns to home screen

## Layout
- Right-to-Left (RTL) layout for Arabic text
- Source selection buttons (top section)
- Preview area (70% of screen height)
- Metadata form (below preview)
- Action buttons (fixed bottom)

## Components

### Source Selection
1. **Camera Button**
   - Text: "Take Photo"
   - Icon: Camera
   - Color: Primary (#1976D2)
   - Size: 50% width

2. **Gallery Button**
   - Text: "Choose from Gallery"
   - Icon: Image
   - Color: Secondary (#4CAF50)
   - Size: 50% width

### Image Preview
- Maintains original aspect ratio
- Zoom/pinch gestures enabled
- Crop overlay (square ratio)
- Re-take button (top-right corner)
- Image guidelines overlay (for proper eye positioning)

### Metadata Form
1. **Eye Selection**
   - Label: "Eye"
   - Options:
     - "Right"
     - "Left"
   - Default: None selected (required)

2. **Notes Field**
   - Label: "Notes (Optional)"
   - Placeholder: "Additional notes..."
   - Max length: 200 characters
   - Text direction: LTR

### Upload Button
- Text: "Analyze Image"
- Color: Primary green (#4CAF50)
- Icon: Upload/analyze
- Disabled state: Until image selected
- Loading state: Progress indicator + "Analyzing..."

## States

### Error States
1. Invalid File Type:
   - Message: "Image must be in JPG or PNG format"
   - Visual: Red border + icon

2. Size Limit Exceeded:
   - Message: "Image size too large (maximum 5MB)"
   - Visual: Red border + size indicator

3. Upload Failure:
   - Message: "Upload failed - please try again"
   - Retry button

### Success State
- Progress completion animation
- Auto-navigate to analysis screen
- Success toast message

## Visual Feedback
- Button press animations
- Upload progress indicator
- Field validation states
- Haptic feedback on capture

## Accessibility
- Screen reader support
- High contrast mode
- Keyboard navigation
- Large touch targets