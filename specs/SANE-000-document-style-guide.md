---
saneId: "SANE-000"
title: "SANE Document Style Guide"
description: "Style, structure, and authoring requirements for SANE standards documents."
status: "draft"
version: "0.8"
pubDate: 2026-07-02
authors: ["SANE Community"]
tags: ["meta", "style", "template"]
category: "meta"
type: "practice"
maintainer: "SANE AV"
updates: []
obsoletes: []
---

## Abstract

This document defines the structure, style conventions, and authoring requirements for SANE standards documents. It is the normative reference for anyone preparing a SANE document for publication, and provides a reusable template in Appendix A.

## Status of This Memo

Draft. This document is under active development and may change before publication. Feedback and proposed changes should be submitted through the SANE project repository.

---

## Table of Contents

- [1. Standard at a Glance](#1-standard-at-a-glance)
- [2. Scope](#2-scope)
- [3. Document Categories](#3-document-categories)
- [4. Document Structure](#4-document-structure)
- [5. Requirement Language](#5-requirement-language)
- [6. Style Conventions](#6-style-conventions)
- [7. Safety, Security, and Privacy Considerations](#7-safety-security-and-privacy-considerations)
- [8. Compliance](#8-compliance)
- [9. Relationship to Other Standards](#9-relationship-to-other-standards)
- [10. References](#10-references)
- [Appendix A: Standard Template](#appendix-a-standard-template)
- [Appendix B: Subsection Patterns for the Requirements Section](#appendix-b-subsection-patterns-for-the-requirements-section)
- [Appendix C: Rationale](#appendix-c-rationale)
- [Appendix D: Revision History](#appendix-d-revision-history)

---

## 1. Standard at a Glance

### 1.1 What This Standard Is About

This standard defines how all SANE documents must be structured and written. It is the house style guide for the SANE document series.

### 1.2 Why It Matters

Inconsistently structured standards slow adoption. A designer reviewing a SANE document should immediately find the requirements; a commissioning agent should find the compliance criteria; a service technician should find the field guidance. Without consistent structure, readers spend time learning the document's layout instead of its content.

This guide also defines when and how requirement language (MUST/SHOULD/MAY) should be used. Overusing MUST (applying mandatory language to preferences rather than real failures) erodes the word's meaning across the entire body of work.

### 1.3 Core Rules

- Every SANE document SHOULD include a "Standard at a Glance" section. `specification` and `practice` documents MUST include one.
- Every SANE document MUST identify a document category from the allowed set (see Document Categories).
- MUST and MUST NOT are reserved for safety, interoperability, serviceability, or functional correctness failures.
- `specification` and `practice` documents MUST include a Safety, Security, and Privacy Considerations section, or explicitly state that none apply.
- `informational` documents MUST NOT use BCP 14 requirement language.

### 1.4 Compliance Snapshot

| Question | Answer |
|----------|--------|
| What must be present? | Abstract, Status of This Memo, Scope, valid `type` field; Standard at a Glance for specification and practice documents |
| What must match? | Core Rules must summarize content already in the Requirements section; `type` must be an allowed category value |
| What must be verified? | Each requirement in the Requirements section is numbered and testable; no authoring notes remain in published text |
| What must be documented? | Category, status, version, and all required front matter fields |
| What would clearly fail? | Missing required sections, MUST used for preferences, authoring notes left in a published document |

---

## 2. Scope

This document applies to all published SANE documents: specifications, practices, terminology documents, reference documents, and informational documents.

This document defines:
- required and optional front matter fields;
- the normal section order and the purpose of each section;
- when to include or omit optional sections based on document category;
- requirement language usage;
- style conventions for writing clear professional AV documents.

This document does not define:
- the technical requirements of any AV system;
- the review or ratification process;
- project contracts, legal terms, or licensing;
- any AV-specific technical conventions.

---

## 3. Document Categories

Every SANE document MUST identify exactly one document category in its `type` front matter field.

| Category | Use when the document... |
|---|---|
| `specification` | defines measurable technical requirements: signal levels, timing, connector pinouts, dimensions, interoperability behavior |
| `practice` | defines a repeatable method or workflow: labeling, naming, commissioning, documentation, handoff |
| `terminology` | defines terms, names, concepts, or controlled vocabulary |
| `reference` | provides lookup tables, conversions, or reference data |
| `informational` | explains a topic, surveys practice, records rationale, or explores an area where SANE is not yet ready to make requirements |

A document SHOULD use the lightest category that fits the work. A document that only explains a topic SHOULD NOT be published as a `specification`. Section requirements per category are defined in the Document Structure section below.

---

## 4. Document Structure

A SANE document MUST follow the section order below. Sections marked **Required** must appear. **Recommended** sections should appear unless genuinely not applicable. **Optional** sections may be kept or removed. A dash (—) means the section must not appear for that document type.

| Section | `specification` | `practice` | `terminology` | `reference` | `informational` |
|---|---|---|---|---|---|
| Front Matter | **Required** | **Required** | **Required** | **Required** | **Required** |
| Abstract | **Required** | **Required** | **Required** | **Required** | **Required** |
| Status of This Memo | **Required** | **Required** | **Required** | **Required** | **Required** |
| Standard at a Glance | **Required** | **Required** | *Recommended* | *Recommended* | *Recommended* |
| Scope | **Required** | **Required** | **Required** | *Recommended* | *Recommended* |
| Definitions | *Recommended* | *Recommended* | **Required** | Optional | Optional |
| Requirements | **Required** | **Required** | **Required** | Optional | — |
| Compliance | **Required** | **Required** | **Required** | Optional | — |
| Examples | ***Strongly Recommended*** | ***Strongly Recommended*** | ***Strongly Recommended*** | Optional | Optional |
| Field Notes | Optional | Optional | Optional | Optional | Optional |
| Safety, Security, and Privacy Considerations | **Required** | **Required** | Optional | Optional | Optional |
| Exceptions | Optional | Optional | Optional | Optional | Optional |
| Relationship to Other Standards | *Recommended* | *Recommended* | *Recommended* | Optional | Optional |
| References | *Recommended* | *Recommended* | *Recommended* | Optional | Optional |
| Acknowledgements | Optional | Optional | Optional | Optional | Optional |
| Appendices | Optional | Optional | Optional | Optional | Optional |
| Revision History | Optional | Optional | Optional | Optional | Optional |

### 4.1 Front Matter

Required fields: `saneId`, `title`, `description`, `status`, `version`, `pubDate`, `authors`, `category`, `type`, `maintainer`.

Optional fields: `tags`, `updates`, `obsoletes`, `supersededBy`, `related`.

`status` MUST be one of: `draft`, `under-review`, `published`, `deprecated`, `superseded`. `type` MUST be one of the categories defined in Document Categories. `category` is the AV subject area (e.g., Documentation, Audio, Video, Control, Networking).

### 4.2 Abstract

Short and self-contained. Summarizes what the document does and who it is for. Appears in indexes and search results; MUST be complete in isolation. MUST NOT contain citations, unresolved placeholders, or context that only makes sense inside the document.

### 4.3 Status of This Memo

States the lifecycle stage: draft, under-review, published, deprecated, or superseded. SHOULD say where feedback and errata are tracked.

### 4.4 Standard at a Glance

SANE's primary practitioner-facing entry point. A Standard at a Glance section MUST summarize the document in a practitioner-facing way. It SHOULD include what the standard is about, why it matters, core rules or key points, and a compliance snapshot.

Short-form documents (informational documents, simple reference tables, or brief terminology entries) MAY use a simplified form. When a document is short enough that a separate Abstract and Standard at a Glance would repeat the same content, the two sections MAY be combined.

For full-length specification and practice documents, the Standard at a Glance SHOULD include the following subsections:
- **What This Standard Is About**: one paragraph, plain language.
- **Why It Matters**: the practical problem this standard solves. If the rationale is extensive, summarize here and expand in Appendix B.
- **Core Rules**: bullet-point summary of 3–5 requirements or key findings. For `informational` documents, rename this "Key Points."
- **Compliance Snapshot**: the five-question pass/fail table. Adapt for non-normative document types.

| Question | Answer |
|----------|--------|
| What must be present? | |
| What must match? | |
| What must be verified? | |
| What must be documented? | |
| What would clearly fail? | |

### 4.5 Scope

Two subsections: **In Scope** (bullet list of what this document covers) and **Out of Scope** (what it explicitly does NOT cover). AV topics overlap heavily; being explicit prevents misapplication. Reference other SANE documents or external standards where applicable.

### 4.6 Definitions

Define terms used in a specific or non-obvious way. Skip common industry knowledge. For `terminology` documents, this section is the primary deliverable. Format: **Term**: Definition. Omit the section entirely if no special terminology is introduced; do not publish an empty section.

### 4.7 Requirements

Number each requirement so it can be cited during review, commissioning, and issue tracking. Requirements must be testable by a reviewer who did not write the document.

- **Vague:** *"Labels should be clear."*
- **Testable:** *"Each cable label MUST include the source device, destination device, and signal type."*

Organize into named subsections. Common patterns include organizing by artifact, role, phase, topic, or requirement strength (see SANE-000 Appendix B for details). Add a one-sentence rationale inline where helpful: *(why: a slash in a filename is illegal on all major operating systems)*.

> **Requirement language:** Documents using BCP 14 requirement language MUST include the requirement-language boilerplate defined in the Requirement Language section. `informational` documents MUST NOT use BCP 14 requirement language.

### 4.8 Compliance

Define what conformance means. Must be objective: pass/fail without guessing intent.

- **Specification** documents need auditable criteria with measurable thresholds.
- **Practice** and **terminology** documents often need only: *"All project deliverables consistently apply these conventions."*
- **Reference** and **informational** documents may omit this section.

Subsections: Compliance Requirements `[Required]`, Compliance Evidence `[Optional]`, Non-Compliance `[Optional]`.

### 4.9 Examples

Show the standard applied to real AV work. Each example MUST explain why it passes, fails, or requires judgment. Standards without examples are harder to adopt: practitioners need to see the rule applied, not just stated. Move extended examples to Appendix A rather than bloating this section.

### 4.10 Field Notes

SANE's most distinctive section. Practical guidance from real AV work: design habits, installation practice, commissioning tips, service implications, legacy systems, and differences between drawings and field conditions. Field notes are informative unless they explicitly use MUST or SHOULD.

Do not use Field Notes to introduce requirements; those belong in the Requirements section.

### 4.11 Safety, Security, and Privacy Considerations

`specification` and `practice` documents MUST include this section. If none of safety, security, or privacy is relevant, state it directly: *"This document has no safety, security, or privacy considerations."* Do not omit the section.

AV-relevant topics: electrical hazards, structural loads, rigging, fire and emergency systems, high SPL, network exposure, access control, privacy, recording, camera placement, room occupancy data, signage analytics, and operational misuse.

### 4.12 Exceptions

How approved deviations from requirements are documented. A documented exception must include: the requirement being excepted, the reason, the alternate method, the approving role, and the date of approval. Exceptions MUST NOT be used to avoid safety, code, or contractual requirements. Omit this section if no exceptions are possible or if exceptions are handled inline within the requirements.

### 4.13 Relationship to Other Standards

How this document interacts with other SANE documents, public standards, codes, manufacturer documentation, or contract documents. State whether this document extends, complements, or is independent of each. When this document conflicts with law, code, or an authority having jurisdiction, the higher authority governs.

### 4.14 References

Split into Normative References and Informative References when both are present. Omit if no citations exist. Do not publish an empty References section.

### 4.15 Acknowledgements, Appendices, Revision History

Acknowledgements: credit contributors who provided feedback, review, or field testing. One sentence per contributor.

Appendices: for extended examples, rationale, migration guidance, legacy notes, or supporting material. Informative unless explicitly stated normative. Label A, B, C.

Revision History: human-readable summary of changes between published versions. The canonical record is the git log.

---

## 5. Requirement Language

The key words **MUST**, **MUST NOT**, **REQUIRED**, **SHOULD**, **SHOULD NOT**, **RECOMMENDED**, **MAY**, and **OPTIONAL** in SANE documents are interpreted as described in BCP 14 [RFC2119] [RFC8174] when, and only when, they appear in all capitals.

Use these terms sparingly. Reserve **MUST** and **MUST NOT** for requirements affecting safety, interoperability, serviceability, or functional correctness. Use **SHOULD** when practitioners can reasonably deviate with documented justification. Use **MAY** for genuinely optional behaviors with no strong preference.

`informational` documents MUST NOT use BCP 14 requirement language.

Requirement language SHOULD appear only in the Requirements section, the Compliance section, the Safety, Security, and Privacy Considerations section, or other sections explicitly identified as normative. Examples, rationale, and appendices should avoid requirement language unless the document explicitly marks a section as normative.

---

## 6. Style Conventions

Write for a working AV professional: a designer, installer, programmer, commissioning agent, or service technician.

**Do:**
- Use short sentences.
- Define terms before relying on them.
- Use the same term for the same concept throughout.
- Write requirements as testable statements.
- Separate requirements from rationale and examples.
- Use tables when they make comparison or lookup easier.
- Keep examples realistic to professional AV work.

**Avoid:**
- Using a requirement to express a preference.
- Hiding safety or code implications in casual notes.
- Relying on "clear," "proper," "reasonable," or "best practice" without defining those words in context.
- Publishing empty sections.
- Leaving authoring instructions in a ratified document.
- Vendor-specific language unless intentional.

Spelling and punctuation MUST be internally consistent within a document. SANE documents SHOULD use American English.

---

## 7. Safety, Security, and Privacy Considerations

This document defines structure and style conventions and introduces no technical requirements for AV systems. It has no safety, security, or privacy considerations.

---

## 8. Compliance

A SANE document conforms to this style guide when:

1. the `type` field identifies a valid category from Document Categories;
2. all required front matter fields are present and non-empty;
3. the Abstract and Status of This Memo sections are present;
4. the Standard at a Glance section is present when required for the document category, and is self-contained when included;
5. the Scope section is present when required for the document category, and identifies what is and is not covered when included;
6. requirement language follows the Requirement Language section;
7. all requirements are numbered and testable;
8. `specification` and `practice` documents include Safety, Security, and Privacy Considerations or state that none apply;
9. normative and informative references are separated when both are present;
10. no authoring instructions remain in the published document.

---

## 9. Relationship to Other Standards

This document is the normative style foundation for the SANE document series. All SANE documents must conform to it.

SANE documents adopt the requirement language defined in RFC 2119 and RFC 8174, and follow the general approach to document structure described in RFC 7322, adapted for the AV industry. SANE documents are not part of the IETF publication process.

When any SANE document conflicts with law, code, contract documents, or an authority having jurisdiction, the higher authority governs.

---

## 10. References

### 10.1 Normative References

**[RFC2119]** Bradner, S., "Key words for use in RFCs to Indicate Requirement Levels", BCP 14, RFC 2119, March 1997. <https://www.rfc-editor.org/rfc/rfc2119>

**[RFC8174]** Leiba, B., "Ambiguity of Uppercase vs Lowercase in RFC 2119 Key Words", BCP 14, RFC 8174, May 2017. <https://www.rfc-editor.org/rfc/rfc8174>

### 10.2 Informative References

**[RFC7322]** Flanagan, H. and Ginoza, S., "RFC Style Guide", RFC 7322, September 2014. <https://www.rfc-editor.org/rfc/rfc7322>

---

## Acknowledgements

The structure of this document is informed by RFC 7322 and the IETF RFC publication model.

---

## Appendix A: Standard Template

Copy this template when starting a new SANE document. Replace all placeholder text. Delete all instructional comments before publication.

````markdown
---
saneId: "SANE-___"
title: "Document Title"
description: "One-sentence description of what this document defines."
status: "draft"
version: "0.1"
pubDate: YYYY-MM-DD
authors: ["Author Name"]
tags: []
category: ""
type: ""
maintainer: "SANE AV"
updates: []
obsoletes: []
---

## Abstract

This document defines ...

## Status of This Memo

Draft. Feedback and proposed changes should be submitted via the SANE project repository.

---

## Table of Contents

- [1. Standard at a Glance](#1-standard-at-a-glance)
- [2. Scope](#2-scope)
- [3. Definitions](#3-definitions)
- [4. Requirements](#4-requirements)
- [5. Compliance](#5-compliance)
- [6. Examples](#6-examples)
- [7. Field Notes](#7-field-notes)
- [8. Safety, Security, and Privacy Considerations](#8-safety-security-and-privacy-considerations)
- [9. Relationship to Other Standards](#9-relationship-to-other-standards)
- [10. References](#10-references)

---

## 1. Standard at a Glance

### 1.1 What This Standard Is About

This standard defines how [subject] should be [action] in professional AV systems.

### 1.2 Why It Matters

[Describe the practical problem this standard solves.]

### 1.3 Core Rules

- [Most important rule or finding.]
- [Second.]
- [Third.]

### 1.4 Compliance Snapshot

| Question | Answer |
|----------|--------|
| What must be present? | |
| What must match? | |
| What must be verified? | |
| What must be documented? | |
| What would clearly fail? | |

### 1.5 Who Should Read This

- **Designers** should review the [Requirements](#4-requirements) section.
- **Installers** should review the [Requirements](#4-requirements) section.
- **Programmers and DSP engineers** should review the [Requirements](#4-requirements) section.
- **Service technicians** should review the [Field Notes](#7-field-notes) section.
- **Project managers** should review the [Compliance](#5-compliance) section. |

---

## 2. Scope

### 2.1 In Scope

- ...

### 2.2 Out of Scope

- ...

---

## 3. Definitions

**Term**: Definition.

---

## 4. Requirements

> **Requirement language:** This document uses **MUST**, **MUST NOT**, **SHOULD**, **SHOULD NOT**, and **MAY** per BCP 14, RFC 2119, and RFC 8174. Reserve MUST for safety, interoperability, or functional failures.

### 4.1 [Subsection name]

1. [Requirement.] *(why: ...)*
2. [Requirement.]

---

## 5. Compliance

### 5.1 Compliance Requirements

A [deliverable/project/system] conforms to this document when:

1. ...

### 5.2 Compliance Evidence

[Optional.]

### 5.3 Non-Compliance

[Optional.]

---

## 6. Examples

### 6.1 Compliant Example

...

### 6.2 Non-Compliant Example

...

---

## 7. Field Notes

- [Practical guidance from real AV work.]

---

## 8. Safety, Security, and Privacy Considerations

[This document has no safety, security, or privacy considerations.] OR [Describe relevant considerations.]

---

## 9. Relationship to Other Standards

[This standard is independent.] OR [Describe relationships.]

---

## 10. References

### 10.1 Normative References

...

### 10.2 Informative References

...

---

## Acknowledgements

...

## Appendix A: Extended Guidance

...

## Appendix B: Rationale

...

## Appendix C: Revision History

| Version | Date | Notes |
|---------|------|-------|
| 0.1 | YYYY-MM-DD | Initial draft. |
````

---

## Appendix B: Subsection Patterns for the Requirements Section

These patterns are informative. Individual SANE documents may use them during drafting, but should not include this appendix in the published document unless it adds value to that specific standard.

| Pattern | Best when | Example subsection names |
|---------|-----------|--------------------------|
| By artifact | Different deliverable types have different requirements | Drawings, Labels, Filenames, Configuration Files |
| By role | Different practitioners have meaningfully different duties | Designer Requirements, Installer Requirements, Programmer Requirements |
| By phase | Requirements change at project stages | Design Phase, Installation Phase, Commissioning Phase |
| By topic | The standard covers distinct technical areas | Signal Levels, Connectors, Cabling, Documentation |
| By requirement strength | Clean separation of normative from advisory | Mandatory Requirements, Prohibited Practices, Recommended Practices |

---

## Appendix C: Rationale

SANE adopts the useful parts of RFC structure: stable identifiers, clear status, careful requirement language, separated references, mandatory safety, security, and privacy review, without the full IETF publication model.

The "Standard at a Glance" section is SANE's primary departure from the RFC model. An RFC Abstract is written for discovery; the Standard at a Glance is written for a practitioner who will use the standard in the field. Core Rules and the Compliance Snapshot give working AV professionals immediate value without requiring them to read the full document.

Field Notes is uniquely SANE. No major standards body has a dedicated section for field-tested practical wisdom. It captures what experienced practitioners carry in their heads from real installs and makes it part of the written record.

---

## Appendix D: Revision History

| Version | Date | Notes |
|---------|------|-------|
| 0.8 | 2026-07-02 | Working draft: RFC-style structure, document categories, section matrix, requirement language conventions, reusable template. |