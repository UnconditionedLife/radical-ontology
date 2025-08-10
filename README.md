# Radical World Ontology (JSON-LD)

The **Radical World Ontology** is the public, versioned, machine-readable vocabulary that underpins multiple Radical World projects — including **rProtocols**, **Neobooks**, and future life-aligned collaboration tools.

It provides a shared language for describing **Life Functions**, **Levels of Organization**, and the **function×level contexts** that help align Needs, Protocols, and knowledge content with the living processes they serve.

---

## 📂 Contents

### Current (v1)
- [`v1/context.jsonld`](https://unconditionedlife.github.io/radical-ontology/v1/context.jsonld)  
  The JSON-LD `@context` defining namespaces, prefixes, and core term mappings.
  
- [`v1/lifefunctions.jsonld`](https://unconditionedlife.github.io/radical-ontology/v1/lifefunctions.jsonld)  
  The 20 core Life Functions — generalized from James G. Miller’s *Living Systems Theory* functions — with IRIs, definitions, canonical descriptions, and aliases.

### Planned
- `v1/levels.jsonld`  
  Levels of organization from subatomic to planetary, with canonical names, descriptions, and related functions.

- `v1/fxlevel.jsonld`  
  Cross-mapped Life Function × Level contexts, giving each function level-specific language and examples.

---

## 🛠 How to Use

Reference the ontology in your JSON-LD, RDF, or other linked-data aware systems:

```json
{
  "@context": "https://unconditionedlife.github.io/radical-ontology/v1/context.jsonld",
  "@type": "rad:LifeFunction",
  "@id": "https://ontology.radical.world/lifefunction/integrating-signals",
  "rdfs:label": "Integrating Signals",
  "schema:description": "Aggregating and coordinating incoming information..."
}
```json
---

**Notes**
- Use `name` and `description` (mapped in the context to `schema:name` and `schema:description`).  
- `alias` maps to `skos:altLabel`.  
- IRIs are stable and versioned via the folder (`/v1/`). For breaking changes, publish `/v2/` rather than mutating `/v1/`.

---

## Versioning & changes

- `v1/` is intended to remain stable.  
- Breaking changes will be published under a new version directory (`v2/`, `v3/`, …).  
- Clarifications/typo fixes that don’t change meaning may be applied in place.

---

## Contributing

Improvements and additions are welcome via pull request.  
Please propose changes with clear rationale and, when possible, examples of usage across Needs/Protocols.

---

**Maintainer:** Radical World  
**Project home:** https://radical.world
