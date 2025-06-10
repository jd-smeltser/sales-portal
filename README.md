# Sales Opportunity Portal

A bleeding-edge framework for transforming unstructured sales opportunity data into beautiful, shareable microsites.

## 🚀 Quick Start

### For Claude Code Sessions
```bash
# Analyze a sales opportunity and generate a microsite
"Analyze /kernel/sales-opportunities/[opportunity-name] and generate a microsite using the sales portal framework"
```

### For Manual Use
1. Visit the [live portal](https://jd-smeltser.github.io/sales-portal/)
2. Upload your opportunity JSON data
3. Generate a compressed data URL
4. Share the URL with stakeholders

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

- **Zero Dependencies**: Pure web standards only
- **CompressionStream API**: Native browser compression
- **Modern CSS**: Custom properties, container queries
- **Progressive Enhancement**: Works everywhere, enhanced in modern browsers
- **Single File Output**: Easy deployment anywhere

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

1. **Data Extraction**: Claude Code analyzes markdown files and extracts structured data
2. **Site Generation**: Creates a beautiful HTML microsite using the template framework
3. **Compression**: Generates a shareable data URL version
4. **Deployment**: Single file works on any web server or as a data URL

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
Modify CSS custom properties in the template:
```css
:root {
  --primary: #8B5CF6;    /* Make.com purple */
  --success: #10B981;    /* Success indicators */
  --warning: #F59E0B;    /* Attention items */
  --error: #EF4444;      /* Risk factors */
}
```

### Data Schema
Extend `sales-opportunity-schema.json` for additional fields while maintaining backward compatibility.

## 📱 Browser Support

- **Modern Browsers**: Full feature set (Chrome 88+, Safari 14+, Firefox 85+)
- **Legacy Browsers**: Graceful degradation with core functionality
- **Mobile**: Touch-friendly responsive design

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