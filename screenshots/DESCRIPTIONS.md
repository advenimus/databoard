# Screenshot Guide for DataBoard

This document describes what each screenshot should capture to effectively showcase DataBoard's features in the README.

## Required Screenshots

### 1. `icon.png`
**Location in README:** Top of page (header)

**What to capture:**
- Copy the app icon from `/Users/chris/Github/databoard/assets/icon.png`
- No screenshot needed - just copy the existing icon file

**Purpose:** Brand identity and visual header

---

### 2. `dashboard-view.png`
**Location in README:** Main features section, first screenshot

**What to capture:**
- Main dashboard view with multiple tiles arranged in a grid
- Should show variety of tile types (at least 3-4 tiles):
  - One line chart (showing time series data)
  - One bar chart
  - One KPI tile (large number)
  - One data table
- Tiles should contain actual data (not empty)
- Show the sidebar navigation on the left
- Clean, uncluttered layout

**Camera positioning:**
- Full window capture
- Window should be reasonably sized (not maximized, not tiny)
- Capture entire dashboard grid area

**Purpose:** First impression - shows the core value proposition

---

### 3. `visualizations.png`
**Location in README:** Rich Visualizations feature section

**What to capture:**
- Dashboard with focus on different visualization types
- Should prominently feature:
  - Line chart with multiple series/colors
  - Bar chart with grouped data
  - Pie chart with labels
  - KPI tile with large formatted number
  - Data table with several rows
- Optional: Status indicator or gauge if implemented

**Camera positioning:**
- Full window or cropped to show just the tile area
- Make sure chart colors and labels are visible

**Purpose:** Demonstrates the variety and quality of visualizations

---

### 4. `connection-management.png`
**Location in README:** Screenshots section - Connection Management

**What to capture:**
- Connections page showing the list of database connections
- Should show at least 2-3 example connections:
  - Different database types (SQL Server, MySQL, PostgreSQL)
  - Mix of connected/disconnected states (if visible)
- "New Connection" button should be visible
- Connection cards/rows should show:
  - Database icon/type
  - Connection name
  - Host/server information
  - Action buttons (edit, delete, test)

**Camera positioning:**
- Full window capture showing the connections list
- Sidebar navigation visible on left

**Purpose:** Shows how users manage their database connections

---

### 5. `tile-editor.png`
**Location in README:** Screenshots section - Tile Editor

**What to capture:**
- The tile creation/editing dialog or page
- Should show:
  - SQL query editor with syntax highlighting
  - Sample SQL query (SELECT statement with some formatting)
  - Tile configuration options:
    - Tile name field
    - Visualization type selector
    - Connection dropdown
    - Refresh interval setting (if visible)
  - Preview of the visualization (if applicable)
  - Save/Cancel buttons

**Camera positioning:**
- Capture the full dialog/modal or editor view
- Query editor should be prominent
- Make sure query text is readable

**Purpose:** Demonstrates how users create tiles with custom queries

---

### 6. `settings.png` (Optional)
**Location in README:** Screenshots section - Settings

**What to capture:**
- Settings page showing available configuration options
- Should show:
  - Database path configuration
  - Theme settings (if implemented)
  - Any other customization options
  - Clear labels and descriptions

**Camera positioning:**
- Full window capture of settings page
- Sidebar visible on left

**Purpose:** Shows customization capabilities

---

## Screenshot Best Practices

### General Guidelines
1. **Window Size**: Use a consistent window size for all screenshots (recommend ~1400x900 pixels)
2. **Clean Data**: Use realistic but clean sample data (no sensitive information)
3. **Professional Appearance**:
   - No distracting desktop background visible
   - Close unnecessary apps/notifications
   - Use real database names and queries that make sense
4. **Lighting/Theme**: Use consistent theme (light or dark) across all screenshots
5. **Resolution**: High DPI/Retina screenshots preferred (will be displayed at smaller size in README)

### Data Recommendations
Create sample connections and data that show:
- **Sales Dashboard** - Monthly revenue, top products, sales trends
- **Analytics Dashboard** - User metrics, page views, conversion rates
- **System Monitoring** - Server stats, response times, error rates

This makes the screenshots immediately relatable to potential users.

### File Format
- **Format**: PNG (preferred) or JPG
- **Compression**: Optimize for web (use tools like ImageOptim, TinyPNG)
- **Max file size**: Keep under 500KB per image if possible

### Naming Convention
Use exactly these filenames (already referenced in README.md):
- `icon.png`
- `dashboard-view.png`
- `visualizations.png`
- `connection-management.png`
- `tile-editor.png`
- `settings.png` (optional)

---

## Screenshot Checklist

Before finalizing screenshots:
- [ ] Copy `icon.png` from assets folder
- [ ] Capture `dashboard-view.png` with multiple tile types
- [ ] Capture `visualizations.png` showing chart variety
- [ ] Capture `connection-management.png` with sample connections
- [ ] Capture `tile-editor.png` showing query editor
- [ ] Capture `settings.png` (optional)
- [ ] All images are PNG format
- [ ] All images are optimized/compressed
- [ ] All filenames match exactly
- [ ] Reviewed for sensitive information
- [ ] Images look good at both full and reduced sizes

---

## Quick Start Commands

After capturing screenshots:

```bash
# Copy app icon
cp /Users/chris/Github/databoard/assets/icon.png /Users/chris/Github/databoard-public/screenshots/icon.png

# Optimize all screenshots (if you have ImageOptim CLI)
find screenshots -name "*.png" -exec imageoptim {} \;

# Check file sizes
ls -lh screenshots/

# Commit to public repo
cd /Users/chris/Github/databoard-public
git add screenshots/
git commit -m "Add application screenshots"
git push origin main
```
