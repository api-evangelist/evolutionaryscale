# EvolutionaryScale (evolutionaryscale)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
