# AuditIQ — Frequently Asked Questions

---

## **📱 Getting Started**

### **Q: Do I need to install anything?**
**A:** No! AuditIQ is a pure web application. Just open `index.html` in your browser and start using it immediately. No installation, no dependencies, no backend server.

### **Q: Which browsers are supported?**
**A:** 
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

Older browsers may have issues. Make sure your browser is up-to-date.

### **Q: Can I use AuditIQ offline?**
**A:** Yes, 100%! All data is stored locally in your browser. You don't need an internet connection to use it. Data is persisted in LocalStorage automatically.

### **Q: Is my data secure?**
**A:** Absolutely. All assessments stay on your computer in browser memory/storage. Data is never sent to any external server. No tracking, no cookies, no data collection.

---

## **🎯 Usage Questions**

### **Q: How do I create a new engagement?**
**A:** 
1. Click the **"New Engagement"** tab
2. Enter Organization Name and Details
3. Select Compliance Framework (ISO/IEC 27001:2022 or SOC 2)
4. Choose Audit Type (Internal or External)
5. Click **"Create"**

### **Q: What's the difference between the frameworks?**
**A:**

**ISO/IEC 27001:2022**
- 93 controls across 14 domains
- International information security standard
- Broader scope, covers all aspects of security
- Good for general security governance

**SOC 2 Type II**
- Service organization compliance criteria
- Focuses on trust service principles
- Tailored for service providers
- Good for cloud/SaaS companies

Choose the one relevant to your organization's needs.

### **Q: How do I upload evidence?**
**A:**
1. Go to **Assessment** tab
2. Find the control you want to assess
3. Click the **Upload** button
4. Select file (PDF, Word, Excel, text, image)
5. File is automatically saved to that control
6. (Optional) Click **"AI Scan Evidence"** to validate relevance

### **Q: What file types are supported for evidence?**
**A:** 
- PDF documents
- Excel/CSV files
- Word documents (.docx)
- Text files (.txt)
- Images (.jpg, .png, .gif)
- Most other common formats

Size limit: Up to browser's storage capacity (typically 5-50MB per browser).

### **Q: How do I set a control status?**
**A:** 
Click the **Status Dropdown** for each control and select:
- 🟢 **Compliant** — Control is fully implemented
- 🟡 **Partially Compliant** — Control partially implemented, some gaps
- 🔴 **Non-compliant** — Control not implemented
- ⚪ **N/A** — Not applicable to this organization

### **Q: What's the difference between Status and Remarks?**
**A:**
- **Status** — Your assessment result (Compliant/Partial/Non-compliant/N/A)
- **Remarks** — Detailed explanation (findings, evidence, remediation plan)

Example:
- Status: Partially Compliant
- Remarks: "Access logging implemented for prod DB. Development environment lacks logging. Target remediation: Q2 2026."

---

## **🤖 AI Features**

### **Q: How does "AI Suggest" work?**
**A:** The AI button provides context-aware compliance remarks based on:
1. The specific control being assessed
2. The status you selected (Compliant/Partial/Non-compliant)
3. Common best practices for that control

It's **not connected to internet** — all suggestions are generated offline using pre-programmed patterns.

**Example:**
- Control: "Access Control Policy"
- Status: Non-compliant
- AI Suggestion: "Develop and implement a formal access control policy covering privilege levels, approval workflows, and quarterly reviews..."

### **Q: How accurate is "AI Scan Evidence"?**
**A:** 
- Accuracy: **65-95%** depending on evidence quality
- Uses intelligent keyword matching against control requirements
- Provides confidence score (shown as percentage)
- Manual review still recommended

**Better evidence = Higher accuracy**

### **Q: How does the Evidence Scanner work?**
**A:** 
1. Reads uploaded file content
2. Extracts keywords from control description
3. Matches file content against keywords
4. Calculates relevance score
5. Shows verdict: ✅ Relevant | ⚠️ Partially | ❌ Not Relevant

**Tips for better scanning:**
- Upload clear, well-formatted documents
- Include control names/numbers in file names
- Use detailed policy documents
- Avoid scanned images (use OCR first)

### **Q: Can AI Suggest generate false positives?**
**A:** Possibly, but rarely. Remember:
- Suggestions are **recommendations**, not gospel
- Always review and customize suggestions
- Add your own context and details
- Tailor to your organization's specific situation

---

## **📊 Assessment & Reporting**

### **Q: How is the Compliance Score calculated?**
**A:** 
```
Score = (Compliant Controls + Partial Controls × 0.5) / Total Controls × 100
```

**Example:**
- Total: 93 controls
- Compliant: 60
- Partial: 20
- Non-compliant: 13
- **Score = (60 + 20×0.5) / 93 × 100 = 73.1%** 🟡

Partial controls count as 50% because they show progress.

### **Q: What do the dashboard colors mean?**
**A:**
- 🟢 **Green (75-100%)** — Strong compliance posture
- 🟡 **Amber (50-74%)** — Moderate compliance posture
- 🟠 **Orange (25-49%)** — Developing compliance program
- 🔴 **Red (0-24%)** — Early-stage implementation

### **Q: How do I generate a report?**
**A:**
1. Go to **Report** tab
2. Click **"Generate Report"** (takes 1-2 seconds)
3. View report with charts and control details
4. (Optional) Click **"AI Summary"** for executive narrative
5. Click **"Export as PDF"** to download

Report includes:
- Executive summary
- Compliance score
- Control status breakdown
- Detailed findings per control
- Remediation recommendations

### **Q: Can I export my assessment?**
**A:** Yes! Two ways:

**Method 1: PDF Report**
- Go to Report tab
- Click "Export as PDF"
- Save to computer

**Method 2: Data Export** (coming soon)
- Will allow JSON/CSV export
- Can be imported to another browser/device

### **Q: Can I edit a report after generating?**
**A:** No, but you can:
1. Go back to Assessment tab
2. Update control statuses/remarks
3. Re-generate report
4. Export new version

---

## **💾 Data Management**

### **Q: Where is my data stored?**
**A:** 
All data is stored in your browser's **LocalStorage**:
- Persists across browser sessions
- Lost if you clear browser data
- Not synced to cloud
- Specific to that browser/device

### **Q: Can I access data across devices?**
**A:** Not automatically. To access on another device:
1. **Export** assessment from original device
2. **Import** on new device (feature coming soon)
OR use cloud storage to back up browser data

### **Q: What happens if I clear browser data?**
**A:** Your assessments will be **permanently deleted**. To avoid this:
1. Regularly export reports to PDF
2. Use browser backup features
3. Don't clear LocalStorage if you have active assessments

### **Q: How do I backup my assessments?**
**A:**
1. Generate PDF reports regularly
2. Store PDFs on cloud storage (Google Drive, OneDrive, etc.)
3. Keep organized folder structure

**Backup Schedule Recommendation:** Weekly or after each major update

### **Q: Can multiple people work on one assessment?**
**A:** Not yet. Current version is single-user. Coming features:
- Multi-user support
- Team collaboration
- Version history
- Change tracking

---

## **🔧 Technical Questions**

### **Q: Can I modify the application?**
**A:** Yes! The code is available under MIT License. You can:
- Fork on GitHub
- Modify colors, text, layout
- Add new frameworks
- Extend functionality
- Deploy to your own domain

### **Q: How do I add a new compliance framework?**
**A:** 
Technical steps (requires JavaScript knowledge):
1. Define control array (see `ISO_CONTROLS`, `SOC2_CONTROLS` in code)
2. Add framework option in UI
3. Update assessment logic
4. Test thoroughly

See code comments for implementation details.

### **Q: Can I use this commercially?**
**A:** Yes! MIT License allows commercial use. Just:
- Keep the license file
- Acknowledge the original author
- Follow MIT terms

### **Q: Can I self-host this?**
**A:** Absolutely! Since it's single-file HTML:
1. Download `index.html`
2. Host on any web server (GitHub Pages, AWS, your own server)
3. No backend needed
4. Works immediately

### **Q: How large can my assessment be?**
**A:** 
- **Controls:** Unlimited (tested with 500+ controls)
- **Assessments:** Limited by browser storage (typically 5-50MB)
- **File size:** Individual files should be <100MB

### **Q: Is there an API?**
**A:** Not yet, but possible. You can:
- Request feature via GitHub Issues
- Fork and build yourself
- Integrate with your own systems

---

## **🐛 Troubleshooting**

### **Q: The page won't load or is blank**
**A:** 
Try these steps:
1. Hard refresh browser (Ctrl+Shift+R or Cmd+Shift+R)
2. Clear browser cache and reload
3. Try different browser
4. Check browser console (F12) for errors
5. Download fresh copy of `index.html`

### **Q: My assessments disappeared!**
**A:** 
Unfortunately, if you cleared browser data, they're gone. To recover:
1. Check trash/recycle bin for HTML file
2. Use browser history recovery if available
3. Contact support (no promises)

**Prevention:** Regularly export PDFs!

### **Q: Charts aren't displaying**
**A:** 
This happens if Chart.js CDN is blocked. Solutions:
1. Check internet connection
2. Try different browser
3. Disable ad blockers/privacy extensions
4. Check firewall settings

### **Q: Export to PDF is not working**
**A:**
1. Check that pop-ups aren't blocked
2. Try different browser
3. Check file storage permissions
4. Ensure sufficient disk space

### **Q: "AI Suggest" button doesn't do anything**
**A:**
1. Make sure assessment is loaded
2. Try clicking it again
3. Check browser console (F12) for errors
4. Refresh page and try again
5. Try different browser

### **Q: Files won't upload**
**A:**
1. Check file size (should be <100MB)
2. Try different file format
3. Check browser permissions
4. Clear browser cache
5. Disable extensions

---

## **📚 Advanced Usage**

### **Q: Can I print assessments?**
**A:** Yes! 
1. Generate PDF report (recommended)
2. Or use browser Print function (Ctrl+P / Cmd+P)
3. Select "Print to PDF"
4. Save file

### **Q: How do I organize multiple assessments?**
**A:** 
Naming convention suggestion:
```
Client_Name_Framework_Date
Example: "Acme_Corp_ISO27001_2026_Q1"
```

### **Q: Can I compare two assessments?**
**A:** Not built-in, but you can:
1. Open assessment 1, export PDF
2. Open assessment 2, export PDF
3. Compare PDFs manually
4. Or review scores side-by-side

### **Q: How do I track remediation progress?**
**A:**
1. Set initial status (Non-compliant)
2. Add detailed remediation remarks with timeline
3. Update status as work progresses
4. Add evidence of completed remediation
5. Change to Compliant when done
6. Re-generate report to show progress

### **Q: Can I create custom controls?**
**A:** Not in UI yet, but you can:
- Edit HTML source code
- Add custom control to array
- Modify control descriptions
- Rebuild application

Coming in future versions: UI customization

---

## **❓ Other Questions**

### **Q: Is there support or documentation?**
**A:** 
- 📖 [README.md](../README.md) — Project overview
- 📘 [INSTALLATION.md](INSTALLATION.md) — Setup guide
- ⭐ [FEATURES.md](FEATURES.md) — Detailed features
- 🐛 [GitHub Issues](https://github.com/paripatel2907/auditiq/issues) — Report issues
- 📧 Email: paripatel2907@gmail.com

### **Q: How often is AuditIQ updated?**
**A:** 
- Regular improvements as features are added
- Bug fixes as they're reported
- Framework updates as standards evolve
- Watch repository for notifications

### **Q: Can I suggest features?**
**A:** Absolutely! 
- Open GitHub Issue with feature request
- Describe use case
- Explain why it's important
- Suggest implementation approach

### **Q: Is AuditIQ GDPR compliant?**
**A:** 
Yes! Because:
- No data collection
- No external transmission
- All data stored locally
- No tracking/cookies
- User controls all data

### **Q: Can this replace professional auditors?**
**A:** 
Absolutely not. AuditIQ is a **tool to assist**, not replace:
- Professional auditors
- Compliance consultants
- Security teams
- Regulatory experts

Use it for:
- ✅ Self-assessments
- ✅ Readiness checks
- ✅ Internal audits
- ✅ Training

Always involve professionals for:
- ⚠️ Certification audits
- ⚠️ Regulatory compliance
- ⚠️ Critical security decisions
- ⚠️ External assessments

---

## **🎓 Learning Resources**

### **ISO/IEC 27001:2022**
- [ISO.org](https://www.iso.org/isoiec-27001-information-security-management.html)
- [NIST Cyber Framework](https://www.nist.gov/cyberframework)
- [CIS Controls](https://www.cisecurity.org/cis-controls/)

### **SOC 2**
- [AICPA SOC 2](https://www.aicpa.org/interestareas/informationsystems/resources/downloadabledocuments/description-of-the-aicpa-soc-2-reporting-framework)
- [SOC 2 101](https://www.ssae18.com/)

### **GRC & Compliance**
- [GRC Institute](https://www.grc-institute.org/)
- [Audit Practices](https://www.isaca.org/)

---

## **🤝 Contributing**

### **Q: Can I contribute to AuditIQ?**
**A:** Yes! Ways to contribute:
- Report bugs
- Suggest features
- Improve documentation
- Add new frameworks
- Optimize code
- Fix issues

See CONTRIBUTING.md (coming soon)

---

## **Still Have Questions?**

**📧 Email:** paripatel2907@gmail.com  
**🔗 LinkedIn:** https://www.linkedin.com/in/pari-patel-48362b240  
**📞 Phone:** +91 9429516472  

**Response time:** Usually within 24-48 hours

---

**Last Updated:** 2026  
**FAQ Version:** 1.0

