# AI-Based Smart Document Analyzer

A simple React web app (Phase 2) that:
- Extracts text from an uploaded PDF document (using `pdfjs-dist`)
- **Classifies** the document type (Resume / Invoice / Contract / Report) using keyword-based NLP
- **Extracts key information** based on document type (basic heuristics + regex)
- Generates a short **summary** and **keyword analysis**

Built with **React + Tailwind CSS**.

## Features

- **Document upload & text extraction** (PDF)
- **Auto document classification** (keyword-based)
- **Information extraction** (per doc type)
- **Summarization + keyword analytics**

## How to run

Install:

```bash
npm install
```

Start:

```bash
npm start
```

Test (single run):

```bash
npm test -- --watchAll=false
```

Build:

```bash
npm run build
```

## Project structure (important files)

- `src/App.js`: UI dashboard (upload → results)
- `src/utils/smartDocAnalyzer.js`: classification + extraction + summary + keywords
- `src/index.css`: Tailwind + small animation utilities

## Notes / limitations

- PDF text extraction quality depends on the PDF (some PDFs lose line breaks).
- Classification is keyword-based (simple and explainable).

## Phase 3 (pending)

- Backend API + file storage (full-stack)
- User authentication
- DOCX upload + ML-based classifier (optional upgrade)

