Tri‑Tender General Template

Welcome to the Tri‑Tender General Template, the core framework that powers Tri‑Tender’s AI‑driven tender response generation. This template is designed to transform any tender pack (RFP, RFQ, bid, panel or framework) into a complete, compliant and professionally structured proposal—all while aligning your response with the evaluation criteria and maintaining your brand identity.

🎯 Why Use This Template?

Evaluation‑Aligned Responses: The template mirrors common tender sections and scoring criteria
xait.com
, ensuring you address every point that evaluators look for—so you earn maximum points.

AI‑Guided Content Creation: Paired with our AI‑RULES.md, the template instructs the AI exactly how to extract requirements, map them to your company’s capabilities, and populate each section without hallucinating facts.

Modular & Reusable: With partials for every section and clearly defined placeholders, you can adapt the template to any tender—whether it’s construction, hosted telephony, CCTV or maintenance.

Built‑In Compliance: The structure includes sections for administrative, technical and legal compliance matrices so you never miss a mandatory requirement.

Visual Preview: An optional src directory includes a simple HTML preview page to view your compiled response before final submission.

📁 Folder Structure
tri-tender-general-template/
│
├── AI-RULES.md                # Detailed rules that govern how the AI builds your response
├── template.html              # Main HTML skeleton combining all sections
├── partials/                  # Modular HTML snippets for each section
│   ├── 00-metadata.json       # Placeholder schema for tender & company info
│   ├── 01-cover-letter.html
│   ├── 02-executive-summary.html
│   ├── ...                    # More partials up to 14-checklists...
│   └── 14-checklists-&-submission-instructions.html
│
├── tender-input/              # Place your raw tender documents here (PDF, DOCX, Excel)
│   └── README.md              # Explains what goes into this folder
│
├── tender-output/             # Generated responses (HTML/PDF/DOCX) will be saved here
│   └── README.md              # Explains how outputs are handled
│
└── src/                       # Optional UI for previewing the compiled tender response
    ├── index.html             # Loads your final-response.html for quick viewing
    └── README.md              # Instructions for using or extending the preview

🧠 How the Template Works

Prepare Your Inputs:

Drop all relevant tender documents (RFP PDFs, Excel pricing schedules, Word annexures) into tender-input/.

Ensure your company profile (registration, VAT number, PSIRA/CIDB certificates, B‑BBEE certificate) is available—these will populate company.* placeholders.

AI Extraction & Planning:

When Tri‑Tender runs, it first reads the AI-RULES.md file. This document instructs the AI to:

Extract tender metadata (title, number, issuer, closing date, evaluation criteria, etc.).

Identify all mandatory requirements and evaluation criteria
xait.com
.

Plan which section of the template each requirement belongs to.

Avoid hallucinating facts by using placeholders where information is missing.

Section Assembly:

The AI writes each part of your proposal using the HTML snippets in partials/.

For example, 05-technical-solution.html guides the AI to describe your proposed solution, equipment specs, methodology and compliance with technical requirements.

Placeholders (e.g. {{tender.number}}, {{company.reg_no}}) are replaced with real values from your tender and company documents.

Output Generation:

All completed sections are combined into template.html to form a single, polished tender response.

The finished document is saved in tender-output/ (e.g. final-response.html). From there you can convert it to PDF or DOCX.

Preview (Optional):

Open src/index.html in a browser to preview your response. It automatically loads tender-output/final-response.html so you can check formatting, correctness and completeness before submission.

You can extend the src folder with a full React/Next.js app for more advanced editing or collaboration.

✅ Tips for Success

Follow the Tender Structure: Keep headings consistent with the tender document and do not add or skip sections unless specifically allowed.

Complete the Compliance Matrix: This is where you prove you meet administrative (CSD, tax, BBBEE), technical (equipment specs, standards) and legal (forms, declarations) requirements.

Leverage Placeholders: If information is missing or to be provided later (e.g. pricing details), leave the placeholder in place ({{INSERT_PRICING_FROM_OFFICIAL_BOQ}}). Tri‑Tender will prompt you to fill it manually before final submission.

Customise Branding: Add your own colours, fonts and logos by editing the CSS in the generated HTML or extending the src folder.

🌟 Why Tri‑Tender Is the Best

Tri‑Tender isn’t just a template—it’s a methodology. By combining structured documents with AI rules, Tri‑Tender ensures:

Consistency: Every tender response follows a high‑quality, evaluator‑friendly format.

Compliance: Built‑in checks help you avoid non‑compliance that could disqualify your bid.

Efficiency: Generate a first draft in minutes, not days, freeing your team to refine the message instead of re‑creating boilerplate.

Accuracy: The AI rulebook prevents hallucinations and ensures factual correctness. It leaves placeholders for anything missing rather than inventing data.

Scalability: Whether responding to one tender or dozens, the template scales effortlessly; you just swap out the input files and regenerate.
