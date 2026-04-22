# bioanchor-permanent-mcmc-archival

## Proposal Name
bioanchor-permanent-mcmc-archival

## Motivation
Reproducibility is a crisis in biomedical science. Researchers running 
Bayesian/MCMC statistical models — in drug discovery, genomics, and 
clinical trials — have no standard way to permanently preserve their 
analysis provenance. Files disappear. Journal links rot.

BioAnchor solves this by permanently archiving MCMC analysis metadata 
to Arweave, making it the world's first open-source Python tool 
bridging the scientific computing stack (PyMC 5, Stan) with Arweave 
permanent storage. No prior art exists on PyPI or in the literature.

This grant would support continued development and community outreach 
to bring Arweave adoption to the global biomedical research community.

## Specification

BioAnchor v0.1.0 (live on PyPI: `pip install bioanchor`) provides:

- **Manifest format**: structured JSON capturing model parameters, 
  sampler diagnostics (R-hat, ESS, divergences), and full provenance
- **ArweaveUploader**: direct upload via arweave-python-client
- **TurboUploader**: upload via ArDrive Turbo SDK (AR.IO compatible)
- **MockUploader**: fallback for offline/testing environments
- **PyMC 5 integration**: `anchor_mcmc()` wrapping standard workflows
- **CLI**: `bioanchor upload` for standalone use

Verified real Arweave upload:
TX: `2lIZtjsu120ERqPKu6XbITpUnAveWeH7hI4owBfNCdY`

**Roadmap with this grant:**
- Stan/CmdStanPy integration
- arviz InferenceData full serialization  
- Permaweb-hosted documentation site
- Bioinformatics (Oxford) journal submission

## Deliverables

- Stan integration (v0.2.0 release on PyPI)
- arviz full diagnostic serialization
- Permaweb documentation site via AR.IO
- Journal manuscript submission (Bioinformatics Oxford)

## Team

**Dohoon Kim** — Founder, Promptgenix LLC  
GitHub: https://github.com/kdh4win4  
Repository: https://github.com/kdh4win4/bioanchor  
PyPI: https://pypi.org/project/bioanchor/  
Email: dkim@promptgenix.org  
bioRxiv: under review (BIORXIV/2026/719695)

## Funding Request

**$1,500 USD equivalent in AR**

- Stan integration development: $800
- Arweave upload costs for CI/test suite: $200  
- Permaweb documentation hosting: $500
