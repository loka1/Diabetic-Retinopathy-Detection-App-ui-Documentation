# Archive/History Screen Specifications

## Purpose
- View previously saved analysis results
- Manage and organize historical scans
- Export/share multiple analyses

## Navigation
- Previous screen: Home screen (via "History" button)
- Next screens:
  - Analysis details → Full result view
  - Export → Sharing options
  - Home → Returns to main dashboard

## Layout
- Left-to-Right (LTR) layout for English text
- Search and filters bar (fixed top)
- Content area (scrollable)
- View mode toggle
- Bulk actions panel (appears on selection)
- Fixed footer navigation (consistent across app)

### Footer Navigation
1. **Home Button**
   - Icon: Home
   - Text: "Home"
   - Active state: Outline icon (not current screen)

2. **New Upload Button**
   - Icon: Camera/upload
   - Text: "New Scan"
   - Position: Center

3. **More Button**
   - Icon: Menu
   - Text: "More"
   - Active state: Filled icon (current screen)

## Components

### Search & Filters
1. **Search Bar**
   - Placeholder: "Search history"
   - Clear button
   - Search icon (right side)
   - Instant results as you type

2. **Filter Controls
   - Date range picker
     - Presets: Today, Week, Month, Year
     - Custom range selector
   - Risk level filters:
     - All (default)
     - Low (green)
     - Medium (yellow)
     - High (red)

3. **View Toggle**
   - Grid view (default)
   - List view
   - Icon size adjustment

### Analysis Items

**Grid View Card:**
- Thumbnail (120x120px rounded)
- Date (DD/MM/YYYY format)
- Time (if same day)
- Risk level badge (corner)
- Quick actions menu (⋮ icon)

**List View Item:**
- Thumbnail (80x80px left)
- Date/time (primary text)
- Risk level (color bar)
- Details preview (1 line)
- Action arrow (right)

**Detailed View:**
- Opens when item clicked
- Shows full analysis
- Comparison tools
- Export options

### Bulk Actions
- **Selection Mode**
  - Checkboxes appear
  - Counter shows selected count
  - Select all/none options

- **Available Actions**
  1. Export (PDF/CSV)
  2. Share (multiple formats)
  3. Delete (with confirmation)

## States

### Loading State
- Skeleton loading cards
- Progressive loading
- Pagination loader

### Empty State
- Illustration (folder with magnifying glass)
- Title: "No saved analyses"
- Subtext: "Your analyses will be saved here automatically"
- CTA: "Upload first image"

### Error State
- Error icon
- "Failed to load history"
- Retry button
- Contact support link

## Visual Feedback
- Smooth scrolling
- Card hover/focus states
- Selection animations
- Action transitions

## Accessibility
- Screen reader support
- Keyboard navigation
- High contrast mode
- Text size scaling