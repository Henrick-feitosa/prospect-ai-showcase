# Validation record

Preparation date: November 14, 2026 (America/Sao_Paulo).

| Check | Result |
| --- | --- |
| Backend: `python -m pytest -q` | 56 passed; one Starlette/httpx compatibility deprecation warning |
| Frontend: `pnpm test` | 7 passed in 2 test files |
| Frontend: `pnpm build` | Passed, including TypeScript checking and static generation |
| Local database migrations | Passed with a fresh, isolated SQLite database |
| Browser demo | One synthetic research job completed with 6 records; business details and initial/final pipeline views inspected in English and Brazilian Portuguese |
| Console error log at end of demo | No error entries returned |

Frontend tested with Next.js 16.4.5 and Vitest 3.2.7. Application source was extracted from the supplied portfolio archive. A local pnpm build approval for esbuild was needed; the copied workspace configuration records it.

The browser exercise is a focused portfolio smoke check, not a full end-to-end regression suite or mobile validation. It did not repeat manual review submission, pipeline stage changes, exports, or authenticated deployment checks. No real-source queries were performed. No PostgreSQL/Redis/Celery container execution was performed. Historical claims about two real searches returning 20 records each were not revalidated or reused in the new post.

Only synthetic records are included in screenshots. Timestamps inside the UI are UTC; they can show November 15 while the local preparation date is November 14.

No GitHub repository, commit, LinkedIn post, upload, or public deployment was created during preparation.
