# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **policy proposal and presentation project** for 녹색전환연구소 (Green Transition Institute) focused on improving energy efficiency standards in Korea's heating equipment subsidy program. The project advocates for:

1. Unified energy efficiency testing standards for all electric heating equipment
2. Technology-neutral market competition vs. heat pump-centric subsidies
3. Evidence-based policy through transparent efficiency data disclosure
4. Ion heating system validation as an alternative to heat pumps

**Client**: TVTL Energy Solution / 뉴에너지
**Target Organization**: 녹색전환연구소 (Green Transition Institute)
**Policy Context**: Korea's 2035 National Greenhouse Gas Reduction Target (NDC)

## Repository Structure

```
/
├── data/                    # Source images (JPEG format)
├── output/                  # Generated HTML deliverables
│   ├── meeting-proposal.html    # Main A4 landscape infographic
│   ├── meeting-outline.html     # Meeting outline document
│   ├── proposal-donut.html      # Donut economy framework proposal
│   └── ppt_slide/               # Individual PPT slide pages (HTML)
│       ├── page_1.html          # Title slide (1280x720)
│       ├── page_2.html          # Problem statement
│       └── page_3-9.html        # Content slides
├── 발표보고자료/           # Reference materials (PDFs)
├── 디자인참고자료/         # Design references
├── 미팅목차.txt            # Meeting outline (Korean)
├── 의견제출서.txt          # Official policy submission letter
├── 내용정리1.txt           # Full proposal content (Korean)
└── 난방 기기 보급 사업의 문제점과 개선 방안.pptx  # Source PowerPoint
```

## Document Types & Formats

### HTML Output Specifications

**Meeting Proposal Infographic** (`meeting-proposal.html`):
- Format: A4 landscape (297mm × 210mm)
- Layout: Full-page infographic with gradient backgrounds
- Framework: Chart.js for data visualization
- Print-ready: CSS `@page` rules configured

**PPT Slides** (`ppt_slide/page_*.html`):
- Dimensions: 1280px × 720px (16:9 aspect ratio)
- Framework: Tailwind CSS
- Fonts: Nanum Square (titles), Nanum Gothic (body)
- Icons: Font Awesome 6.0
- Design: Green (#4CAF50) and dark gray (#333333) accent colors
- Purpose: Individual slide exports for web presentation

### Content Structure

**Core Policy Arguments**:
1. Problem: Chinese low-efficiency heat pumps flooding subsidy program
2. Gap: No unified efficiency testing system for electric heating in Korea (vs. Japan APF, US UEF)
3. Solution: K-EEES (Korean Energy Efficiency Evaluation System) proposal
4. Evidence: KCL test data showing 28.1% savings vs. heat pumps
5. Call to Action: Joint R&D project with Green Transition Institute

## Korean Language Context

All content is in **Korean (ko-KR)**:
- Primary audience: Korean policymakers and research institutes
- Technical terminology: Energy efficiency (에너지 효율), heat pump (히트펌프), ion heating (이온히팅)
- Policy framework: Carbon Neutral Framework Act Article 8 (탄소중립 기본법 제8조)
- Date formats: Korean standard (2025년 11월 1일)

## Design System

**Color Palette**:
- Primary: Green (#4CAF50) - sustainability theme
- Secondary: Dark Gray (#333333) - professional tone
- Backgrounds: Gradient combinations (slate to gray to indigo)
- Text: Gray scale (#0f172a to #6b7280)

**Typography**:
- Headings: Nanum Square (bold weights: 700, 800)
- Body: Nanum Gothic (regular: 400, bold: 700)
- Fallbacks: Malgun Gothic, Noto Sans KR, Segoe UI

**Layout Principles**:
- Clean, modern aesthetic with generous whitespace
- Data visualization with charts for impact metrics
- Icon-based section markers (Font Awesome)
- Responsive grid layouts using Tailwind/Flexbox

## Content Sources

**Reference Documents**:
- `내용정리1.txt`: Complete policy proposal narrative (Korean)
- `미팅목차.txt`: 9-section meeting outline structure
- `의견제출서.txt`: Official policy submission template
- `통화 녹음 뉴에너지 김영태 기술이사_251030_214241.txt`: Call transcript with technical director

**Key Data Points**:
- Annual CO2 reduction: 2,304.6 tCO2
- Efficiency advantage: 28.1% savings vs. heat pumps (KCL data)
- Installation case studies: Hyundai, Daesang, Novelis, Lotte World
- Awards: CES 2025 Innovation Award

## Workflow Patterns

**Generating New Slides**:
1. Reference existing `page_*.html` files for structure consistency
2. Maintain 1280×720 dimensions and Tailwind framework
3. Use consistent color scheme (green/dark gray accents)
4. Apply gradient backgrounds (`gradient-bg` class)
5. Include top/bottom accent lines (`accent-line` class)
6. Use Font Awesome icons contextually

**Creating Infographics**:
1. Reference `meeting-proposal.html` for A4 landscape setup
2. Include Chart.js for data visualizations
3. Apply print-ready CSS with `@page` rules
4. Use gradient backgrounds for visual appeal
5. Maintain professional tone with data-driven content

**Content Updates**:
- Always preserve Korean language and technical accuracy
- Maintain consistent terminology across documents
- Reference `내용정리1.txt` for source content
- Verify data points against source materials

## Technical Notes

**HTML Generation**:
- All HTML files are standalone (inline CSS, CDN scripts)
- No build process or dependencies
- Direct browser rendering for presentations
- Print functionality via browser print dialog

**Font Loading**:
- Google Fonts CDN for Nanum family
- Font Awesome CDN for icons (v6.0.0-beta3)
- Tailwind CSS via CDN (latest)
- Chart.js via jsDelivr CDN

**Browser Compatibility**:
- Target: Modern browsers (Chrome, Edge, Firefox)
- Print media queries for A4 output
- Flexbox/Grid for layouts (IE11 not required)

## Context for Future Work

This project supports **policy advocacy for technology-neutral energy efficiency standards** in Korea's heating sector. The core argument is that transparent efficiency testing and data disclosure will naturally drive market selection of high-efficiency technologies, achieving NDC targets faster than subsidy-dependent approaches.

When extending this work:
- Maintain focus on evidence-based arguments (KCL test data, international standards)
- Preserve professional policy proposal tone
- Reference international examples (Japan APF, US UEF, EU ErP)
- Connect to legal framework (Carbon Neutral Framework Act Article 8)
- Emphasize fairness, transparency, and market-based competition
