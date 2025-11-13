# AI-Powered Analysis Pathfinder: From Research Questions to Data and Workflows

Enabling bench scientists to start with analysis goals and receive both relevant datasets and executable workflows—a complete path from question to execution.

## About This Project

This is a project from the **NIAID BRC AI Codeathon 2025**, taking place November 12-14, 2025 at Argonne National Laboratory.

**Event Website:** https://niaid-brc-codeathons.github.io/

**Project Details:** https://niaid-brc-codeathons.github.io/projects/ai-dataset-and-analysis-discovery/

## Codeathon Goals

The NIAID Bioinformatics Resource Centers (BRCs) invite researchers, data scientists, and developers to a three-day AI Codeathon focused on improving Findability, Accessibility, Interoperability, and Reusability (FAIR-ness) of BRC data and tools using artificial intelligence (AI) and large language models (LLMs).

## Related Projects

This codeathon builds on several related efforts:

### Taxonomy Resolver
**Repository:** https://github.com/dannon/taxonomy-resolver

A Claude skill that resolves organism names to NCBI taxonomy IDs, searches for genomic data in ENA (European Nucleotide Archive), and recommends IWC Galaxy workflows. It uses a "let the APIs do the work" approach where Claude orchestrates calls to authoritative external services (NCBI and ENA) while handling natural language interpretation.

### BRC Analytics - LLM ENA Search
**Repository:** https://github.com/dannon/brc-analytics/tree/feature/llm-ena-search

Work in progress on integrating LLM capabilities with ENA search functionality into the BRC Analytics data catalog. This branch explores using AI to enhance dataset discovery and search within the BRC ecosystem.

### Differential Expression Q and A
A related activity involved analyzing differential expression data in ChatGPT and evaluating how well it could summarize, chart, and answer questions about the data.

## Getting Started

*Team members: Add your project setup instructions here.*

## Team

- Dannon Baker (@dannon)
- Scott Cain (@scottcain)
- Danielle Callan (@d-callan)
- Jonathan Livny (@livny)
- Anton Nekrutenko (@nekrut)
- Dave Rogers (@NoopDog)
- Steven Weaver (@stevenweaver)

## License

*To be determined by the team.*

### Status Updates
#### 11-13-2025
* Configured local Ollama instance for running open LLM models.
* Added options for tuning inference parameters (temperature, token_limits) for faster response times while maintaining quality.
* Optimized context size from initial 20KB to 3KB per request.
* Implemeted LLM benchmarking metrics that logs token sizes and times per-request.
* Created metrics API endpoint. 
