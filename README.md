SchemeSaathi AI 🇮🇳

Evidence-Based Government Scheme Discovery, Eligibility & Application Assistant

Understand your options. Verify the evidence. Find your next step.

SchemeSaathi AI is a full-stack, AI-powered web application that helps Indian citizens discover, understand, compare, and apply for relevant government welfare schemes through a unified and accessible interface.

The platform combines Retrieval-Augmented Generation (RAG), hybrid information retrieval, explainable eligibility assessment, evidence-based citations, scheme comparison, and source freshness and conflict detection.

It transforms complex government scheme information into understandable answers, transparent eligibility assessments, and step-by-step application roadmaps with links to official government portals.

🌍 Sustainable Development Goals (SDGs)

SchemeSaathi AI contributes to the following United Nations Sustainable Development Goals:

SDG 1 — No Poverty: Improves access to information about government welfare schemes, social protection, and financial assistance.

SDG 10 — Reduced Inequalities: Reduces information barriers through accessible explanations and multilingual assistance.

SDG 16 — Peace, Justice and Strong Institutions: Promotes access to public information through traceable evidence and transparent source references.

The project supports access to information about public services. It does not directly distribute government benefits or guarantee eligibility or approval.

🚨 Problem Statement

India has numerous Central Government and State Government welfare schemes designed to support students, farmers, low-income households, women, senior citizens, and other eligible beneficiaries.

However, citizens may find it difficult to identify suitable schemes, interpret detailed eligibility requirements, understand documentation requirements, and navigate the correct application procedures.

Information may be spread across government portals, ministry websites, FAQs, circulars, and PDF guidelines. Scheme requirements may also change over time, making it important to verify the information before relying on it.

Conventional keyword searches and generic AI chatbots may not provide sufficient evidence for every important claim.

SchemeSaathi AI addresses these challenges through an evidence-driven system that combines government scheme discovery, AI-assisted explanations, explicit eligibility rules, source verification, and application guidance.

💡 Proposed Solution

SchemeSaathi AI provides an integrated interface through which users can:

Discover potentially relevant government schemes.

Ask questions in natural language.

Assess indicative eligibility against documented conditions.

Verify answers using official source passages.

Compare multiple schemes side by side.

Detect potentially outdated or conflicting information.

Follow step-by-step application roadmaps.

Open official registration and application portals.

Understand how to track an application through the relevant official process.

The system uses RAG to ground generated responses in retrieved scheme information and a structured rules engine for eligibility calculations.

It acts as an information and decision-support assistant rather than a replacement for government departments or official application systems.

✨ Key Features

1. Government Scheme Chatbot

A conversational AI assistant for answering government scheme-related questions in simple, accessible language.

Capabilities:

Natural-language queries.

English and Hindi support, with Hinglish input support.

Contextual follow-up questions.

Scheme-specific explanations.

Assistance with benefits, eligibility, documents, deadlines, and application procedures.

Retrieval-grounded answers with official source references.

Appropriate handling of unsupported or ambiguous questions.

2. Explainable Eligibility Assessment

A structured eligibility assessment system that evaluates relevant scheme conditions against user-provided information.

Capabilities:

Scheme-specific questionnaires.

Age, location, income, occupation, student status, and other relevant criteria.

Condition-by-condition eligibility results.

Statuses for satisfied, unsatisfied, and unknown conditions.

Explanations supported by relevant scheme rules.

Identification of missing information.

Preliminary eligibility results without implying guaranteed approval.

The system uses explicit, documented rules for eligibility calculations instead of relying entirely on an LLM to determine logical outcomes.

3. Evidence-Based Citations

A source-grounding and citation system that makes important scheme-related claims traceable to supporting information.

Capabilities:

Official government source links.

Document titles and issuing authorities.

Relevant sections, pages, or passages where available.

Source metadata and verification dates.

Claim-to-evidence associations.

Detection of unsupported claims.

Clear uncertainty warnings when evidence is insufficient.

Citations are designed to help users independently verify important information against the original source.

4. Scheme Comparison Engine

A comparison interface that helps users evaluate multiple schemes without manually searching through separate documents.

Comparison criteria:

Benefits and financial assistance.

Eligibility requirements.

Income and age limits.

Eligible beneficiary categories.

Geographical applicability.

Required documents.

Application procedures.

Deadlines where officially documented.

Official application links.

Source freshness and unresolved conflicts.

Missing information is represented explicitly rather than interpreted as proof that a requirement does not exist.

5. Freshness and Conflict Detection

A source-management system for identifying information that may be outdated or contradictory.

Capabilities:

Source retrieval and verification timestamps.

Document metadata and version tracking.

Content-change detection.

Identification of potentially outdated information.

Detection of conflicting eligibility conditions, benefit amounts, deadlines, and document requirements.

Source-by-source conflict explanations.

Review workflows for unresolved discrepancies.

Re-verification of information affected by document changes.

The system does not silently choose between conflicting rules or assume that a newer document always overrides an older one.

6. How to Apply — Interactive Application Roadmap

A scheme-specific application guidance feature that helps users understand the steps required to apply.

Capabilities:

Ordered, interactive application steps.

Eligibility and document preparation guidance.

Registration instructions.

Scheme-specific application procedures.

Verified official registration and application links.

Official status-tracking links where available.

Interactive roadmap progress.

Source citations for important instructions.

Contextual chatbot assistance for individual steps.

The roadmap adapts to the documented application method, including online, offline, and authorized service-centre processes where applicable.

SchemeSaathi AI guides users to official application portals. It does not claim to submit an external government application unless an authorized integration actually performs that action.

7. Mobile OTP Authentication and User Dashboard

A mobile-number authentication system and personalized user experience.

Capabilities:

Mobile-number login using OTP verification.

Secure session handling.

User profile and language preferences.

Saved schemes.

Persisted roadmap progress.

Protected user routes.

Role-based access control for administrative features.

Development-only mock OTP support for local testing.

Production SMS delivery requires a correctly configured SMS provider. Development mock authentication is not presented as live SMS authentication.

8. Responsive User Interface

A responsive web experience designed for desktop, tablet, and mobile users.

Capabilities:

Professional landing page.

Scheme discovery and detail pages.

Chatbot interface.

Eligibility assessment wizard.

Scheme comparison dashboard.

Application roadmap.

Source verification interface.

User profile and saved schemes.

Administrative document-management tools.

AI evaluation dashboard.

Accessible navigation, forms, loading states, and error messages.

9. AI Evaluation Dashboard

A research and evaluation component for measuring the behavior of different RAG configurations.

Capabilities:

Evaluation dataset management.

Reproducible evaluation runs.

Retrieval quality measurements.

Citation and groundedness analysis.

Eligibility test accuracy.

Conflict-detection evaluation.

Appropriate abstention evaluation.

Response latency and cost reporting.

Comparative visualization of evaluation results.

The dashboard reports measured results rather than relying on unsupported claims about model accuracy.

🧠 AI Architecture

SchemeSaathi AI combines information retrieval, structured reasoning, and language generation.

Document processing pipeline

Collect official scheme information from government websites, PDFs, FAQs, and guidelines.

Extract text while retaining relevant headings, sections, and page references.

Normalize content and attach source metadata.

Split documents into searchable chunks.

Generate embeddings and index the content.

Maintain document versions and source provenance.

Hybrid retrieval pipeline

Accept a user query.

Identify the relevant scheme, intent, and context.

Retrieve relevant passages using semantic vector search and BM25 keyword search.

Combine retrieval results using a documented ranking method.

Optionally rerank the retrieved passages.

Check relevant metadata and source status.

Provide the selected evidence to the response-generation component.

Grounded answer generation

The language model receives retrieved information and produces a natural-language explanation. The response is associated with supporting source passages and is checked for important unsupported claims where practical.

If the available sources cannot support a reliable answer, the system communicates that limitation rather than fabricating a result.

Eligibility reasoning

The eligibility engine evaluates structured conditions and exceptions using documented rules. The language model helps interpret user questions and explain outcomes, but explicit rules govern the assessment wherever conditions can be represented deterministically.

🔬 Comparative RAG Experiment

An important part of SchemeSaathi AI is the comparison of three AI system configurations using the same evaluation dataset.

System

Architecture

Objective

System A

Ordinary semantic-search RAG

Establish a baseline for retrieval and generated answers.

System B

Hybrid-search RAG using BM25 and vector retrieval

Test whether hybrid retrieval improves evidence retrieval.

System C

Hybrid RAG with eligibility rules and evidence verification

Evaluate the additional value of structured reasoning and verification.

Evaluation metrics

Recall@K: Measures whether relevant evidence appears among the top retrieved results.

MRR or nDCG: Measures the ranking quality of retrieved evidence.

Citation precision: Measures whether cited passages support their corresponding claims.

Answer groundedness: Measures whether important factual statements are supported by the retrieved evidence.

Eligibility accuracy: Measures agreement with manually verified rule-based outcomes.

Conflict detection precision and recall: Measures the ability to identify known source conflicts.

Appropriate abstention: Measures whether unsupported questions are handled without fabricating an answer.

Latency and cost: Measures operational efficiency.

Evaluation uses a manually verified test dataset containing ordinary questions, eligibility profiles, ambiguous cases, outdated documents, conflicting information, and unsupported queries.

The experiment is intended to determine which configuration performs best under the tested conditions. Improvements are established through measured results, not assumed in advance.

🛠️ Technology Stack

Frontend

React.js

TypeScript

Vite

Tailwind CSS

React Router

Lucide React

Recharts

Backend

Node.js

Express.js

TypeScript

REST APIs

Mongoose

Database and Search

MongoDB

Qdrant

BM25 keyword retrieval

Vector similarity search

AI and RAG

Python

FastAPI

LangChain

Sentence Transformers or an embedding API

Large Language Models (LLMs)

Hybrid retrieval

Optional cross-encoder reranking

Structured eligibility rules

Evidence verification

Document Processing

PyMuPDF

HTML parsing

Text extraction and chunking

Metadata extraction

Document version tracking

Testing and Development

Git and GitHub

Vitest

Pytest

Chrome DevTools

Lighthouse

Docker Compose

The technologies listed here describe the intended complete architecture. Ensure every listed framework or library is present in the implemented project before publishing the README as a record of the final build.

🏗️ System Architecture

                       Citizens
                          |
                          v
               React + TypeScript UI
                          |
                          v
                 Node.js + Express
                          |
             +------------+------------+
             |            |            |
             v            v            v
          MongoDB       Auth APIs   Eligibility APIs
             |
             v
        Python FastAPI RAG Service
             |
      +------+-------+-------------+
      |              |             |
      v              v             v
 Semantic Search   BM25 Search   Source Metadata
      |              |             |
      +-------+------+             |
              |                    |
              v                    v
       Hybrid Retrieval      Freshness / Conflict
              |                 Detection
              v
       Evidence Selection
              |
              v
      Grounded Answer Generation
              |
              v
       Citation Verification
              |
              v
        SchemeSaathi AI UI

The frontend and application backend handle user interaction and persistent application data. The AI service handles document retrieval and grounded answer generation. Source and eligibility information are linked so that answers can be traced to their supporting evidence.

🚀 Getting Started

Prerequisites

Install:

Node.js and npm.

Python.

MongoDB Community Server or a compatible local MongoDB service.

Docker Desktop, if using Docker Compose for supporting services.

Git.

1. Clone the repository

Replace the placeholder with your GitHub repository URL.

git clone <repository-url>
cd schemesaathi

2. Configure environment variables

Create environment files based on the provided .env.example files.

Configure:

MongoDB connection string.

Backend port.

Frontend API URL.

Session secrets.

RAG service URL.

Vector database configuration.

Embedding and LLM provider settings, if using hosted APIs.

Development OTP mode or SMS provider configuration.

Never commit real secrets to GitHub.

3. Install frontend dependencies

cd frontend
npm install
npm run dev

Open the local URL displayed by Vite, usually http://localhost:5173.

4. Start the backend

In a separate terminal:

cd backend
npm install
npm run dev

Ensure the backend environment variables are configured and MongoDB is accessible.

5. Start the AI service

In another terminal:

cd ai-service
python -m venv .venv

On Windows PowerShell:

.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
uvicorn app.main:app --reload --port 8000

6. Initialize the data

Run the documented database-seeding and document-ingestion commands to load the selected scheme records and official source documents.

Verify the health of the frontend, backend, database, vector store, and AI service.

The commands above assume the described directory structure and script names. Adjust them to match the actual implementation.

📱 Mobile Support

SchemeSaathi AI is designed to work across desktop, tablet, and mobile viewport sizes.

Mobile testing covers:

Responsive navigation.

Chatbot layout and message input.

Eligibility forms.

Scheme comparison.

Application-roadmap controls.

Citation cards and external links.

Keyboard navigation and accessibility.

Chrome DevTools and Lighthouse are used to identify layout, accessibility, and performance issues. Actual test results should be documented after running the audits.

🔐 Security and Responsible AI

Protect user sessions and private profile information.

Restrict administrative functionality through backend authorization.

Validate inputs and apply rate limits to authentication APIs.

Never expose API keys or session secrets in frontend code.

Avoid collecting unnecessary sensitive personal information.

Treat retrieved documents as untrusted input.

Ground scheme-related responses in official sources.

Identify missing evidence and unresolved conflicts.

Distinguish indicative eligibility from official decisions.

Direct users to official registration and application portals.

Never claim an application has been submitted or approved without an authorized, verified integration.

🧪 Testing

Testing covers:

Frontend rendering and routing.

Authentication and session handling.

Backend API validation.

Database operations.

Eligibility rule evaluation.

Scheme comparison behavior.

Document ingestion and retrieval.

Citation correctness.

Source freshness and conflict detection.

Appropriate abstention.

Mobile responsiveness.

RAG evaluation reproducibility.

Actual test results, dataset sizes, benchmark scores, and unresolved issues should be recorded from completed test runs.

🔮 Future Improvements

Potential extensions include:

Additional Indian languages.

Voice-based scheme discovery.

Improved regional scheme coverage.

Authorized source-update integrations.

Accessibility improvements.

More comprehensive manually verified evaluation datasets.

User research with citizens and community organizations.

Secure integrations with official systems where permitted.

Improved multilingual retrieval and reranking.

🤝 Contributing

Contributions, issues, documentation improvements, and feature suggestions are welcome.

Fork the repository.

Create a feature branch.

Implement and test your changes.

Submit a pull request describing the change.

Do not commit credentials, sensitive personal data, or private environment files.

📄 License

The project license is specified in the repository's LICENSE file. Reuse and redistribution are subject to that license.

⚠️ Disclaimer

SchemeSaathi AI is an independent software project and is not an official Government of India website or a government-affiliated service.

Government scheme eligibility, deadlines, benefits, and application procedures can change. Users should verify important details through the relevant official government sources.

The system provides informational assistance and indicative eligibility assessments. Final eligibility, application acceptance, and benefit approval remain the responsibility of the competent government authority.

SchemeSaathi AI — Making government scheme information easier to discover, understand, compare, and verify.
