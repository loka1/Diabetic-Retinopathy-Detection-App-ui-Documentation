# FAQ Screen Specifications

## Purpose
- Provide answers to common questions
- Help users troubleshoot issues
- Offer guidance on app features

## Navigation
- Previous screen: Home screen (via FAQ link)
- Next screens:
  - Expanded FAQ item → Shows detailed answer
  - Back → Returns to previous screen

## Layout
- Left-to-Right (LTR) layout
- Search bar at top
- Scrollable list of questions below
- Fixed footer navigation

## Components

### Search Bar
- Placeholder: "Search FAQs"
- Clear button appears when typing
- Real-time filtering of questions

### FAQ Items
- Each question in an expandable card
- Default state: Only question visible
- Expanded state: Shows answer with 16px padding
- Chevron icon indicates expand/collapse state

### Categories
- Optional category filter tabs above list
- Categories: General, Account, Technical, Payments

## States

### Empty Search State
- Illustration: Magnifying glass
- Text: "No results found"
- Subtext: "Try different keywords"

### Loading State
- Skeleton loading for FAQ items
- 3 placeholder cards while loading

## Accessibility
- Screen reader support
- Keyboard navigation between items
- Proper heading hierarchy
- Sufficient color contrast