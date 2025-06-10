# Sales Opportunity Portal

A bleeding-edge framework for transforming unstructured sales opportunity data into beautiful, interactive microsites.

## 🚀 Quick Start

### For Claude Code Sessions
```bash
# Analyze a sales opportunity and generate a microsite
"Analyze /kernel/sales-opportunities/[opportunity-name] and generate a microsite using the sales portal framework"
```

### For Manual Use
1. Create a JSON file following the `sales-opportunity-schema.json` structure
2. Use the `opportunity-template.html` template 
3. Deploy as a single HTML file anywhere
4. Share with stakeholders

## 🎯 What This Creates

**Input**: Unstructured markdown files in a sales opportunity directory  
**Output**: Professional microsite with compressed data URL for sharing

### Example Structure
```
/sales-opportunities/rimas/
├── CLAUDE.md                    # Opportunity overview
├── eugenio-handover/           
│   ├── handover-notes.md       # Handover documentation
│   ├── status.md               # Current status
│   └── technical-landscape.md  # Technical details
└── email-threads.json          # Communication history
```

**Becomes**: A single HTML file with opportunity overview, contacts, timeline, risks, and technical details.

## 🛠 Technology Stack

- **CSS Layers**: Perfect cascade control and maintainability
- **OKLCH Color Space**: Modern color functions with color-mix()
- **Web Components**: Custom elements with full encapsulation
- **View Transitions API**: Smooth navigation between sections
- **Service Worker**: Offline capability and performance optimization
- **Intersection Observer**: Scroll-triggered animations
- **CSS Container Queries**: Responsive components
- **Zero Dependencies**: Pure web standards only

## 📐 Design Philosophy

### The Effortless Principle
- Information hierarchy guides attention naturally
- Progressive disclosure keeps interface clean
- One-click actions for key tasks

### Simplicity as Power
- Essential information prominently displayed
- Clean visual relationships
- Minimal cognitive load

### Immediate Feedback
- Real-time compression stats
- Visual status indicators
- Instant sharing capabilities

## 🔧 How It Works

1. **Data Extraction**: Claude Code analyzes markdown files and extracts structured data into JSON
2. **Template Processing**: Uses Mustache-style templating to populate the HTML template
3. **Modern Web APIs**: Leverages bleeding-edge browser technologies for interactive features
4. **Single File Output**: Self-contained HTML that works anywhere

## 📊 Features

### Opportunity Overview
- Company information and industry
- Current status with health indicators
- Next actions and timeline

### Contact Management
- Key stakeholders with roles
- Click-to-email functionality
- Technical and business contacts

### Technical Assessment
- Complexity indicators
- System requirements
- Integration challenges

### Risk Analysis
- Risk factors with impact levels
- Mitigation strategies
- Success metrics

### Interactive Features
- Collapsible sections with smooth animations
- Progressive disclosure for complex information
- Scroll-triggered animations and effects
- Touch-friendly mobile interactions
- Print-optimized layouts

## 🚀 Deployment Options

### GitHub Pages
```bash
# Push to any GitHub repo
git add opportunity-site.html
git commit -m "Add [company] opportunity microsite"
git push

# Enable Pages in repo settings
# Site live at: username.github.io/repo-name/opportunity-site.html
```

### Data URL Sharing
- Compressed version fits in URLs
- Works without hosting
- Perfect for email/Slack/Teams

### Self-Hosted
- Works on any web server
- No backend required
- Instant deployment

## 🎨 Customization

### Design System
Built with CSS Layers and modern color functions:
```css
@layer design-tokens {
  :root {
    --primary: oklch(0.7 0.15 280);         /* Modern purple */
    --success: oklch(0.65 0.15 150);        /* Success green */
    --warning: oklch(0.7 0.12 80);          /* Warning amber */
    --error: oklch(0.65 0.15 20);           /* Error red */
    --surface: oklch(0.98 0.005 280);       /* Light surface */
  }
}
```

### Data Schema
Extend `sales-opportunity-schema.json` for additional fields while maintaining backward compatibility.

## 📱 Browser Support

- **Cutting-Edge Features**: Chrome 105+, Safari 16+, Firefox 110+
- **Core Functionality**: All modern browsers
- **Graceful Degradation**: Progressive enhancement approach
- **Mobile Optimized**: Touch-friendly responsive design

## 🔒 Privacy & Security

- **Client-side Only**: No data sent to servers
- **No Dependencies**: No third-party code
- **URL Fragments**: Data never hits server logs
- **Local Processing**: Everything happens in the browser

## 🎯 Use Cases

### Sales Teams
- Share opportunities with prospects
- Align stakeholders on requirements
- Track deal progression

### Solutions Engineers
- Technical handoff documentation
- Complexity assessment sharing
- Implementation planning

### Account Executives
- Executive summaries
- Decision maker alignment
- Timeline communication

## 🚧 Roadmap

### Planned Features
- [ ] Batch processing for multiple opportunities
- [ ] Template variants for different industries
- [ ] CRM integration capabilities
- [ ] Analytics dashboard

### Emerging Tech Integration
- [ ] WebAssembly compression
- [ ] Web Components modularity
- [ ] PWA capabilities
- [ ] AI content suggestions

## 📝 License

MIT License - feel free to adapt for your organization's needs.

## 🤝 Contributing

This is a template framework designed to be customized. Fork and adapt for your specific sales process and design requirements.

---

**Built with bleeding-edge web technologies and Make.com's design philosophy**