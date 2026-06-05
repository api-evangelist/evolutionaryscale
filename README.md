# EvolutionaryScale (evolutionaryscale)

EvolutionaryScale is a New York-based biology foundation model lab spun out of Meta AI's ESM team that develops AI to deepen scientific understanding of biology. Its flagship ESM3 model is a multimodal generative protein language model that reasons jointly across sequence, structure, and function, scaling to 98B parameters trained on 771B tokens from 2.78B natural proteins. The companion ESM Cambrian (ESM C) family provides protein representation learning at 300M–6B parameters as a performant ESM2 replacement. Models are accessible via the hosted Forge inference API (forge.evolutionaryscale.ai), an open-source Python SDK (`pip install esm`), open weights on Hugging Face, and AWS Marketplace (SageMaker, NVIDIA BioNeMo and NIM). EvolutionaryScale was integrated into the Biohub organization in 2025; the ESM SDK now lives at github.com/Biohub/esm.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/evolutionaryscale/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming

## Tags

- AI
- Artificial Intelligence
- Biology
- Bioinformatics
- Computational Biology
- Drug Discovery
- ESM
- ESM3
- ESM Cambrian
- Foundation Models
- Generative Biology
- Life Sciences
- Machine Learning
- Protein Design
- Protein Folding
- Protein Language Models
- Proteins
- Representation Learning
- Structure Prediction

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### EvolutionaryScale Forge ESM3 API

Hosted inference API for the ESM3 multimodal protein language model. Reasons jointly across sequence, structure, and function tracks. Provides generate, batch_generate, encode, decode, forward_and_sample, and logits operations across small (1.4B), medium (7B), and large (98B) parameter checkpoints. Accessed via the `esm` Python SDK (`pip install esm`) using a bearer token issued by forge.evolutionaryscale.ai. Closed beta with commercial license tiers.

- **Human URL:** [https://forge.evolutionaryscale.ai](https://forge.evolutionaryscale.ai)

#### Tags

- AI
- Biology
- Foundation Models
- Proteins
- ESM3
- Generation

#### Properties

- [Documentation](https://forge.evolutionaryscale.ai)
- [Source Code](https://github.com/Biohub/esm)
- [OpenAPI](openapi/evolutionaryscale-forge-esm3-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/evolutionaryscale-forge-esm3-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/evolutionaryscale-forge-esm3-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/evolutionaryscale-esm-protein-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/evolutionaryscale-generation-config-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/evolutionaryscale-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### EvolutionaryScale Forge ESM Cambrian API

Hosted inference API for the ESM Cambrian (ESM C) protein representation learning model family. Drop-in replacement for ESM2 offering comparable accuracy at lower memory footprint. Available in 300M, 600M, and 6B parameter sizes. Exposes encode and logits operations for generating protein sequence embeddings, hidden states, and per-residue logits for downstream representation tasks.

- **Human URL:** [https://forge.evolutionaryscale.ai](https://forge.evolutionaryscale.ai)

#### Tags

- AI
- Biology
- Foundation Models
- Proteins
- ESM Cambrian
- Embeddings
- Representation Learning

#### Properties

- [Documentation](https://forge.evolutionaryscale.ai)
- [Source Code](https://github.com/Biohub/esm)
- [OpenAPI](openapi/evolutionaryscale-forge-esmc-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/evolutionaryscale-forge-esmc-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/evolutionaryscale-forge-esmc-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/evolutionaryscale-logits-output-schema.json) — [JSON Schema](https://json-schema.org/specification)

### EvolutionaryScale Forge Folding API

Hosted folding and inverse-folding inference endpoints. `fold` predicts protein backbone coordinates plus pLDDT/PTM confidence from an input sequence; `inverse_fold` designs candidate sequences consistent with an input structure. Includes an `msa` endpoint for fetching multiple sequence alignments used to condition predictions.

- **Human URL:** [https://forge.evolutionaryscale.ai](https://forge.evolutionaryscale.ai)

#### Tags

- AI
- Biology
- Foundation Models
- Proteins
- Structure Prediction
- Inverse Folding

#### Properties

- [Documentation](https://forge.evolutionaryscale.ai)
- [Source Code](https://github.com/Biohub/esm)
- [OpenAPI](openapi/evolutionaryscale-forge-folding-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/evolutionaryscale-forge-folding-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/evolutionaryscale-forge-folding-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### EvolutionaryScale ESM Python SDK

Official Python SDK packaging ESM3 and ESM Cambrian model loaders, the `ESMProtein` multi-track data model, generation/sampling configurations, structure tokenization utilities, and a `forge.client()` factory that swaps local checkpoints for Forge-hosted inference without code changes. Installable from PyPI as `esm`. Mixed commercial / non-commercial licenses.

- **Human URL:** [https://github.com/Biohub/esm](https://github.com/Biohub/esm)

#### Tags

- AI
- Biology
- SDK
- Python
- Open Source
- ESM3
- ESM Cambrian

#### Properties

- [Source Code](https://github.com/Biohub/esm)
- [SDK](https://pypi.org/project/esm/)
- [Documentation](https://huggingface.co/biohub/esm3-sm-open-v1)
- [Documentation](https://huggingface.co/biohub/esmc-300m-2024-12)
- [Documentation](https://huggingface.co/biohub/esmc-600m-2024-12)
- [Code Examples](https://github.com/Biohub/esm/tree/main/cookbook)
- [Postman Collection](collections/evolutionaryscale-forge-esm3-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/evolutionaryscale-forge-esm3-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/evolutionaryscale-forge-esmc-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/evolutionaryscale-forge-esmc-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/evolutionaryscale-forge-folding-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/evolutionaryscale-forge-folding-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
