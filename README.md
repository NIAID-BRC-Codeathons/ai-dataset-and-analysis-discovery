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

A Claude skill that bridges natural language queries and specialized bioinformatics databases. The skill enables researchers to work with organism data using common names rather than formal taxonomic identifiers.

**Key Capabilities:**
- **Taxonomy Resolution**: Converts common organism names (e.g., "malaria parasite") to scientific nomenclature ("Plasmodium falciparum") and NCBI taxonomy IDs
- **Genomic Data Discovery**: Searches the European Nucleotide Archive (ENA) for FASTQ files and genome assemblies with accession numbers and metadata
- **Workflow Recommendations**: Suggests appropriate Galaxy workflows from the Intergalactic Workflow Commission (IWC) based on data characteristics
- **Smart Disambiguation**: Uses conversational interactions to clarify ambiguous organism references before making API calls

**Technical Approach:**
Built on a "let the APIs do the work" philosophy - Claude orchestrates calls to authoritative external services (NCBI Taxonomy API, ENA Portal API, IWC Workflow Registry) while handling natural language interpretation. Implemented in Python 3.6+ with no external dependencies, prioritizing verifiable data accuracy over embedded AI knowledge.

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
