# Campus Lost & Found - Design Guidelines

## Design Approach
**Utility-Focused Design System** - Inspired by Craigslist's functional simplicity and community bulletin boards. This is a tool for rapid information exchange, not a marketing site. Prioritize clarity, scannability, and immediate access to listings over visual flourishes.

## Typography
- **Primary Font**: Roboto (Google Fonts)
- **Hierarchy**: 
  - Page titles: 32px bold
  - Section headers: 24px semibold
  - Card titles: 18px medium
  - Body text: 16px regular
  - Labels/metadata: 14px regular

## Layout System
**Spacing Units**: Use Tailwind's 4-unit scale (p-4, m-4, gap-4, etc.) consistently throughout. 16px base spacing creates clean, predictable rhythm.

**Container Strategy**:
- Max-width: 1200px centered container
- Page padding: px-4 on mobile, px-6 on desktop
- No hero section - lead directly with counters and action buttons

## Component Library

### A. Header
- Simple horizontal bar with logo/site name (left) and "Report Lost" / "Report Found" action buttons (right)
- Sticky positioning for easy access
- Background: white with subtle bottom border

### B. Statistics Counters (Below Header)
- Three prominent stat boxes in horizontal row (grid on mobile)
- Lost Items (orange accent), Found Items (green accent), Returned Items (blue accent)
- Large numbers (48px bold) with small labels below
- Light background cards with colored left border

### C. Listing Cards Grid
- 3-column grid on desktop, 2-column on tablet, 1-column on mobile
- Each card includes:
  - Square image thumbnail at top (240x240px, object-cover)
  - Item title/description (2-line clamp)
  - Reporter name
  - Contact info badges (phone with icon, email with icon)
  - Timestamp ("Posted 2 hours ago")
  - Status badge (Lost/Found with appropriate color)
- White background, subtle shadow on hover
- 16px padding inside cards, 16px gap between cards

### D. Report Forms (Modal or Dedicated Page)
- Clean vertical form layout with clear sections
- Input fields: Full width with 12px padding, border on all sides
- Labels: Above inputs, 14px semibold
- Image upload: Drag-drop zone with preview thumbnail
- Phone input: Pre-filled +91 prefix, numeric validation
- Submit button: Full width on mobile, auto-width on desktop

### E. Contact Information Display
- Phone: Click-to-call link with phone icon
- Email: Click-to-email link with envelope icon
- Display as horizontal pill badges with icon + text
- Use primary blue background with white text

## Color Application
- **Primary #2196F3**: Action buttons, links, primary CTAs
- **Secondary #4CAF50**: "Found" badges, success states
- **Alert #FF9800**: "Lost" badges, important notices
- **Background #FAFAFA**: Page background
- **Text #212121**: All body text and headings
- **Card Background #FFFFFF**: All cards and modals

## Navigation & Interaction
- Filter tabs: "All", "Lost Items", "Found Items" below counters
- Active tab indicated by bottom border in primary blue
- No pagination initially - simple scroll-to-load more
- Minimal animations: subtle hover states on cards (shadow lift)

## Images
**No hero image** - this is a utility platform, not a marketing site.

**Listing Images**:
- Square thumbnails (1:1 aspect ratio) in grid cards
- Placeholder icon/illustration when no image uploaded (grey background with upload icon)
- Full-size image view on card click (modal overlay)

## Mobile Optimization
- Stack all elements to single column below 768px
- Larger touch targets (48px minimum)
- Bottom-fixed action buttons on mobile for easy access
- Collapsible filters/search on mobile

## Key Design Principles
1. **Information Density**: Show maximum listings in viewport without clutter
2. **Scannability**: Clear visual hierarchy, consistent card structure
3. **Speed**: Minimal visual effects, instant feedback
4. **Accessibility**: High contrast text, clear focus states, semantic HTML