# Radical World Ontology (JSON-LD)

This repository hosts the JSON-LD ontology for Life Functions, Levels, and Function×Level contexts used by rProtocols, Neobooks, and other apps.

## Structure
- `v1/context.jsonld` – JSON-LD context & vocabulary bindings
- `v1/lifefunctions.jsonld` – 20 canonical LifeFunction nodes
- `.nojekyll` – disables Jekyll processing on GitHub Pages

## Publish on GitHub Pages
1. Create a new GitHub repository (e.g., `radical-ontology`).
2. Push these files to the repo (default branch: `main`).
3. In **Settings → Pages**, choose **Deploy from a branch**: `main` / `/ (root)`. Save.
4. Your site will be live at `https://<user>.github.io/radical-ontology/`.
5. (Optional) Add a custom domain `ontology.radical.world` in **Settings → Pages**.
6. In your DNS, create a CNAME:
   - Host: `ontology`
   - Value: `<user>.github.io`
7. Back in GitHub Pages, enable **Enforce HTTPS** once the certificate is issued.

## Stable IRIs
- Context: `https://ontology.radical.world/v1/context.jsonld`
- Life Functions graph: `https://ontology.radical.world/v1/lifefunctions.jsonld`

## Versioning
Create new folders (`v2/`, etc.) for breaking changes; do not overwrite previous versions.
