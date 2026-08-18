<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/gslhub/website/main/public/brand/gslhub-logo-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/gslhub/website/main/public/brand/gslhub-logo.svg">
  <img src="https://raw.githubusercontent.com/gslhub/website/main/public/brand/gslhub-logo.svg" alt="GSLHub — Generative Search Lab Hub" width="360">
</picture>

# GSLHub

### Investigación aplicada independiente en Búsqueda Generativa, GEO, sistemas de IA e investigación reproducible

**Barcelona, España · Investigación abierta · Infraestructura open-source**

[English](./README.md) · **Español**

[Web](https://gslhub.com) · [Investigación](https://github.com/gslhub/research) · [Benchmarks](https://github.com/gslhub/benchmarks) · [Software](https://github.com/gslhub/software) · [Docs](https://github.com/gslhub/docs) · [Contacto](mailto:research@gslhub.com)

</div>

---

## Acerca de GSLHub

**GSLHub — Generative Search Lab Hub** es una iniciativa independiente de investigación y una infraestructura tecnológica abierta centrada en comprender cómo los sistemas de IA generativa descubren, seleccionan, citan y recomiendan información.

Nuestro trabajo combina **investigación en Búsqueda Generativa, Generative Engine Optimization (GEO), evaluación de sistemas de IA, evidencia gobernada, experimentación reproducible e ingeniería de software**.

El objetivo no es únicamente estudiar los sistemas generativos, sino construir la infraestructura necesaria para que esa investigación sea **auditable, repetible y útil en entornos reales**.

## Arquitectura de investigación

```text
Problema científico
→ Hipótesis
→ Experimento
→ Ejecución controlada
→ Artefacto de investigación preservado
→ Evidencia
→ Observación
→ Cita / Métrica
→ Revisión de reproducibilidad
→ Difusión pública
```

GSLHub trata las métricas como resultados de investigación trazables, no como números aislados. La metodología científica vive en [`gslhub/research`](https://github.com/gslhub/research), las especificaciones de benchmark en [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks), las implementaciones reutilizables en [`gslhub/software`](https://github.com/gslhub/software) y la plataforma operativa gobernada en [`gslhub/website`](https://github.com/gslhub/website).

## Repositorios públicos

### [`gslhub/website`](https://github.com/gslhub/website)

Web pública y plataforma principal de investigación para gobernanza de experimentos, ejecuciones controladas, procedencia de evidencias, métricas científicas, artefactos de investigación y controles de reproducibilidad.

**Stack:** `Next.js` · `TypeScript` · `React` · `Payload CMS` · `MongoDB` · `Tailwind CSS` · `Node.js` · `GitHub Actions`  
**Licencia:** `AGPL-3.0-only`

### [`gslhub/research`](https://github.com/gslhub/research)

Capa metodológica canónica con el modelo de investigación, protocolos, codebooks, gobernanza, requisitos de reproducibilidad y metadatos de citación.

**Licencia:** `CC BY 4.0` para documentación original de investigación salvo indicación contraria.

### [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks)

Benchmarks reproducibles y especificaciones métricas para Búsqueda Generativa y GEO. La baseline pública actual incluye **AIR, CR, MCP y RCR**, una definición machine-readable del benchmark y fixtures sintéticos de validación.

**Licencia:** `CC BY 4.0` para especificaciones y documentación originales del benchmark.

### [`gslhub/software`](https://github.com/gslhub/software)

Software de investigación reutilizable que implementa partes de la metodología GSLHub de forma independiente y testeable. El primer paquete, **`@gslhub/metrics-core` v0.1.0**, ofrece cálculos deterministas de AIR, CR, MCP y RCR independientes del framework, con exclusiones, numeradores/denominadores y checksums SHA-256 para auditoría.

**Stack:** `TypeScript` · `Node.js` · `npm workspaces` · `GitHub Actions`  
**Licencia:** `AGPL-3.0-only`

### [`gslhub/docs`](https://github.com/gslhub/docs)

Documentación técnica e institucional pública y transversal sobre arquitectura, límites entre repositorios, gobernanza y estándares de publicación segura.

**Licencia:** `CC BY 4.0` salvo indicación contraria.

### [`gslhub/branding`](https://github.com/gslhub/branding)

Identidad visual aprobada de GSLHub: variantes de logo claro/oscuro, icono, paleta y guía de uso de marca. Los derechos de marca se gestionan de forma separada a las licencias de software y documentación científica.

## Roadmap de repositorios

| Área | Estado | Propósito |
|---|---|---|
| [`website`](https://github.com/gslhub/website) | **Público** | Web pública y plataforma principal de investigación |
| [`research`](https://github.com/gslhub/research) | **Público** | Protocolos, metodología y codebooks canónicos |
| [`benchmarks`](https://github.com/gslhub/benchmarks) | **Público** | Marcos de evaluación y especificaciones métricas reproducibles |
| [`software`](https://github.com/gslhub/software) | **Público** | Software reutilizable y métricas deterministas |
| [`docs`](https://github.com/gslhub/docs) | **Público** | Documentación técnica e institucional |
| [`branding`](https://github.com/gslhub/branding) | **Público** | Identidad visual y guía de uso |
| **datasets** | En preparación | Releases de datasets revisados con licencia por release |

Los repositorios se abren progresivamente únicamente cuando su contenido está documentado, licenciado y preparado para reutilización pública.

## Familias métricas principales

| Código | Métrica | Pregunta principal |
|---|---|---|
| **AIR** | Answer Inclusion Rate | ¿Con qué frecuencia aparece visiblemente el target evaluado? |
| **CR** | Citation Rate | ¿Con qué frecuencia se cita explícitamente el target evaluado? |
| **MCP** | Mean Citation Position | Cuando se cita, ¿en qué posición aparece la primera cita válida? |
| **RCR** | Response Consistency Rate | ¿Qué estabilidad tienen las repeticiones controladas frente a una baseline congelada? |

Las especificaciones normativas se versionan en [`gslhub/benchmarks`](https://github.com/gslhub/benchmarks), mientras que las implementaciones deterministas reutilizables se versionan de forma independiente en [`gslhub/software`](https://github.com/gslhub/software). Esta separación permite validar los cálculos contra una especificación congelada sin acoplarlos a la base de datos o al CMS de la aplicación.

## Ciencia abierta y licencias

GSLHub aplica licencias según el tipo de resultado:

- **Plataforma de investigación y software original:** GNU AGPL-3.0-only, salvo que un paquete indique lo contrario.
- **Investigación original y documentación de benchmarks:** Creative Commons Attribution 4.0 International (CC BY 4.0), salvo indicación contraria.
- **Datasets:** licencia individual según procedencia, derechos y restricciones de investigación.
- **Publicaciones:** regidas por las condiciones de cada publicación o editorial.
- **Activos de marca y trademarks:** gestionados de forma separada.

## Principios

**Transparencia** — metodología y decisiones técnicas inspeccionables.  
**Reproducibilidad** — preservar el contexto necesario para repetir experimentos.  
**Basado en evidencia** — conclusiones trazables hasta evidencias preservadas.  
**Rigor técnico** — infraestructura de investigación diseñada con cuidado de nivel productivo.  
**Abierto cuando sea posible** — software, métodos y resultados reutilizables siempre que las restricciones legales, éticas y metodológicas lo permitan.

## Colaboración

GSLHub está abierto a colaborar con investigadores, desarrolladores, universidades, profesionales de IA y organizaciones interesadas en Búsqueda Generativa, GEO, evaluación de IA e investigación reproducible.

**Web:** [gslhub.com](https://gslhub.com)  
**Investigación:** [github.com/gslhub/research](https://github.com/gslhub/research)  
**Benchmarks:** [github.com/gslhub/benchmarks](https://github.com/gslhub/benchmarks)  
**Software:** [github.com/gslhub/software](https://github.com/gslhub/software)  
**Email:** [research@gslhub.com](mailto:research@gslhub.com)

---

<div align="center">

**Investigación abierta · Evidencia reproducible · IA aplicada**

</div>
