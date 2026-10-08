# Accessibility Baseline & Repository Architecture Audit

## Project Overview

This project documents an accessibility and performance audit of the public-facing Government of India portal (india.gov.in).

The audit was performed using Chrome Lighthouse and a keyboard-only navigation review.

## Audit Target

**Website:** https://www.india.gov.in/

## Lighthouse Results

| Category | Score |
|---|---:|
| Performance | 48 |
| Accessibility | 88 |
| Best Practices | 88 |
| SEO | 92 |

## Key Findings

1. Render-blocking resources affecting page loading performance.
2. Inefficient cache lifetimes for static resources.
3. ARIA elements with incorrect parent/child relationships.
4. Focusable elements contained inside `aria-hidden="true"` elements.
5. Image delivery can be improved to reduce page weight.

## Repository Structure

```text
accessibility-baseline-repository/
├── client/
├── server/
├── docs/
│   ├── audit-report.md
│   └── architecture.md
├── tests/
└── README.md
