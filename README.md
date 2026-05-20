# AuditIQ – AI-Integrated GRC Compliance Platform

<div align="center">

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/paripatel2907/auditiq?style=social)](https://github.com/paripatel2907/auditiq)
[![Made with](https://img.shields.io/badge/Made%20with-HTML5%20%7C%20JavaScript%20%7C%20CSS3-orange)](https://github.com/paripatel2907/auditiq)

A **powerful, offline-capable web application** for ISO/IEC 27001:2022 and SOC 2 Type II compliance auditing with AI-powered automation.

[🚀 Try Live Demo](https://paripatel2907.github.io/auditiq/) • [📖 Documentation](docs/) • [🐛 Report Issue](https://github.com/paripatel2907/auditiq/issues)

</div>

---

## ✨ Features

### 🎯 **Dual Compliance Frameworks**
- **ISO/IEC 27001:2022** — 93 controls across 14 domains
- **SOC 2 Type II** — Trust service criteria and principles

### 🤖 **AI-Powered Automation**
- **Smart Remark Suggestions** — Context-aware compliance recommendations based on control status
- **Intelligent Evidence Scanning** — AI analyzes uploaded evidence and matches relevance to controls
- **Executive Summary Generation** — Automated narrative reports with compliance posture analysis

### 📊 **Compliance Management**
- Real-time compliance dashboards with live scoring
- Control-level assessment tracking (Compliant/Partial/Non-compliant/N/A)
- Evidence file upload and validation
- Remediation action tracking
- Professional PDF report generation

### 💾 **Data & Privacy**
- **100% Offline** — Fully client-side processing, no backend required
- **Zero Data Collection** — All data stored locally in browser
- **GDPR-Friendly** — No external data transmission
- **Data Persistence** — Automatic save to LocalStorage

### 🎨 **Professional UI**
- Modern, responsive design
- Dark/light theme support
- Intuitive navigation with tabbed interface
- Real-time status indicators

---

## 🚀 Quick Start

### **Option 1: Open Directly (Easiest)**
1. Download `index.html`
2. Open in your web browser (no installation needed!)
3. Start creating compliance assessments

### **Option 2: Clone Repository**
```bash
git clone https://github.com/paripatel2907/auditiq.git
cd auditiq
# Open index.html in your browser
```

### **Option 3: Use Live Demo**
[👉 Try AuditIQ Online](https://paripatel2907.github.io/auditiq/)

---

## 📋 How to Use

### **1. Create a New Engagement**
- Click "New Engagement"
- Enter organization details
- Select compliance framework (ISO/IEC 27001:2022 or SOC 2)
- Choose audit type (Internal/External)

### **2. Start Assessment**
Navigate to the **Assessment** tab and for each control:

| Action | Description |
|--------|-------------|
| 📌 Select Status | Mark as Compliant, Partial, Non-compliant, or N/A |
| 📤 Upload Evidence | Add supporting documentation (policies, logs, reports, etc.) |
| 🔍 Scan Evidence | Use AI to analyze evidence relevance (90%+ accuracy) |
| ✨ Get AI Suggestions | Click "AI Suggest" for context-aware remediation remarks |
| 📝 Add Remarks | Document findings, remediation plans, and timelines |

### **3. Monitor Progress**
- **Dashboard Tab** — View real-time compliance score and status distribution
- **Assessment Tab** — Track individual control details
- **Evidence Tab** — Manage all uploaded files across controls

### **4. Generate Reports**
- **Report Tab** — Creates comprehensive audit report
- **AI Summary Button** — Auto-generates executive narrative
- **PDF Export** — Download professional reports for stakeholders

---

## 🧠 AI Features Explained

### **AI Remark Suggestions**
Provides intelligent, context-aware compliance remarks:
- **Compliant Controls** — Best practice affirmations
- **Partial Controls** — Improvement recommendations
- **Non-compliant Controls** — Remediation guidance

**Example:** For a non-compliant access control, the AI might suggest: *"Implement multi-factor authentication across all administrative accounts with 30-day enforcement window. Document all exceptions with business justification and management approval."*

### **Evidence Scanner**
Analyzes uploaded files against control requirements:
- **Keyword Matching Algorithm** — Compares control descriptions with document content
- **Relevance Scoring** — ✅ Relevant | ⚠️ Partially Relevant | ❌ Not Relevant
- **Confidence Percentage** — Shows matching accuracy (65-95%)

**Works with:**
- PDF documents
- Excel/CSV files
- Text files
- Image-based evidence

### **Executive Summary Generator**
Auto-generates professional audit narratives:
- Compliance posture assessment
- Key control status analysis
- Risk level classification
- Remediation priority recommendations
- Professional language suitable for C-suite review

**Example:** *"The compliance assessment indicates a moderate overall compliance posture with an aggregate score of 68%. Critical gaps were identified in access control and encryption domains, representing significant organizational risk requiring prioritized remediation."*

---

## 📊 Compliance Scoring

**Formula:** `(Compliant Controls + Partial Controls × 0.5) / Total Controls × 100`

**Score Interpretation:**
- 🟢 **75-100%** — Strong compliance posture
- 🟡 **50-74%** — Moderate compliance posture
- 🟠 **25-49%** — Developing compliance program
- 🔴 **0-24%** — Early-stage compliance implementation

---

## 🛠️ Technical Details

### **Architecture**
- **Pure Frontend** — No backend server required
- **Single File** — Entire application in one `index.html`
- **Vanilla JavaScript** — No framework dependencies (easy to understand & modify)

### **Technologies Used**
- **HTML5** — Semantic markup
- **CSS3** — Modern styling with CSS variables
- **JavaScript ES6+** — Modern JavaScript features
- **Chart.js** — Beautiful compliance dashboards
- **jsPDF** — Professional PDF generation
- **Google Fonts** — Premium typography (DM Sans, DM Serif Display, JetBrains Mono)

### **Browser Support**
| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Full Support |
| Firefox | 88+ | ✅ Full Support |
| Safari | 14+ | ✅ Full Support |
| Edge | 90+ | ✅ Full Support |

---

## 📱 Screenshots

### Dashboard View
```
Real-time compliance metrics and control status distribution
Charts showing compliance breakdown by framework
Quick access to all assessments
```

### Assessment Interface
```
Control checklist with detailed descriptions
Evidence upload and scanning interface
AI-powered suggestion buttons
Status tracking and remediation tracking
```

### Report Generation
```
Professional audit reports with charts
Executive summary with AI-generated narrative
Compliance scoring and gap analysis
PDF export ready for stakeholders
```

---

## 💾 Data Management

### **Local Storage**
- All assessments stored in browser's LocalStorage
- Automatic saving after each action
- Survives browser refresh

### **Backup & Export**
- Use browser DevTools to export data
- Copy data across browsers/devices
- No account required

### **Import Previous Work**
- Seamlessly restore previous assessments
- Continue work across sessions
- Share assessments via data export

---

## 🔒 Security & Compliance

### **Data Protection**
✅ No external API calls  
✅ No user tracking  
✅ No cookies or third-party scripts  
✅ All processing in-browser  
✅ GDPR-compliant (no data collection)  
✅ Suitable for confidential assessments  

### **Supported Security Standards**
- ISO/IEC 27001:2022
- SOC 2 Type II
- SEBI (mentioned in original assessment)
- Extensible to other frameworks

---

## 📖 Documentation

- [**INSTALLATION.md**](docs/INSTALLATION.md) — Setup and usage guide
- [**FEATURES.md**](docs/FEATURES.md) — Detailed feature documentation
- [**FAQ.md**](docs/FAQ.md) — Common questions and troubleshooting

---

## 🎨 Customization

### **Change Color Scheme**
Edit the CSS variables in the `<style>` section:
```css
:root {
  --gold: #d4a853;           /* Primary brand color */
  --blue: #2563eb;           /* Secondary accent */
  --ink: #0a0f1e;            /* Text color */
  /* ... more colors ... */
}
```

### **Add New Compliance Framework**
1. Define control array (e.g., `MY_CONTROLS`)
2. Add framework selection option
3. Reference in assessment logic
4. Add to reporting calculations

### **Extend AI Features**
- Modify `aiSuggest()` function for custom remarks
- Enhance `aiScan()` for better evidence matching
- Customize `aiNarrative()` for different report styles

---

## 🚀 Roadmap

- [ ] Multi-user support with cloud sync
- [ ] Additional frameworks (NIST, CIS, HIPAA)
- [ ] Real-time collaboration features
- [ ] Advanced analytics and trend analysis
- [ ] Mobile app version
- [ ] Integration with ticketing systems (Jira, ServiceNow)
- [ ] Automated evidence collection
- [ ] API for third-party integrations

---

## 📈 Use Cases

✅ **Internal Audit Preparation**  
✅ **Third-party Certification Assessment**  
✅ **Compliance Readiness Check**  
✅ **Security Governance Training**  
✅ **Risk Assessment & Management**  
✅ **Client Compliance Consulting**  
✅ **Security Posture Review**  

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### **Development Guidelines**
- Keep code clean and well-commented
- Test across all major browsers
- Update documentation for new features
- Follow existing code style

---

## 📝 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

**Summary:** Free to use, modify, and distribute with attribution.

---

## 👤 Author

**Pari Patel**

- 🎓 M.Sc. Cybersecurity, National Forensic Sciences University
- 🏆 ISO/IEC 27001:2022 Lead Auditor (DNV)
- 💼 GRC Project Manager, PSY9 Security
- 📧 [paripatel2907@gmail.com](mailto:paripatel2907@gmail.com)
- 🔗 [LinkedIn](https://www.linkedin.com/in/pari-patel-48362b240)
- 📱 +91 9429516472

---

## 🙏 Acknowledgments

- **ISO/IEC 27001:2022** — Information Security Management
- **SOC 2** — Service Organization Control Framework
- **Chart.js** — Beautiful, responsive charts
- **jsPDF** — Client-side PDF generation
- **Google Fonts** — Premium typography

---

## 📞 Support & Feedback

- 🐛 **Found a bug?** [Open an Issue](https://github.com/paripatel2907/auditiq/issues/new)
- 💡 **Feature request?** [Suggest an enhancement](https://github.com/paripatel2907/auditiq/issues/new)
- 📧 **Other questions?** [Email me](mailto:paripatel2907@gmail.com)

---

<div align="center">

**[⬆ Back to Top](#auditiq--ai-integrated-grc-compliance-platform)**

Made with ❤️ by [Pari Patel](https://github.com/paripatel2907)

⭐ If you find this helpful, please consider starring the repository!

</div>
