# Why This Project Satisfies Agentic RAG

## Portfolio Claim

**Support Ticket Resolver** is not a static prompt demo. It is a runnable full-stack AI application for **Support Ticket Resolver** that demonstrates the core expectations of a **Agentic RAG** project at **Intermediate** difficulty.

## What A Reviewer Can Verify

- A real React interface accepts user questions and shows final answers, cited sources, and timeline steps.
- A real FastAPI backend exposes `POST /api/ask`.
- A service pipeline runs the expected project flow: Planner Agent, Retriever Agent, Reasoning Agent, Reviewer Agent.
- Sample domain documents are stored in `backend/app/data/sample_docs`.
- The vector/search layer retrieves cited context instead of returning a generic answer.
- The run log database stores each request so the project behaves like an application workflow.
- Tests verify metadata, pipeline output, tool behavior, and full-stack file presence.

## Type Fit

Planner -> retriever -> reasoning step -> optional tool call -> final answer with sources and timeline.

## Framework And Orchestration Evidence

- `backend/app/services/pipeline.py` adds planner, retrieval, tool, reasoning, and final-answer steps.
- `backend/app/services/tools.py` exposes deterministic tools used by the agentic flow.

## Conclusion

This codebase justifies the **Agentic RAG** label because the selected framework or orchestration pattern appears in executable backend code, the API returns observable timeline evidence, and the tests verify that the generated project runs as a real application rather than a static prompt sample.

## Recruiter / Interview Talking Points

- Explain why this project type was chosen for the domain.
- Walk through how the backend converts a user request into timeline steps.
- Show how cited sources reduce hallucination risk.
- Discuss how Docker, tests, and environment variables make the repo runnable by someone else.
- Describe one production upgrade: authentication, file upload, richer vector DB, background jobs, or deployment.
