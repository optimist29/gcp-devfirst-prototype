# Google Cloud: Developer-First Product Page Evolution ⚡

> An interactive side-by-side prototype demonstrating how to rewrite Google Cloud product pages (starting with **Cloud Run** and **Cloud Spanner**) using modern developer marketing principles: **The Flaw-First Anti-Pitch**, **Zero-Fluff Receipts**, **Lambda Concurrency Proofs**, and **Migration Honesty**.

## 🌐 Live Interactive Demo

Try the side-by-side interactive prototype:
👉 **[https://optimist29.github.io/gcp-devfirst-prototype/](https://optimist29.github.io/gcp-devfirst-prototype/)**

---

## What This Demonstrates

Cloud marketing pages are traditionally written for procurement committees, but the purchase decision is now made by an engineer in a terminal (or an AI coding agent reading docs on their behalf).

This project demonstrates the contrast between:
1. **Current Corporate Website (`cloud.google.com`)**: Vague value propositions (*"seamless autoscaling"*, *"empower developers"*), zero copy-pasteable code on the hero screen, and buried pricing calculators.
2. **Developer-First Redesign**:
   - **1-Command Runnable Hero:** Immediate `gcloud` deploy command on the first screen.
   - **The Anti-Pitch (When NOT to use):** Explicitly tells developers when a product is the wrong fit (e.g. persistent disk state, 24/7 flat CPU, heavy idle WebSockets).
   - **The Concurrency Proof:** Shows why Cloud Run beats AWS Lambda (1 container multiplexing 80 requests vs 80 cold lambdas).
   - **The Transparent Receipt:** Granular vCPU-second / GiB-second math with an interactive monthly bill calculator.
   - **Migration Honesty (Cloud Spanner):** Explicitly states the multi-region consensus lock-in and outlines the exact escape route.

---

## Included Playbooks & Research

- [`PLAYBOOK.md`](./PLAYBOOK.md): The comprehensive 4-part framework to scale developer-first pages across Cloud Run, Spanner, GKE, and BigQuery.
- [`VERCEL_ANALYSIS.md`](./VERCEL_ANALYSIS.md): Competitive teardown of Vercel product pages vs. Google Cloud, detailing where Vercel wins on DX and where Google Cloud can beat them on infrastructure transparency and open OCI container standards.

---

## Running Locally

```bash
# Clone the repository
git clone https://github.com/optimist29/gcp-devfirst-prototype.git
cd gcp-devfirst-prototype

# Serve index.html with any static server
npx serve .
# or
python3 -m http.server 8080
```

Open `http://localhost:8080` in your browser.

---

## License

MIT © Praveen
