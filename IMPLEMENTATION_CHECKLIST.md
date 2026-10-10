# Implementation Checklist

Build the application yourself using `PROJECT_BRIEF.md`.

## Initial setup

- [ ] Read the project specification.
- [ ] Review the architecture and data model.
- [ ] Create a Python virtual environment.
- [ ] Install and pin the required dependencies.
- [ ] Configure credentials through environment variables.
- [ ] Review the data privacy and security requirements.

## Project acceptance criteria

- [ ] Upload succeeds for at least 10 sample arXiv PDFs
- [ ] Embeddings stored with <0.5 s latency per chunk
- [ ] Citation edges created correctly (>=90% of detected citations)
- [ ] API returns combined results within 2 s for queries on 5 k papers
- [ ] At least 1 citation hop is included for 70% of queries
- [ ] Answers include a "Sources" section with correct paper IDs
- [ ] Human evaluator rates relevance ≥4/5 on 20 test questions
- [ ] Create repo, CI pipeline, Dockerfile
- [ ] Implement PDF text extraction (pdfminer)
- [ ] Build Neo4j schema & citation parser
- [ ] Generate embeddings with sentence‑transformers
- [ ] Unit tests for PDF parsing and citation extraction
- [ ] Integration tests for vector‑graph pipeline using pytest‑asyncio
- [ ] Load test: 100 concurrent /search requests with locust (target <2 s latency)
- [ ] Security test: OWASP API Top 10 scan
- [ ] Containerize with Docker Compose (api, postgres, neo4j)
- [ ] Deploy to Railway or Render (free tier) for MVP
- [ ] Configure HTTPS via Let's Encrypt
- [ ] Set up GitHub Actions to build, test, and push Docker images

## Before completion

- [ ] Implement the planned MVP features.
- [ ] Add unit and integration tests.
- [ ] Run the test suite.
- [ ] Measure the evaluation metrics in the brief.
- [ ] Record actual results and known limitations.
- [ ] Document setup and deployment.
- [ ] Update the README to reflect the implemented features.
- [ ] Add only verified outcomes to your resume.
