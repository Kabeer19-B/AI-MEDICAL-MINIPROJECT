# AI-Assisted Clinical Documentation and Coding Support System

## Project Overview

The **AI-Assisted Clinical Documentation and Coding Support System** is an AI-powered healthcare solution designed to reduce the manual workload of doctors during patient consultations.

The system captures doctor-patient conversations, converts speech into text using OpenAI Whisper Large-v3, processes the transcript using Natural Language Processing (NLP) and Large Language Models (LLMs), and generates structured clinical notes (SOAP) along with relevant ICD-10 diagnostic code suggestions.

Doctors can review, edit, approve, or reject AI-generated results before saving them to the Electronic Health Record (EHR).

## Problem Statement

Doctors spend significant time documenting patient consultations and assigning standardized diagnostic codes manually. This increases administrative workload, reduces patient interaction time, and may lead to incomplete or inconsistent clinical records.

This project aims to automate clinical documentation and support medical coding using AI technologies.

## Key Features

- **Speech Recognition:** Converts doctor-patient audio conversations into text using Whisper Large-v3.
- **Medical Entity Extraction:** Identifies symptoms, medical findings, and diagnoses from transcripts.
- **SOAP Note Generation:** Automatically generates structured clinical documentation.
- **ICD-10 Code Recommendation:** Suggests relevant diagnostic codes based on extracted medical information.
- **Confidence Scores:** Provides confidence values for suggested diagnostic codes.
- **Clinician Review:** Allows doctors to edit, approve, or reject AI-generated outputs.
- **Secure Storage:** Stores approved clinical notes and coding information.

## System Workflow

1. Capture doctor-patient consultation audio.
2. Convert audio into text using Whisper Large-v3.
3. Process the transcript using NLP and an LLM.
4. Extract relevant medical entities.
5. Generate structured SOAP notes.
6. Recommend relevant ICD-10 diagnostic codes.
7. Display results for clinician review.
8. Allow editing, approval, or rejection.
9. Save approved information to the Electronic Health Record.

**Workflow:**

`Audio Input → Speech-to-Text → NLP/LLM Processing → SOAP Notes + ICD-10 Suggestions → Doctor Approval → EHR Storage`

## Technology Stack

| Component | Technology |
|---|---|
| Frontend | React.js, Tailwind CSS |
| Backend | FastAPI (Python) |
| Speech Recognition | OpenAI Whisper Large-v3 |
| AI Processing | NLP and Large Language Models |
| Database | Supabase |
| Authentication | Supabase Auth |
| Deployment | Docker |
| Version Control | GitHub |

## SOAP Documentation

The system generates clinical notes using the SOAP format:

- **S – Subjective:** Patient's symptoms and complaints.
- **O – Objective:** Observations and clinical findings.
- **A – Assessment:** Clinical assessment and possible diagnosis.
- **P – Plan:** Recommended treatment or next steps.

## ICD-10 Coding Support

The system analyses extracted medical information from consultation transcripts and recommends relevant ICD-10 diagnostic codes.

The suggested codes are displayed with confidence values for clinician review. Final code selection requires clinical verification.

## System Architecture

The project consists of the following major components:

1. Consultation Input
2. Speech Recognition
3. NLP / LLM Processing
4. Clinical Note Generation
5. ICD-10 Coding Support
6. Clinician Review
7. Electronic Health Record Storage

## Installation and Setup

### Prerequisites

- Python
- Node.js and npm
- Git
- Supabase account
- Required AI model/API access

### Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd YOUR_PROJECT_FOLDER
```

### Backend Setup

```bash
cd backend
pip install -r requirements.txt
```

Configure the required environment variables in your `.env` file according to your project configuration.

Start the backend using:

```bash
uvicorn main:app --reload
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

*Note: Update the folder names, entry-point files, environment variables, and commands according to your actual repository structure.*

## Future Enhancements

- Multilingual medical speech recognition.
- Improved medical terminology extraction.
- Integration with standardized EHR systems.
- Enhanced ICD-10 code matching.
- Advanced patient data security and audit tracking.

## Project Objective

To improve healthcare documentation efficiency by combining speech recognition, artificial intelligence, and automated medical coding while ensuring that clinicians maintain control over final medical decisions.

## Contributors

**Batch Number:** CBC_09

- Kabeer Baig
- Suchetanaradhya C
- Arinjay Kailash Jai
- Kishore Kumar S

**Institution:** Presidency University

**Department:** School of Artificial Intelligence and Advanced Computing

## Supervisor

Dr. Sridevi S

## Disclaimer

This project is developed for academic purposes. AI-generated clinical notes and diagnostic code suggestions must be reviewed and verified by qualified healthcare professionals before clinical use.

---

**License:** Academic Project
