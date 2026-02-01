# Void Fragment: Field Matcher

Matches fields between two systems based on semantic meaning, not hardcoded rules.

---

## Purpose

When integrating two systems, mapping fields is often manual, repetitive, and error-prone.  
Field Matcher answers: “Which target field means the same thing as this input field?”

---

## Inputs / Outputs

**Inputs**
- One input field:
  - `fieldHandle` (required)
  - `fieldLabel` (required)
  - `fieldType` (required)
  - `fieldDescription` (optional)
- A list of target fields with the same attributes

**Outputs**
- Top matching target fields with similarity scores
- Best match plus confidence information for inspection

---

## Guarantees

- No hardcoded mapping rules
- Runs locally (no external API required)
- Designed to be inspectable: returns top matches and scores, not just a single guess

---

## Typical usage

- ERP ↔ ecommerce schema mapping
- CMS ↔ PIM / warehouse field alignment
- Integration tooling where naming conventions are inconsistent
- Reducing the effort of initial schema discovery and normalization

---

## Repository

https://github.com/OpsDevHub/void-fragment--field-matcher
