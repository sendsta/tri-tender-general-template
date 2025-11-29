# Tri-Tender Template

**AI-Powered Tender Response Document Generator**

Tri-Tender creates comprehensive, professional tender response documents that are **structured entirely according to your specific tender's requirements**—not pre-defined templates.

---

## 🎯 Core Principle: Tender-Driven Structure

**Every tender is different. Every response should be different.**

Tri-Tender does NOT use:
- ❌ Pre-defined document templates
- ❌ Standard section structures
- ❌ One-size-fits-all formats

Tri-Tender DOES:
- ✅ Analyse YOUR tender document
- ✅ Extract the EXACT structure required
- ✅ Create documents that match the tender's specifications
- ✅ Ensure compliance with tender-specific formatting

---

## 📋 How It Works

### Step 1: Upload Your Documents
Place your tender and company documents in `tender-input/`

### Step 2: AI Analyses the Tender
The AI reads your tender document and identifies:
- Required documents and sections
- Mandatory forms and annexures
- Evaluation criteria
- Submission format requirements

### Step 3: Structure Discovery
The AI presents a **proposed document structure** based on your tender:

```
Example (Government RFP):
├── Part A: Administrative Documents
│   ├── Completed SBD Forms
│   ├── Tax Clearance Certificate
│   └── B-BBEE Certificate
├── Part B: Technical Proposal
│   ├── Company Profile
│   ├── Methodology
│   └── Team Composition
└── Part C: Financial Proposal
    ├── Pricing Schedule
    └── Payment Terms

Example (Corporate RFQ):
├── Executive Summary
├── Understanding of Requirements
├── Proposed Solution
├── Implementation Approach
├── Project Team
├── Relevant Experience
└── Commercial Proposal
```

**You approve the structure before any documents are created.**

### Step 4: Document Creation
The AI creates each document with comprehensive content, checking in with you after each section.

### Step 5: Final Review
Complete package reviewed against tender requirements.

---

## 📁 Folder Structure

```
tri-tender-template/
├── tender_planner_prompt.ts    # AI system prompt
├── README.md                   # This file
├── index.html                  # Document preview hub
│
├── tender-config/              # Company & brand settings
│   ├── tender_profile.json     # Your company details
│   ├── brand_profile.json      # Brand voice & identity
│   ├── sectors.json            # Industry sectors
│   ├── style_guide.md          # Writing guidelines
│   └── brand.css               # Document styling
│
├── tender-input/               # YOUR UPLOADS GO HERE
│   └── (tender & company docs)
│
└── tender-output/              # GENERATED DOCUMENTS APPEAR HERE
    └── (structured per tender requirements)
```

---

## 🔄 Human-in-the-Loop Workflow

The AI consults you at **7 checkpoints**:

| # | Phase | What Happens |
|---|-------|--------------|
| 1 | Document Intake | Confirm all documents received |
| 2 | Requirements | Validate extracted requirements |
| 3 | **Structure Discovery** | **Approve the proposed document structure** |
| 4 | Company Profile | Approve company information |
| 5 | Strategy | Agree on response approach |
| 6 | Each Document | Review and approve each section |
| 7 | Final Review | Approve complete package |

**The AI will NOT proceed without your approval at each checkpoint.**

---

## 📄 Document Output

### Format
- **Default:** HTML (easy preview, converts to PDF)
- **Alternative:** DOCX, PDF (if tender specifies)

### Naming
Documents are named according to:
1. Tender-specified names (if prescribed)
2. Logical names matching tender structure (if not specified)

### Previewing
- Open any `.html` file in a browser
- Use `index.html` as your document hub
- Export to PDF via browser print function

---

## 🚀 Getting Started

### 1. Gather Your Documents

**Tender Documents:**
- RFP / RFQ / ToR / ITT
- Specifications
- Addenda / Clarifications
- Pricing templates (if provided)

**Company Documents:**
- Company profile
- Registration certificates
- Tax clearance
- B-BBEE certificate
- Key personnel CVs
- Reference letters
- Relevant certifications

### 2. Upload to tender-input/
Place all documents in the `tender-input/` folder.

### 3. Start the AI Workflow
The AI will:
1. Confirm document receipt
2. Analyse tender requirements
3. **Propose a structure based on YOUR tender**
4. Create documents for your review

---

## ⚠️ Important Notes

1. **No Pre-defined Templates**
   The document structure comes from YOUR tender, not from this template.

2. **Review AI Output**
   Always review generated content before submission.

3. **Verify Compliance**
   Double-check all claims against your actual capabilities.

4. **Tool Failures**
   If something fails, the AI will tell you and attempt to fix it—it won't assume success.

---

## 📞 Workflow Commands

During the AI session:

| Say This | To Do This |
|----------|------------|
| "Let's start" | Begin the workflow |
| "Show the requirements" | Review extracted requirements |
| "Show the proposed structure" | See/revise document structure |
| "Proceed" | Move to next phase (after checkpoint) |
| "Make changes to..." | Request revisions |
| "What's the status?" | Get progress overview |

---

## 🎨 Customisation

### Brand Colours
Edit `tender-config/brand.css`:
```css
:root {
    --primary-color: #1a365d;    /* Your brand colour */
    --accent-color: #3182ce;     /* Accent colour */
}
```

### Company Details
Edit `tender-config/tender_profile.json` with your company information, or let the AI extract it from your uploaded documents.

---

**Ready to create a winning tender response? Upload your tender document and let's discover what structure it requires!**
