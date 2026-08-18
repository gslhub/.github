<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/gslhub/website/main/public/brand/gslhub-logo-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/gslhub/website/main/public/brand/gslhub-logo.svg">
  <img src="https://raw.githubusercontent.com/gslhub/website/main/public/brand/gslhub-logo.svg" alt="GSLHub — Generative Search Lab Hub" width="360">
</picture>

# GSLHub

### Independent applied research in Generative Search, GEO, AI systems and reproducible research

**Barcelona, Spain · Open research · Open-source infrastructure**

[Website](https://gslhub.com) · [Research](https://github.com/gslhub/research) · [Benchmarks](https://github.com/gslhub/benchmarks) · [Software](https://github.com/gslhub/software) · [Docs](https://github.com/gslhub/docs) · [Contact](mailto:research@gslhub.com)

</div>

---

## About GSLHub

**GSLHub — Generative Search Lab Hub** is an independent research initiative and open technological infrastructure focused on understanding how generative AI systems discover, select, cite and recommend information.

Our work combines **Generative Search research, Generative Engine Optimization (GEO), AI evaluation, governed evidence, reproducible experimentation and software engineering**.

The objective is not only to study generative systems, but to build the infrastructure required to make that research **auditable, repeatable and useful in real-world environments**.

## Research architecture

```text
Scientific problem
→ Hypothesis
→ Experiment
→ Controlled execution
→ Preserved research artifact
→ Evidence
→ Observation
→ Citation / Metric
→ Reproducibility review
→ Public dissemination
```

GSLHub treats metrics as traceable research outputs rather than isolated numbers. Scientific methodology lives in [`gslhub/research`](https://github.com/gslhub/research), benchmark specifications in [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks), reusable implementations in [`gslhub/software`](https://github.com/gslhub/software), and the governed operational platform in [`gslhub/website`](https://github.com/gslhub/website).

## Public repositories

### [`gslhub/website`](https://github.com/gslhub/website)

Public website and core research platform for experiment governance, controlled executions, evidence provenance, scientific metrics, research artifacts and reproducibility controls.

**Stack:** `Next.js` · `TypeScript` · `React` · `Payload CMS` · `MongoDB` · `Tailwind CSS` · `Node.js` · `GitHub Actions`  
**License:** `AGPL-3.0-only`

### [`gslhub/research`](https://github.com/gslhub/research)

Canonical methodological layer containing the research model, protocols, codebooks, governance, reproducibility requirements and citation metadata.

**License:** `CC BY 4.0` for original research documentation unless otherwise stated.

### [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks)

Reproducible benchmark and metric specifications for Generative Search and GEO. The current public baseline includes **AIR, CR, MCP and RCR**, a machine-readable benchmark definition and synthetic validation fixtures.

**License:** `CC BY 4.0` for original benchmark specifications and documentation.

### [`gslhub/software`](https://github.com/gslhub/software)

Reusable research software implementing independently testable parts of the GSLHub methodology. The first package, **`@gslhub/metrics-core` v0.1.0**, provides framework-independent deterministic AIR, CR, MCP and RCR calculations with exclusions, numerator/denominator data and SHA-256 audit checksums.

**Stack:** `TypeScript` · `Node.js` · `npm workspaces` · `GitHub Actions`  
**License:** `AGPL-3.0-only`

### [`gslhub/docs`](https://github.com/gslhub/docs)

Cross-project public technical and institutional documentation covering architecture, repository boundaries, governance and safe-publication standards.

**License:** `CC BY 4.0` unless otherwise stated.

### [`gslhub/branding`](https://github.com/gslhub/branding)

Approved GSLHub visual identity, light/dark logo variants, icon, palette and brand-usage guidance. Brand and trademark rights are handled separately from software and research-documentation licenses.

## Repository roadmap

| Area | Status | Purpose |
|---|---|---|
| [`website`](https://github.com/gslhub/website) | **Public** | Public site and core research platform |
| [`research`](https://github.com/gslhub/research) | **Public** | Canonical protocols, methodology and codebooks |
| [`benchmarks`](https://github.com/gslhub/benchmarks) | **Public** | Evaluation frameworks and reproducible metric specifications |
| [`software`](https://github.com/gslhub/software) | **Public** | Reusable research software and deterministic metric implementations |
| [`docs`](https://github.com/gslhub/docs) | **Public** | Technical and institutional documentation |
| [`branding`](https://github.com/gslhub/branding) | **Public** | Approved visual identity and usage guidance |
| **datasets** | Preparing | Reviewed dataset releases with per-release licensing |

Repositories are opened progressively only when their contents are documented, licensed and ready for public reuse.

## Core metric families

| Code | Metric | Primary question |
|---|---|---|
| **AIR** | Answer Inclusion Rate | How often is the evaluated target visibly included? |
| **CR** | Citation Rate | How often is the evaluated target explicitly cited? |
| **MCP** | Mean Citation Position | When cited, how early does the target appear? |
| **RCR** | Response Consistency Rate | How stable are controlled repetitions against a frozen baseline? |

The normative specifications are versioned in [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks), while reusable deterministic implementations are versioned independently in [`gslhub/software`](https://github.com/gslhub/software). This separation allows calculations to be tested against a frozen specification without coupling them to the application database or CMS.

## Open science and licensing

GSLHub uses licenses by output type:

- **Research platform and original software:** GNU AGPL-3.0-only unless a package states otherwise.
- **Original research and benchmark documentation:** Creative Commons Attribution 4.0 International (CC BY 4.0), unless otherwise stated.
- **Datasets:** licensed individually according to provenance, rights and research constraints.
- **Publications:** governed by their individual publication or publisher terms.
- **Brand assets and trademarks:** governed separately.

## Principles

**Transparent** — methodology and technical decisions should be inspectable.  
**Reproducible** — experiments should preserve enough context to be repeated.  
**Evidence-driven** — conclusions should remain traceable to preserved evidence.  
**Technically rigorous** — research infrastructure should be engineered with production-level care.  
**Open where possible** — software, methods and outputs should be reusable whenever legal, ethical and methodological constraints allow it.

## Collaborate

GSLHub is open to collaboration with researchers, developers, universities, AI practitioners and organizations interested in Generative Search, GEO, AI evaluation and reproducible research.

**Website:** [gslhub.com](https://gslhub.com)  
**Research:** [github.com/gslhub/research](https://github.com/gslhub/research)  
**Benchmarks:** [github.com/gslhub/benchmarks](https://github.com/gslhub/benchmarks)  
**Software:** [github.com/gslhub/software](https://github.com/gslhub/software)  
**Email:** [research@gslhub.com](mailto:research@gslhub.com)

---

## Español

**GSLHub — Generative Search Lab Hub** es una iniciativa independiente de investigación e infraestructura tecnológica abierta centrada en comprender cómo los sistemas de IA generativa **descubren, seleccionan, citan y recomiendan información**.

La metodología científica se mantiene en [`gslhub/research`](https://github.com/gslhub/research), las especificaciones reproducibles en [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks), las implementaciones reutilizables en [`gslhub/software`](https://github.com/gslhub/software), la documentación transversal en [`gslhub/docs`](https://github.com/gslhub/docs) y la plataforma tecnológica en [`gslhub/website`](https://github.com/gslhub/website).

La documentación metodológica y de benchmark original se publica bajo **CC BY 4.0** salvo indicación contraria; la plataforma y el software original utilizan **AGPL-3.0-only** y la identidad visual se gestiona de forma separada en [`gslhub/branding`](https://github.com/gslhub/branding).

📍 Barcelona, España · 🌐 [gslhub.com](https://gslhub.com) · ✉️ [research@gslhub.com](mailto:research@gslhub.com)

<div align="center">

**Open research · Reproducible evidence · Applied AI**

</div>
