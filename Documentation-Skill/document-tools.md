# TNDS Document Generation Tools

## Python Word Document Generator

This module provides functions for creating TNDS-branded Word documents with proper formatting.

```python
from docx import Document
from docx.shared import Inches, Pt, RGBColor
from docx.enum.text import WD_ALIGN_PARAGRAPH, WD_LINE_SPACING
from docx.oxml.ns import qn
from docx.oxml import OxmlElement
import os
from datetime import date

# TNDS Brand Colors
NAVY = RGBColor(26, 58, 92)      # #1a3a5c
TEAL = RGBColor(61, 142, 185)     # #3d8eb9
LIGHT_TEAL = RGBColor(91, 163, 200)  # #5ba3c8
BLACK = RGBColor(0, 0, 0)
DARK_GRAY = RGBColor(64, 64, 64)

def create_tnds_document():
    """
    Create a new Word document with TNDS branding and formatting.
    Returns: Document object ready for content
    """
    doc = Document()
    
    # Set default font and margins
    style = doc.styles['Normal']
    font = style.font
    font.name = 'Arial'
    font.size = Pt(11)
    
    # Set margins (1 inch all sides)
    sections = doc.sections
    for section in sections:
        section.top_margin = Inches(1)
        section.bottom_margin = Inches(1)
        section.left_margin = Inches(1)
        section.right_margin = Inches(1)
    
    return doc

def add_tnds_header(doc, logo_path='/mnt/user-data/uploads/word-doc-tnds-logo.png'):
    """
    Add TNDS logo to document header.
    
    Args:
        doc: Document object
        logo_path: Path to logo image file
    """
    section = doc.sections[0]
    header = section.header
    
    # Add logo to header (centered)
    paragraph = header.paragraphs[0]
    paragraph.alignment = WD_ALIGN_PARAGRAPH.CENTER
    
    if os.path.exists(logo_path):
        run = paragraph.add_run()
        run.add_picture(logo_path, width=Inches(2.5))
    else:
        # Fallback if logo not found
        run = paragraph.add_run('TRUE NORTH DATA STRATEGIES')
        run.font.size = Pt(18)
        run.font.bold = True
        run.font.color.rgb = NAVY

def add_tnds_footer(doc):
    """
    Add TNDS footer with contact information.
    
    Args:
        doc: Document object
    """
    section = doc.sections[0]
    footer = section.footer
    
    # Line 1: Contact info
    p1 = footer.paragraphs[0]
    p1.alignment = WD_ALIGN_PARAGRAPH.CENTER
    run1 = p1.add_run('Jacob Johnston | 719-204-6365 | jacob@truenorthstrategyops.com')
    run1.font.name = 'Arial'
    run1.font.size = Pt(9)
    run1.font.color.rgb = NAVY
    
    # Line 2: Company and location
    p2 = footer.add_paragraph()
    p2.alignment = WD_ALIGN_PARAGRAPH.CENTER
    run2 = p2.add_run('True North Data Strategies • Colorado Springs, CO')
    run2.font.name = 'Arial'
    run2.font.size = Pt(9)
    run2.font.italic = True
    run2.font.color.rgb = NAVY

def add_h1(doc, text):
    """
    Add H1 heading (Title) - Navy, 36pt, Bold
    
    Args:
        doc: Document object
        text: Heading text
    Returns: Paragraph object
    """
    p = doc.add_paragraph()
    p.style = 'Heading 1'
    run = p.add_run(text)
    run.font.name = 'Arial'
    run.font.size = Pt(36)
    run.font.bold = True
    run.font.color.rgb = NAVY
    
    # Add spacing after
    p.paragraph_format.space_after = Pt(12)
    
    return p

def add_h2(doc, text):
    """
    Add H2 heading (Major Section) - Teal, 28pt, Bold
    
    Args:
        doc: Document object
        text: Heading text
    Returns: Paragraph object
    """
    p = doc.add_paragraph()
    p.style = 'Heading 2'
    run = p.add_run(text)
    run.font.name = 'Arial'
    run.font.size = Pt(28)
    run.font.bold = True
    run.font.color.rgb = TEAL
    
    # Add spacing after
    p.paragraph_format.space_after = Pt(10)
    
    return p

def add_h3(doc, text):
    """
    Add H3 heading (Subsection) - Navy, 24pt, Bold
    
    Args:
        doc: Document object
        text: Heading text
    Returns: Paragraph object
    """
    p = doc.add_paragraph()
    p.style = 'Heading 3'
    run = p.add_run(text)
    run.font.name = 'Arial'
    run.font.size = Pt(24)
    run.font.bold = True
    run.font.color.rgb = NAVY
    
    # Add spacing after
    p.paragraph_format.space_after = Pt(8)
    
    return p

def add_h4(doc, text):
    """
    Add H4 heading (Minor Heading) - Navy, 18pt, Bold
    
    Args:
        doc: Document object
        text: Heading text
    Returns: Paragraph object
    """
    p = doc.add_paragraph()
    run = p.add_run(text)
    run.font.name = 'Arial'
    run.font.size = Pt(18)
    run.font.bold = True
    run.font.color.rgb = NAVY
    
    # Add spacing after
    p.paragraph_format.space_after = Pt(6)
    
    return p

def add_subtitle(doc, text):
    """
    Add subtitle text (italicized, teal)
    
    Args:
        doc: Document object
        text: Subtitle text
    Returns: Paragraph object
    """
    p = doc.add_paragraph()
    run = p.add_run(text)
    run.font.name = 'Arial'
    run.font.size = Pt(14)
    run.font.italic = True
    run.font.color.rgb = TEAL
    p.alignment = WD_ALIGN_PARAGRAPH.CENTER
    
    # Add spacing after
    p.paragraph_format.space_after = Pt(20)
    
    return p

def add_body_text(doc, text):
    """
    Add body paragraph - Arial, 11pt
    
    Args:
        doc: Document object
        text: Body text
    Returns: Paragraph object
    """
    p = doc.add_paragraph(text)
    p.style = 'Normal'
    
    # Set line spacing to 1.15
    p.paragraph_format.line_spacing_rule = WD_LINE_SPACING.MULTIPLE
    p.paragraph_format.line_spacing = 1.15
    
    # Add spacing after
    p.paragraph_format.space_after = Pt(10)
    
    return p

def add_bullet_list(doc, items):
    """
    Add bullet list with proper formatting
    
    Args:
        doc: Document object
        items: List of strings for bullet points
    Returns: List of paragraph objects
    """
    paragraphs = []
    
    for item in items:
        p = doc.add_paragraph(item, style='List Bullet')
        p.paragraph_format.space_after = Pt(6)
        paragraphs.append(p)
    
    return paragraphs

def add_numbered_list(doc, items):
    """
    Add numbered list with proper formatting
    
    Args:
        doc: Document object
        items: List of strings for numbered points
    Returns: List of paragraph objects
    """
    paragraphs = []
    
    for item in items:
        p = doc.add_paragraph(item, style='List Number')
        p.paragraph_format.space_after = Pt(6)
        paragraphs.append(p)
    
    return paragraphs

def add_quote(doc, text):
    """
    Add quoted text (italicized, indented)
    
    Args:
        doc: Document object
        text: Quote text
    Returns: Paragraph object
    """
    p = doc.add_paragraph()
    run = p.add_run(text)
    run.font.name = 'Arial'
    run.font.size = Pt(10)
    run.font.italic = True
    run.font.color.rgb = DARK_GRAY
    
    # Indent the quote
    p.paragraph_format.left_indent = Inches(0.5)
    p.paragraph_format.space_after = Pt(10)
    
    return p

def add_callout_box(doc, text):
    """
    Add callout box with light teal background and navy left border
    
    Args:
        doc: Document object
        text: Callout text
    Returns: Paragraph object
    """
    p = doc.add_paragraph(text)
    
    # Add background shading
    shading = OxmlElement('w:shd')
    shading.set(qn('w:fill'), 'E8F4F8')  # Light teal at ~20% opacity
    p._element.get_or_add_pPr().append(shading)
    
    # Add left border
    pBdr = OxmlElement('w:pBdr')
    left = OxmlElement('w:left')
    left.set(qn('w:val'), 'single')
    left.set(qn('w:sz'), '24')  # 4pt
    left.set(qn('w:color'), '1a3a5c')  # Navy
    pBdr.append(left)
    p._element.get_or_add_pPr().append(pBdr)
    
    # Add padding
    p.paragraph_format.left_indent = Inches(0.25)
    p.paragraph_format.right_indent = Inches(0.25)
    p.paragraph_format.space_before = Pt(10)
    p.paragraph_format.space_after = Pt(10)
    
    return p

def add_table(doc, headers, rows):
    """
    Add table with TNDS styling
    
    Args:
        doc: Document object
        headers: List of header strings
        rows: List of lists for table data
    Returns: Table object
    """
    table = doc.add_table(rows=1, cols=len(headers))
    table.style = 'Light Grid Accent 1'
    
    # Add and format header row
    header_cells = table.rows[0].cells
    for i, header in enumerate(headers):
        header_cells[i].text = header
        # Format header
        for paragraph in header_cells[i].paragraphs:
            for run in paragraph.runs:
                run.font.bold = True
                run.font.color.rgb = RGBColor(255, 255, 255)  # White
        # Set header background to teal
        shading = OxmlElement('w:shd')
        shading.set(qn('w:fill'), '3d8eb9')  # Teal
        header_cells[i]._element.get_or_add_tcPr().append(shading)
    
    # Add data rows
    for row_data in rows:
        row_cells = table.add_row().cells
        for i, cell_data in enumerate(row_data):
            row_cells[i].text = str(cell_data)
    
    return table

def add_key_phrase(doc, text):
    """
    Add key phrase with teal color and bold
    
    Args:
        doc: Document object
        text: Key phrase text
    Returns: Paragraph object
    """
    p = doc.add_paragraph()
    run = p.add_run(text)
    run.font.name = 'Arial'
    run.font.size = Pt(12)
    run.font.bold = True
    run.font.color.rgb = TEAL
    
    p.paragraph_format.space_after = Pt(10)
    
    return p

def add_internal_use_marker(doc):
    """
    Add "INTERNAL USE ONLY" marker in red
    
    Args:
        doc: Document object
    Returns: Paragraph object
    """
    p = doc.add_paragraph()
    run = p.add_run('INTERNAL USE ONLY')
    run.font.name = 'Arial'
    run.font.size = Pt(10)
    run.font.bold = True
    run.font.color.rgb = RGBColor(211, 47, 47)  # Red
    p.alignment = WD_ALIGN_PARAGRAPH.CENTER
    
    return p

def save_tnds_document(doc, filename, output_dir='/mnt/user-data/outputs'):
    """
    Save document to outputs directory
    
    Args:
        doc: Document object
        filename: Base filename (without path)
        output_dir: Output directory path
    Returns: Full path to saved file
    """
    # Ensure output directory exists
    os.makedirs(output_dir, exist_ok=True)
    
    # Add .docx extension if not present
    if not filename.endswith('.docx'):
        filename += '.docx'
    
    # Build full path
    filepath = os.path.join(output_dir, filename)
    
    # Save document
    doc.save(filepath)
    
    return filepath

# Template Functions

def create_service_document(service_name, subtitle, content_sections):
    """
    Create a complete client-facing service document
    
    Args:
        service_name: Name of the service (H1)
        subtitle: Service subtitle (italicized, teal)
        content_sections: Dict with keys matching section names
    
    Returns: Document object
    """
    doc = create_tnds_document()
    add_tnds_header(doc)
    add_tnds_footer(doc)
    
    # Title and subtitle
    add_h1(doc, service_name)
    add_subtitle(doc, subtitle)
    
    # What This Engagement Is
    if 'what_this_is' in content_sections:
        add_h2(doc, 'What This Engagement Is')
        for paragraph in content_sections['what_this_is']:
            add_body_text(doc, paragraph)
    
    # Who This Is For
    if 'who_this_is_for' in content_sections:
        add_h2(doc, 'Who This Is For')
        add_bullet_list(doc, content_sections['who_this_is_for'])
    
    # Problems This Removes
    if 'problems_removed' in content_sections:
        add_h2(doc, 'Problems This Removes')
        add_bullet_list(doc, content_sections['problems_removed'])
    
    # What You Get
    if 'what_you_get' in content_sections:
        add_h2(doc, 'What You Get')
        for component, details in content_sections['what_you_get'].items():
            add_h3(doc, component)
            if isinstance(details, list):
                add_bullet_list(doc, details)
            else:
                add_body_text(doc, details)
    
    # Scope & Pricing
    if 'scope_pricing' in content_sections:
        add_h2(doc, 'Scope & Pricing')
        sp = content_sections['scope_pricing']
        
        # Investment
        if 'investment' in sp:
            p = doc.add_paragraph()
            run1 = p.add_run('Investment: ')
            run1.bold = True
            run2 = p.add_run(sp['investment'])
            p.paragraph_format.space_after = Pt(6)
        
        # Timeline
        if 'timeline' in sp:
            p = doc.add_paragraph()
            run1 = p.add_run('Timeline: ')
            run1.bold = True
            run2 = p.add_run(sp['timeline'])
            p.paragraph_format.space_after = Pt(6)
        
        # Payment Terms
        if 'payment_terms' in sp:
            p = doc.add_paragraph()
            run1 = p.add_run('Payment Terms: ')
            run1.bold = True
            run2 = p.add_run(sp['payment_terms'])
            p.paragraph_format.space_after = Pt(12)
        
        # What's Included
        if 'included' in sp:
            add_h3(doc, "What's Included")
            add_bullet_list(doc, sp['included'])
        
        # What's Not Included
        if 'not_included' in sp:
            add_h3(doc, "What's Not Included")
            add_bullet_list(doc, sp['not_included'])
    
    # Prerequisites
    if 'prerequisites' in content_sections:
        add_h2(doc, 'Prerequisites')
        if isinstance(content_sections['prerequisites'], list):
            add_bullet_list(doc, content_sections['prerequisites'])
        else:
            add_body_text(doc, content_sections['prerequisites'])
    
    # What Comes Next
    if 'what_comes_next' in content_sections:
        add_h2(doc, 'What Comes Next')
        if isinstance(content_sections['what_comes_next'], list):
            add_bullet_list(doc, content_sections['what_comes_next'])
        else:
            add_body_text(doc, content_sections['what_comes_next'])
    
    return doc

def create_internal_process_document(process_name, content_sections, internal_use=True):
    """
    Create an internal process document
    
    Args:
        process_name: Name of the process (H1)
        content_sections: Dict with process content
        internal_use: Whether to mark as internal use only
    
    Returns: Document object
    """
    doc = create_tnds_document()
    add_tnds_header(doc)
    add_tnds_footer(doc)
    
    # Title
    add_h1(doc, process_name)
    add_subtitle(doc, 'Internal Reference Document')
    
    if internal_use:
        add_internal_use_marker(doc)
        doc.add_paragraph()  # Spacing
    
    # Purpose
    if 'purpose' in content_sections:
        add_h2(doc, 'Purpose')
        add_body_text(doc, content_sections['purpose'])
    
    # Overview
    if 'overview' in content_sections:
        add_h2(doc, 'Overview')
        for paragraph in content_sections['overview']:
            add_body_text(doc, paragraph)
    
    # The Process
    if 'process_steps' in content_sections:
        add_h2(doc, 'The Process')
        for step_num, step in enumerate(content_sections['process_steps'], 1):
            add_h3(doc, f"Step {step_num}: {step['name']}")
            add_body_text(doc, step['description'])
            if 'substeps' in step:
                add_bullet_list(doc, step['substeps'])
    
    # Decision Points
    if 'decision_points' in content_sections:
        add_h2(doc, 'Decision Points')
        for decision in content_sections['decision_points']:
            add_h3(doc, decision['scenario'])
            p = doc.add_paragraph()
            run1 = p.add_run('Do this: ')
            run1.bold = True
            run2 = p.add_run(decision['action'])
            
            p2 = doc.add_paragraph()
            run3 = p2.add_run('Because: ')
            run3.bold = True
            run4 = p2.add_run(decision['reasoning'])
    
    # Tools & Resources
    if 'tools_resources' in content_sections:
        add_h2(doc, 'Tools & Resources Needed')
        add_bullet_list(doc, content_sections['tools_resources'])
    
    # Common Issues
    if 'common_issues' in content_sections:
        add_h2(doc, 'Common Issues & Solutions')
        for issue in content_sections['common_issues']:
            add_h4(doc, f"Issue: {issue['problem']}")
            p = doc.add_paragraph()
            run1 = p.add_run('Solution: ')
            run1.bold = True
            run2 = p.add_run(issue['solution'])
    
    return doc

def generate_filename(doc_type, name, date_str=None):
    """
    Generate TNDS-standard filename
    
    Args:
        doc_type: Type code (Service, SOP, Process, etc.)
        name: Document name (will be title-cased and spaces removed)
        date_str: Optional date string (defaults to today)
    
    Returns: Filename string
    """
    if date_str is None:
        date_str = date.today().strftime('%Y-%m-%d')
    
    # Clean up name
    clean_name = name.replace(' ', '')
    
    return f"TNDS_{doc_type}_{clean_name}_{date_str}.docx"

# Example Usage
if __name__ == '__main__':
    # Example: Create a service document
    content = {
        'what_this_is': [
            "Command Center Build is a fixed-scope engagement...",
            "We install operational visibility...",
        ],
        'who_this_is_for': [
            "5-20 person operations",
            "Field service or office operations",
            "Owner is overwhelmed",
        ],
        # ... etc
    }
    
    doc = create_service_document(
        "Command Center Build",
        "Operational Visibility for Small Operations",
        content
    )
    
    filepath = save_tnds_document(doc, "example_service_doc")
    print(f"Document saved to: {filepath}")
```

## Markdown Document Generator

```python
from datetime import date
import os

def create_markdown_frontmatter(title, doc_type, author='True North Data Strategies'):
    """
    Create YAML frontmatter for markdown documents
    
    Args:
        title: Document title
        doc_type: Type of document
        author: Author name
    
    Returns: Frontmatter string
    """
    today = date.today().strftime('%Y-%m-%d')
    
    frontmatter = f"""---
title: {title}
author: {author}
date: {today}
type: {doc_type}
---

"""
    return frontmatter

def create_markdown_document(title, doc_type, content):
    """
    Create a markdown document with frontmatter
    
    Args:
        title: Document title
        doc_type: Type (client-facing, internal, sop, diagnostic)
        content: Document content as string
    
    Returns: Complete markdown string
    """
    frontmatter = create_markdown_frontmatter(title, doc_type)
    return frontmatter + content

def save_markdown_document(content, filename, output_dir='/mnt/user-data/outputs'):
    """
    Save markdown document
    
    Args:
        content: Markdown content string
        filename: Base filename (without path)
        output_dir: Output directory
    
    Returns: Full path to saved file
    """
    # Ensure output directory exists
    os.makedirs(output_dir, exist_ok=True)
    
    # Add .md extension if not present
    if not filename.endswith('.md'):
        filename += '.md'
    
    # Build full path
    filepath = os.path.join(output_dir, filename)
    
    # Write file
    with open(filepath, 'w', encoding='utf-8') as f:
        f.write(content)
    
    return filepath
```

---

**END OF TOOLS**
