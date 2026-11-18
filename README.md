# Responsive Layout Technical Specification

##  Live link- https://natalish01.github.io/Css-layout-battle-assignment/

## 1. Desktop View (1440px)

### Grid and Spacing
- **Container/Wrapper:** Maximum width of 1440px with horizontal margins/padding on both left and right sides.
- **Layout Structure:** Flexbox or CSS Grid dividing the main area into a fixed sidebar and flexible main content container.

### Header
- **Height:** 80px (recommended).
- **Layout Elements:** Logo positioned on the left; navigation links (Home, About, Contact) and primary action button (Get Started) positioned on the right using `display: flex; justify-content: space-between; align-items: center;`.

### Sidebar (Navigation)
- **Width:** Exactly 280px.
- **Content:** Section title "Navigation" followed by vertical list items (Dashboard, Projects, Settings, Help) styled with a vertical stack (`display: flex; flex-direction: column; gap: 12px;`).

### Main Content
- **Width:** 1160px.
- **Content Alignment:** Internal text and call-to-action button aligned according to design requirements.

### Footer
- **Height and Content:** Copyright text (`© 2026 MySite. All rights reserved.`) aligned to the left; secondary links (Privacy, Terms, Contact) aligned to the right.

---

## 2. Tablet View (768px)

### Layout Adjustments
- **Container Width:** 768px.
- **Sidebar Width:** Reduced to 200px.
- **Main Content Width:** Adjusted to 568px to fit the remaining width.

### Header Adjustments
- Navigation links (Home, About, Contact) are hidden and replaced with a hamburger menu icon.
- Action button visibility is adapted or collapsed into the mobile navigation drawer.

---

## 3. Mobile View (375px)

### Layout Reorganization (Stacking)
- **Container Width:** 375px.
- **Sidebar Position:** The sidebar moves below the main content container in the Document Object Model (DOM) order, stacking vertically.
- **Content Elements:** Main content takes full available width with responsive padding.

---

## Design Tokens and Global Parameters

### Colors
- **Main Content Background:** Light green tint.
- **Sidebar Background:** Light lavender/purple tint.
- **Primary Action Color:** Solid brand blue for buttons.
- **Footer Background:** Neutral light beige tint.

### Typography
- **Font Family:** System default sans-serif (e.g., Inter, Roboto).
- **Font Sizes:** Responsive scaling applied to headings across different viewports.

### Breakpoints
- **Tablet Breakpoint:** `max-width: 1024px`
- **Mobile Breakpoint:** `max-width: 768px`
