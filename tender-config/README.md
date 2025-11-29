# Tender Configuration

This folder contains configuration files that define your company profile and brand identity for tender responses.

---

## Files Overview

### `tender_profile.json`
**Your company's factual information**

Contains:
- Company registration details
- Contact information
- Key personnel
- Services and sectors
- Experience and references
- Certifications and insurance

**Usage:** The AI will read this file to populate company information throughout the tender response. You can pre-fill this manually, or the AI will extract information from your uploaded documents.

---

### `brand_profile.json`
**Your brand voice and visual identity**

Contains:
- Brand name and tagline
- Tone and personality
- Writing style preferences
- Visual identity (colours, fonts)
- Key messages and differentiators

**Usage:** Ensures all generated documents match your brand's voice and visual style.

---

### `sectors.json`
**Industry sector definitions**

Contains:
- Pre-defined industry sectors
- Common requirements per sector
- Typical documents needed
- Industry-specific terminology

**Usage:** Helps the AI understand sector-specific requirements and terminology.

---

### `style_guide.md`
**Writing conventions and guidelines**

Contains:
- Tone and formality level
- Preferred terminology
- Formatting conventions
- Key messages to emphasise

**Usage:** The AI generates this based on your company documents, ensuring consistent writing style across all tender sections.

---

### `brand.css`
**Visual styling for HTML documents**

Contains:
- Colour definitions
- Typography settings
- Table and list styles
- Document layout rules

**Usage:** All generated HTML documents link to this stylesheet for consistent visual appearance.

---

## How to Use

### Option 1: Pre-fill manually
Edit the JSON files with your company information before starting the tender workflow.

### Option 2: Let AI extract
Upload your company documents to `tender-input/` and the AI will populate these files automatically.

### Option 3: Hybrid approach
Pre-fill what you know, let the AI complete the rest.

---

## Important Notes

1. **JSON files must be valid JSON** - Use a JSON validator if editing manually
2. **Empty fields are okay** - The AI will handle missing information
3. **brand.css customisation** - Modify CSS variables to match your brand colours
4. **style_guide.md** - Review and approve before document generation

---

## Quick Start

1. Open `tender_profile.json`
2. Fill in at minimum:
   - `companyName`
   - `registrationNumber`
   - `contact` details
   - `authorisedSignatory`
3. Open `brand.css`
4. Update the CSS variables in `:root` to your brand colours
5. You're ready to start!
