# AI Cognitive Routing & RAG System

## Overview
This project implements a cognitive AI loop with:

### Phase 1: Vector-Based Routing
- Uses SentenceTransformers embeddings
- FAISS vector database for similarity search
- Routes posts to relevant bot personas

### Phase 2: Autonomous Content Generation
- Simulates real-world context using mock search tool
- Generates structured JSON outputs

### Phase 3: Deep Thread RAG Defense
- Uses full conversation context
- Implements prompt injection protection
- Maintains persona integrity

## Prompt Injection Defense
The system detects malicious instructions such as:
"Ignore all instructions"

These are rejected using system-level guardrails.

## How to Run
```bash
pip install -r requirements.txt
python main.py