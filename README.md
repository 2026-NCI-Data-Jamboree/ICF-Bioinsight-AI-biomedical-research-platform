# BioInsight AI Biomedical Research Platform for Translation Exploration developed by ICF Team

## NCI Data Jamboree 2026

### Project Overview

This project demonstrates how **BioInsight AI**, a modular agentic AI platform for biomedical research, can connect scientific publications, multimodal cancer data, and clinical trial information through an explainable conversational workflow.

The project addresses a common challenge in translational research: relevant evidence is distributed across publications, molecular datasets, clinical annotations, and clinical trial registries. BioInsight helps researchers follow a scientific question across these sources while preserving **provenance, citations, scientific context, and limitations**.

### Jamboree Use Case

We used **HER2-positive breast cancer** as a demonstration case and followed a progressive discovery workflow:

1. **From publication to supporting data**  
   Starting from published findings suggesting **GPRC5A and TPBG** as potential markers associated with incomplete treatment response, BioInsight explored pretreatment proteomic data from **CALGB 40601 (PDC000582)** to compare these proteins between pathological complete response (pCR) and non-pCR cases.

2. **From one study to an independent cohort**  
   BioInsight then explored the independent **CPTAC prospective breast cancer cohort (PDC000120)** to identify tumors with elevated HER2/ERBB2, GPRC5A, and TPBG protein abundance. Cases were flagged for further research without interpreting co-elevation as evidence of treatment resistance when treatment-response information was unavailable.

3. **From molecular evidence to clinical research**  
   Finally, we integrated **ClinicalTrials.gov** retrieval to identify currently recruiting trials addressing HER2-positive early breast cancer with residual disease after neoadjuvant treatment and compare their treatments and biomarker requirements with CALGB 40601.

### What We Demonstrated

- An **agentic, conversational workflow** connecting literature, proteomics, genomics, clinical annotations, and clinical trial information.
- **Traceable and source-grounded exploration**, with citations, provenance, and explicit handling of missing information and scientific uncertainty.
- An **extensible modular architecture** in which additional biomedical data sources and modalities can be incorporated without redesigning the complete platform.
- A practical approach for moving from a published biological observation to supporting molecular evidence, independent-cohort exploration, and relevant clinical research.

The broader lesson from the project is that **FAIR, well-curated data still require scientific context for meaningful reuse**. AI-assisted workflows such as BioInsight can help connect that context while making evidence boundaries and uncertainties visible.

### Extensibility

The HER2 breast cancer investigation represents one example of the workflow. The same modular approach can be extended to other cancers, research questions, and datasets. As additional resources become publicly available, new source-specific agents and tools can be integrated into BioInsight to support similarly **meaningful, verifiable, reproducible, and reusable scientific exploration**.

## BioInsight AI

The public BioInsight implementation, source code, installation instructions, and supporting resources are available here:

**[BioInsight AI / BDF Public Repository](https://github.com/esacinc/BDF-Public)**

The public repository includes the `bioinsight_ai` application as well as setup instructions and integrations used by the platform.

## Feedback & Contact
We’d love to hear from you! If you have feedback, questions, or suggestions, feel free to reach out to us at <bioinsight-ai@icf.com>.

---

*NCI Data Jamboree 2026 – AI-Assisted Translational Exploration*
