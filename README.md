# Tri-Tender Template

**AI-Powered Tender Response Document Generator**

Tri-Tender is a framework for creating comprehensive, professional tender response documents using AI assistance. It produces custom long-form documents (5+ pages minimum for core sections) through a structured, human-in-the-loop workflow.

---

## 🎯 What Tri-Tender Does

- **Analyses tender documents** to extract all requirements, evaluation criteria, and compliance needs
- **Builds company profiles** from your uploaded documents
- **Creates comprehensive tender responses** with substantial, tailored content
- **Produces preview-ready HTML documents** that can be easily converted to PDF
- **Guides you through a structured workflow** with checkpoints for your approval

---

## 📁 Folder Structure

```
tri-tender-template/
├── tender_planner_prompt.ts    # AI system prompt (the brain)
├── README.md                   # This file
│
├── tender-config/              # Configuration & branding
│   ├── tender_profile.json     # Your company details
│   ├── brand_profile.json      # Brand voice & visual identity
│   ├── sectors.json            # Industry sectors you operate in
│   ├── style_guide.md          # Writing style guidelines
│   ├── brand.css               # Visual styling for documents
│   └── README.md               # Config folder guide
│
├── tender-input/               # YOUR UPLOADS GO HERE
│   ├── README.md               # Upload instructions
│   └── (your tender & company docs)
│
└── tender-output/              # GENERATED DOCUMENTS APPEAR HERE
    ├── README.md               # Output folder guide
    └── (AI-generated HTML documents)
```

---

## 🚀 Getting Started

### Step 1: Prepare Your Documents

Gather the following documents:

**Tender Documents (Required):**
- RFP/RFQ/ToR document
- Specifications or scope of work
- Pricing schedules or BOQ templates
- Any addenda or clarifications

**Company Documents (Required):**
- Company profile
- Registration certificates
- Tax clearance
- B-BBEE certificate (if applicable)
- Key personnel CVs
- Past project references

### Step 2: Upload to tender-input/

Place all your documents in the `tender-input/` folder.

### Step 3: Start the AI Workflow

The AI will guide you through:

1. **Document Analysis** – Extracting tender requirements
2. **Profile Building** – Understanding your company
3. **Strategy Planning** – Aligning your response approach
4. **Document Creation** – Building each section
5. **Review & Refinement** – Polishing the final output

### Step 4: Review Generated Documents

Find your tender response documents in `tender-output/`. Each document is:
- **HTML format** for easy preview
- **Print-ready** with proper styling
- **Previewable** directly in your file browser

---

## 📄 Documents Generated

The AI creates these documents in `tender-output/`:

| File | Description | Min. Length |
|------|-------------|-------------|
| `01_cover_letter.html` | Executive cover letter | 2-3 pages |
| `02_company_profile.html` | Comprehensive company overview | 5-10 pages |
| `03_methodology_and_scope.html` | Detailed approach & methodology | 8-15 pages |
| `04_pricing_schedule.html` | Pricing and cost breakdown | 3-5 pages |
| `05_compliance_checklist.html` | Requirement-by-requirement compliance | Complete |
| `99_appendices.html` | Supporting documents index | As needed |

---

## 🔄 Human-in-the-Loop Workflow

Tri-Tender follows a **checkpoint-based workflow**. The AI will stop and consult you at each phase:

```
📥 Phase 1: Document Intake
   └── ⏸️ Checkpoint: Confirm documents received

📋 Phase 2: Requirements Extraction  
   └── ⏸️ Checkpoint: Validate extracted requirements

🏢 Phase 3: Company Profile
   └── ⏸️ Checkpoint: Approve company summary

📊 Phase 4: Response Strategy
   └── ⏸️ Checkpoint: Agree on approach

📝 Phase 5: Document Creation (per section)
   └── ⏸️ Checkpoint: Review each section

✅ Phase 6: Final Assembly
   └── ⏸️ Checkpoint: Approve complete package
```

**The AI will NOT proceed to the next phase without your explicit approval.**

---

## 🎨 Customising Your Brand

### Brand Configuration

Edit files in `tender-config/` to customise:

**`brand_profile.json`** – Your brand voice and identity:
```json
{
  "brandName": "Your Company",
  "primaryColor": "#1a365d",
  "tone": "professional",
  "values": ["innovation", "reliability"]
}
```

**`brand.css`** – Visual styling:
```css
:root {
  --primary-color: #1a365d;
  --accent-color: #3182ce;
}
```

**`style_guide.md`** – Writing conventions and terminology

---

## 📋 Key Principles

### Custom Content, Not Templates

The AI creates **fresh, tailored content** for each tender. It does NOT:
- Edit pre-existing templates
- Use generic boilerplate
- Copy from previous responses

### Substantial Documents

Core sections are **5+ pages minimum**. The AI will never artificially truncate content to meet arbitrary limits.

### Evidence-Based Claims

All claims in the tender response must be:
- Supported by your uploaded documents
- Verifiable and accurate
- Marked as placeholders if information is missing

### Compliance First

The AI will:
- Address EVERY tender requirement
- Follow prescribed formats exactly
- Flag any deviations for your approval

---

## 🔧 Technical Notes

### Document Format

Generated documents are **HTML files** that:
- Preview in any web browser
- Include print-friendly styling
- Can be exported to PDF via browser print
- Reference `brand.css` for consistent styling

### Previewing Documents

All generated documents can be previewed:
- **In browser:** Open any `.html` file directly
- **In VS Code:** Use Live Preview extension
- **Export to PDF:** Print → Save as PDF

### File Naming Convention

```
XX_section_name.html

01 = Cover Letter
02 = Company Profile
03 = Methodology
04 = Pricing
05 = Compliance
99 = Appendices
```

---

## ⚠️ Important Notes

1. **Never edit files in `tender-output/` manually** – The AI will overwrite them
2. **Keep original documents** in `tender-input/` for reference
3. **Review all AI-generated content** before submission
4. **Verify legal/compliance claims** with appropriate professionals

---

## 📞 Workflow Commands

During the AI session, you can say:

- **"Let's start"** – Begin the tender response workflow
- **"Show me the requirements"** – Review extracted requirements
- **"Proceed to next phase"** – Move forward (after checkpoint)
- **"Make changes to [section]"** – Request revisions
- **"Show me what's complete"** – Get status overview
- **"Create the [section name]"** – Jump to specific section

---

## 📝 License

This template is provided for creating tender response documents. Customise freely for your organisation's needs.

---

**Ready to create a winning tender response? Upload your documents and let's begin!**
