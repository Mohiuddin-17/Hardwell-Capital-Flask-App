# Hardwell-Capital-Flask-App
An AI based Flask App that automates the system of creating Financial Reports for Real Estate Agents 

# Hardwell Capital Flask Application

An AI-powered document automation platform built for **Hardwell Capital**, a real estate company based in Chicago, USA. The application eliminates manual report generation by automatically extracting, processing, and analyzing data from Rent Roll and T-12 financial documents — regardless of their format — and producing structured reports that follow the client's exact template guidelines.

---

## The Problem It Solves

Hardwell Capital regularly receives two critical financial documents from their users:

- **Rent Roll** — A detailed record of all tenants, lease terms, and rental income
- **T-12 (Trailing Twelve Months)** — A 12-month income and expense summary of a property

Previously, their team had to manually read through these documents and build reports by hand every time they needed to present information to a user. This application fully automates that entire workflow.

---

## How It Works

1. **Upload** — The client submits their Rent Roll and T-12 documents through the application
2. **Extraction** — The application uses OCR and text extraction techniques to read and parse the documents regardless of their format
3. **Processing** — The extracted data is analyzed and structured by the AI layer
4. **Report Generation** — A complete, formatted report is automatically generated following Hardwell Capital's exact template guidelines
5. **Output** — The final report is ready for immediate use with their users

---

## Key Features

- Multi-format document support — accepts CSV, XLSX, PDF, and Word documents
- OCR integration for scanned and image-based documents
- Automated report generation following client-defined templates
- Handles both Rent Roll and T-12 document types in a single submission
- Eliminates manual data entry and report building entirely

---

## Tech Stack

| Layer | Technology |
|---|---|
| Backend Framework | Python Flask |
| Document Processing | OCR, Text Extraction |
| File Format Support | CSV, XLSX, PDF, DOCX |
| AI & Analysis | OpenAI API |
| Report Generation | Template-based automated output |

---

## Project Structure

hardwell-capital-flask-app/
├── app.py                  # Main Flask application entry point
├── requirements.txt        # Python dependencies
├── .env                    # Environment variables (not included in repo)
├── .gitignore
├── README.md
├── templates/              # Report template definitions
├── uploads/                # Temporary document upload handling
├── processors/             # Document parsing and OCR logic
└── reports/                # Generated report output handlers

## Prerequisites

- Python 3.10+
- pip
- OpenAI API Key

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Mohiuddin-17/hardwell-capital-flask-app.git
cd hardwell-capital-flask-app
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables

Create a `.env` file in the root folder:
OPENAI_API_KEY=your_openai_api_key

### 5. Run the Application

```bash
python app.py
```

The application will be available at `http://localhost:5000`

---

## Supported Document Formats

| Document Type | Supported Formats |
|---|---|
| Rent Roll | CSV, XLSX, PDF, DOCX |
| T-12 | CSV, XLSX, PDF, DOCX |

---

## License

This project was developed exclusively for Hardwell Capital, Chicago, USA. All rights reserved.
