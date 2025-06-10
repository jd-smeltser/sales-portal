# Sales Opportunity Portal Builder

## Purpose
This project provides a framework for Claude Code to analyze unstructured sales opportunity data (markdown files) and generate beautiful, shareable microsites using bleeding-edge web technologies.

## How It Works

### For Claude Code Sessions
When given a sales opportunity directory (e.g., `/kernel/sales-opportunities/rimas`), follow this process:

1. **Analyze Directory Structure**
   - Read all `.md` files in the opportunity folder
   - Extract key information: company details, contacts, timeline, technical requirements
   - Identify opportunity status, risks, and next actions

2. **Generate Structured Data**
   - Convert unstructured markdown into JSON following the schema in `sales-opportunity-schema.json`
   - Preserve all important details while organizing them logically
   - Handle missing data gracefully with sensible defaults

3. **Build Microsite**
   - Use the template framework in `index.html` as the base
   - Generate a single-file HTML site with all data embedded
   - Apply the design philosophy: effortless, simple, immediate feedback
   - Use bleeding-edge web APIs: CompressionStream, native CSS, Web Components

## Template Structure

### Core Framework (`index.html`)
- Single HTML file with inline CSS and JavaScript
- Native browser APIs only (no dependencies)
- Progressive disclosure design
- Dark mode support with system preferences
- Mobile-responsive with touch-friendly interactions

### Design System
```css
:root {
  --primary: #8B5CF6;        /* Make.com purple */
  --success: #10B981;        /* Success green */
  --warning: #F59E0B;        /* Warning amber */
  --error: #EF4444;          /* Error red */
  /* Adaptive colors for dark mode */
}
```

### Data Schema (`sales-opportunity-schema.json`)
Standard structure for opportunity data:
- Company information
- Status and health indicators
- Key contacts and stakeholders
- Technical requirements and complexity
- Timeline and milestones
- Risks and mitigation strategies

## Implementation Instructions

### Step 1: Data Extraction
```javascript
// Example of what Claude Code should extract:
const opportunityData = {
  company: {
    name: "Extracted from headers/content",
    location: "From context clues",
    industry: "Inferred from use case"
  },
  status: {
    stage: "Determined from notes",
    health: "Yellow/Red/Green based on content",
    nextAction: "From action items or next steps"
  },
  // ... complete schema
}
```

### Step 2: Site Generation
- Use the base template from `index.html`
- Replace placeholder content with extracted data
- Generate compressed data URL version for sharing
- Create both standalone and shareable versions

### Step 3: Output Format
Generate two files:
1. **`opportunity-site.html`** - Complete standalone microsite
2. **`shareable-url.txt`** - Compressed data URL for sharing

## Key Features to Include

### Visual Elements
- Status indicators with color coding
- Contact cards with click-to-email
- Timeline visualization
- Risk assessment grid
- Technical complexity indicators

### Interactive Features
- Collapsible sections for progressive disclosure
- Search/filter functionality for large datasets
- Print-friendly layouts
- QR code generation for mobile sharing

### Modern Web APIs
- **CompressionStream**: For data URL generation
- **Web Share API**: Native sharing on mobile
- **CSS Custom Properties**: Dynamic theming
- **CSS Container Queries**: Responsive components
- **View Transitions**: Smooth page changes

## Design Philosophy Integration

### The Effortless Principle
- Information hierarchy guides attention naturally
- One-click access to key actions (email contacts, copy links)
- Progressive disclosure keeps interface clean

### Simplicity as Power
- Essential information prominently displayed
- Secondary details available on-demand
- Clear visual relationships between data points

### Immediate Feedback
- Real-time search and filtering
- Visual status indicators
- Instant copy/share confirmations

## Example Usage

```bash
# Claude Code session command:
"Analyze /kernel/sales-opportunities/rimas and generate a microsite using the sales portal framework"
```

### Expected Output:
1. **Analysis Summary**: "Found 8 markdown files containing handover notes, technical docs, and email threads"
2. **Data Extraction**: JSON object with structured opportunity data
3. **Site Generation**: Complete HTML microsite
4. **Deployment Ready**: Single file that works on any web server

## Deployment Options

### GitHub Pages
- Push generated HTML to any GitHub repo
- Enable Pages in settings
- Site live at `username.github.io/repo-name`

### Data URL Sharing
- Compressed version fits in URLs
- Works without hosting
- Perfect for email/Slack sharing

### Local Development
- File works directly in browser
- No build process required
- Instant preview capabilities

## Maintenance

### Updating Design
- Modify CSS custom properties in template
- Changes apply to all generated sites
- Maintain consistency across opportunities

### Adding Features
- Extend the data schema as needed
- Add new UI components to base template
- Keep backward compatibility

### Schema Evolution
- Document any schema changes in git history
- Provide migration guidance for existing sites
- Maintain data integrity

## Success Metrics

### For Users
- Stakeholders can quickly understand opportunity status
- Decision makers get clear next actions
- Technical teams see implementation complexity

### For Claude Code
- Successful extraction of key data points
- Proper categorization of information
- Generation of professional-quality microsites

### For Make.com
- Faster sales cycle through better communication
- Consistent opportunity presentation
- Easy sharing with prospects and partners

## Technical Notes

### Browser Support
- Requires modern browsers (Chrome 88+, Safari 14+, Firefox 85+)
- Graceful degradation for older browsers
- Progressive enhancement approach

### Performance
- Single file loads under 1 second
- Compressed versions under 10KB
- Offline-capable with service workers

### Security
- No external dependencies
- Client-side only processing
- Data never leaves user's device

## Future Enhancements

### Planned Features
- Batch processing for multiple opportunities
- Template variants for different use cases
- Integration with CRM systems
- Analytics dashboard

### Emerging Technologies
- WebAssembly for advanced compression
- Web Components for modularity
- Progressive Web App capabilities
- AI-powered content suggestions

---

*This framework enables Claude Code to transform unstructured sales data into professional, shareable microsites that embody Make.com's design philosophy while leveraging the latest web technologies.*