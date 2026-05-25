# EvolutionaryScale (evolutionaryscale)

EvolutionaryScale is a New York-based biology foundation model lab spun out of Meta AI's ESM team that develops AI to deepen scientific understanding of biology. Its flagship ESM3 model is a multimodal generative protein language model that reasons jointly across sequence, structure, and function, scaling to 98B parameters trained on 771B tokens from 2.78B natural proteins. The companion ESM Cambrian (ESM C) family provides protein representation learning at 300M–6B parameters as a performant ESM2 replacement. Models are accessible via the hosted Forge inference API (forge.evolutionaryscale.ai), an open-source Python SDK (`pip install esm`), open weights on Hugging Face, and AWS Marketplace (SageMaker, NVIDIA BioNeMo and NIM). EvolutionaryScale was integrated into the Biohub organization in 2025; the ESM SDK now lives at github.com/Biohub/esm.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - AI, Artificial Intelligence, Biology, Bioinformatics, Computational Biology, Drug Discovery, ESM, ESM3, ESM Cambrian, Foundation Models, Generative Biology, Life Sciences, Machine Learning, Protein Design, Protein Folding, Protein Language Models, Proteins, Representation Learning, Structure Prediction

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Models

| Model | Family | Parameters | Access |
|---|---|---|---|
| `esm3-large-2024-03` | ESM3 | 98B | Forge |
| `esm3-medium-2024-08` | ESM3 | 7B | Forge |
| `esm3-small-2024-08` | ESM3 | 1.4B | Forge |
| `esm3-open` (`biohub/esm3-sm-open-v1`) | ESM3 | 1.4B | Open weights (research) |
| `esmc-6b-2024-12` | ESM Cambrian | 6B | Forge |
| `esmc-600m-2024-12` | ESM Cambrian | 600M | Forge + Open weights |
| `esmc-300m-2024-12` | ESM Cambrian | 300M | Forge + Open weights |

ESM3 was trained on 771B tokens from 2.78B natural proteins (1e24 FLOPs).

## APIs

### EvolutionaryScale Forge ESM3 API
Hosted inference for the ESM3 multimodal protein language model. Generate, batch-generate, encode, decode, forward-and-sample, and logits across small (1.4B), medium (7B), and large (98B) checkpoints. Reasons jointly across sequence, structure, secondary_structure, sasa, and function tracks.

**Human URL:** [https://forge.evolutionaryscale.ai](https://forge.evolutionaryscale.ai)

- [Documentation](https://forge.evolutionaryscale.ai)
- [SourceCode](https://github.com/Biohub/esm)
- [OpenAPI](openapi/evolutionaryscale-forge-esm3-api-openapi.yml)
- [JSON Schema — ESMProtein](json-schema/evolutionaryscale-esm-protein-schema.json)
- [JSON Schema — GenerationConfig](json-schema/evolutionaryscale-generation-config-schema.json)
- [JSON-LD](json-ld/evolutionaryscale-context.jsonld)
- [Naftiko Capability — Generation](capabilities/forge-esm3-generation.yaml)
- [Naftiko Capability — Encoding](capabilities/forge-esm3-encoding.yaml)

### EvolutionaryScale Forge ESM Cambrian API
Hosted inference for the ESM Cambrian (ESM C) representation learning family. Drop-in ESM2 replacement with lower memory footprint, available at 300M, 600M, and 6B parameters. Exposes sequence-only encode and logits for embedding workflows.

**Human URL:** [https://forge.evolutionaryscale.ai](https://forge.evolutionaryscale.ai)

- [Documentation](https://forge.evolutionaryscale.ai)
- [SourceCode](https://github.com/Biohub/esm)
- [OpenAPI](openapi/evolutionaryscale-forge-esmc-api-openapi.yml)
- [JSON Schema — LogitsOutput](json-schema/evolutionaryscale-logits-output-schema.json)
- [Naftiko Capability — Embeddings](capabilities/forge-esmc-embeddings.yaml)

### EvolutionaryScale Forge Folding API
Hosted folding and inverse-folding inference. `fold` predicts atom37 backbone coordinates plus pLDDT/PTM confidence; `inverse_fold` designs candidate sequences for a target structure; `msa` fetches multiple sequence alignments used to condition fold predictions.

**Human URL:** [https://forge.evolutionaryscale.ai](https://forge.evolutionaryscale.ai)

- [Documentation](https://forge.evolutionaryscale.ai)
- [SourceCode](https://github.com/Biohub/esm)
- [OpenAPI](openapi/evolutionaryscale-forge-folding-api-openapi.yml)
- [Naftiko Capability — Folding & Structure](capabilities/forge-folding-structure.yaml)

### EvolutionaryScale ESM Python SDK
Official Python SDK packaging ESM3 and ESM Cambrian model loaders, the `ESMProtein` multi-track data model, generation/sampling configurations, structure tokenization utilities, and a `forge.client()` factory that swaps local checkpoints for Forge-hosted inference without code changes. Installable from PyPI as `esm`. Mixed commercial / non-commercial licenses.

**Human URL:** [https://github.com/Biohub/esm](https://github.com/Biohub/esm)

- [SourceCode](https://github.com/Biohub/esm)
- [PyPI Package — `esm`](https://pypi.org/project/esm/)
- [Cookbook](https://github.com/Biohub/esm/tree/main/cookbook)

## Common Properties

- [Portal](https://www.evolutionaryscale.ai)
- [SignUp — EvolutionaryScale Forge](https://forge.evolutionaryscale.ai)
- [SourceCode — ESM SDK on GitHub](https://github.com/Biohub/esm)
- [SDK — `esm` package on PyPI](https://pypi.org/project/esm/)
- [Biohub on Hugging Face](https://huggingface.co/biohub)
- [Models — ESM3-open (1.4B) on Hugging Face](https://huggingface.co/biohub/esm3-sm-open-v1)
- [Models — ESM C 300M on Hugging Face](https://huggingface.co/biohub/esmc-300m-2024-12)
- [Models — ESM C 600M on Hugging Face](https://huggingface.co/biohub/esmc-600m-2024-12)
- [CodeExamples — ESM Cookbook](https://github.com/Biohub/esm/tree/main/cookbook)
- [Tutorials — ESM Tutorials](https://github.com/Biohub/esm/tree/main/cookbook/tutorials)
- [Documentation — ESM3 Science paper (Hayes et al. 2025)](https://www.science.org/doi/10.1126/science.ads0018)
- [Blog — ESM3 release announcement](https://www.evolutionaryscale.ai/blog/esm3-release)
- [Blog — ESM Cambrian announcement](https://www.evolutionaryscale.ai/blog/esm-cambrian)
- [Blog](https://www.evolutionaryscale.ai/blog)
- [Marketplace — EvolutionaryScale on AWS Marketplace (SageMaker)](https://aws.amazon.com/marketplace/seller-profile?id=seller-iw2nbscescndm)
- [CodeExamples — ESM on Amazon SageMaker examples](https://github.com/evolutionaryscale/esm-sagemaker)
- [CodeExamples — Partner integrations](https://github.com/evolutionaryscale/esm-partner)
- [TermsOfService — Cambrian Inference Clickthrough License](https://www.evolutionaryscale.ai/policies/cambrian-inference-clickthrough-license-agreement)
- [Documentation — Responsible Biodesign Framework](https://responsiblebiodesign.ai)
- [Forum — ESM Community Slack](https://bit.ly/esm-slack)
- [GitHub Organization — EvolutionaryScale](https://github.com/evolutionaryscale)
- [GitHub Organization — Biohub (ESM home)](https://github.com/Biohub)
- [Plans](plans/evolutionaryscale-plans-pricing.yml)
- [Rate Limits](rate-limits/evolutionaryscale-rate-limits.yml)
- [FinOps](finops/evolutionaryscale-finops.yml)
- [Vocabulary](vocabulary/evolutionaryscale-vocabulary.yml)

## Examples

- [Forge ESM3 — generate](examples/evolutionaryscale-forge-generate-example.json)
- [Forge Folding — fold](examples/evolutionaryscale-forge-fold-example.json)
- [Forge ESM Cambrian — logits](examples/evolutionaryscale-forge-esmc-logits-example.json)

## Rules

- [Spectral Ruleset](rules/evolutionaryscale-rules.yml)

## Features

- ESM3 — multimodal generative model jointly conditioning on protein sequence, structure, and function
- 98B-parameter ESM3 trained on 771B tokens from 2.78B natural proteins (1e24 FLOPs)
- ESM Cambrian (ESM C) representation models at 300M, 600M, and 6B parameters
- Forge API providing generate, batch_generate, encode, decode, forward_and_sample, and logits operations
- Fold and inverse-fold endpoints for structure prediction and structure-conditioned sequence design
- MSA endpoint for fetching multiple sequence alignments used by structure prediction
- Iterative masked sampling with configurable num_steps, temperature, top_p, and decoding schedules
- Per-track generation across sequence, structure, secondary_structure, sasa, and function tracks
- Structure tokenizer converting PDB / atom37 coordinates to and from discrete tokens
- ESMProtein and ESMProteinTensor data model unifying raw and tokenized representations
- Async/sync client surface (`async_generate`, `async_fold`, `async_encode`, ...) for high-throughput jobs
- Drop-in Forge client (`esm.sdk.client(model, token=...)`) replaces local checkpoints with hosted inference
- Open-weights ESM3-open (1.4B) and ESM Cambrian distributions on Hugging Face under research license
- AWS Marketplace deployment via SageMaker, NVIDIA BioNeMo, and NVIDIA NIM microservice
- Cookbook tutorials covering protein generation, embedding workflows, and esmGFP-style design
- Responsible Biodesign Framework governing model release and biosecurity review

## Position

Consuming

## Maintainer

- **Kin Lane** ([info@apievangelist.com](mailto:info@apievangelist.com)) — [apievangelist.com](https://apievangelist.com)
