---
saneId: "SANE-001"
title: "The AV Abbreviation: Orthography for Professional Audiovisual Work"
description: "Establishes 'AV' (without slash) as the standard abbreviation for 'audiovisual' in all professional AV documentation, labeling, and digital systems."
status: "under-review"
version: "0.9"
pubDate: 2026-07-02
authors: ["SANE Community"]
tags: ["orthography", "abbreviation", "documentation", "labeling", "naming"]
category: "Documentation"
type: "practice"
maintainer: "SANE AV"
updates: []
obsoletes: []
---

## Abstract

This document defines the correct written abbreviation for "audiovisual" in professional AV work: **AV** (two capital letters, no slash, no hyphen). The forms "A/V" and "A-V" are prohibited in all formal AV documentation, labeling, filenames, drawings, system configurations, database fields, and programmatic identifiers.

## Status of This Memo

Under review. This standard is in its public review period. Feedback and proposed changes should be submitted through the SANE project repository.

---

## 1. Standard at a Glance

### 1.1 What This Standard Is About

This standard defines the correct written abbreviation for "audiovisual" in professional AV engineering work: **AV**: two capital letters, no slash, no hyphen, no punctuation.

### 1.2 Why It Matters

The form "A/V" creates avoidable technical and editorial problems in professional AV documentation. The forward slash is a reserved or syntactically meaningful character in file paths, URLs, many identifiers, and many data-processing contexts. Its presence in an abbreviation creates avoidable problems in filenames, repositories, URLs, database keys, search indexes, and programmatic tools. Beyond the technical problems, the slash incorrectly implies an either/or relationship ("audio or visual"), whereas the field is defined by the integration of both.

The "A-V" hyphenated form is also incorrect: "audiovisual" is a single compound word in standard English, not a hyphenated construction.

This standard eliminates the problem at its source: **AV** is the single correct abbreviation for every document, label, filename, and digital record in professional AV work.

### 1.3 Core Rules

- The abbreviation for "audiovisual" MUST be written as **AV**.
- The form **A/V** (with forward slash) MUST NOT be used in any formal AV documentation, label, filename, drawing, system configuration, database field, or programmatic identifier.
- The form **A-V** (with hyphen) MUST NOT be used as a substitute for the abbreviation.
- When writing the full term, the compound word **audiovisual** MUST be used, not "audio-visual" or "audio/visual."
- Existing legacy systems using "A/V" SHOULD be updated during the next scheduled maintenance or revision cycle.

### 1.4 Compliance Snapshot

| Question | Answer |
|----------|--------|
| What must be present? | The abbreviation "AV" where the term "audiovisual" is abbreviated |
| What must match? | All project documents, labels, filenames, drawings, configuration files, and data records |
| What must be verified? | No slash character in audiovisual abbreviations across all project deliverables |
| What must be documented? | Any legacy exceptions and their remediation plan |
| What would clearly fail? | Use of "A/V" as an abbreviation for "audiovisual" in a new or revised professional AV deliverable |

### 1.5 Who Should Read This

- **Designers** should review the Documentation Requirements section.
- **Installers** should review the Labeling Requirements section.
- **Programmers and DSP engineers** should review the Filename and Identifier Requirements section.
- **Service technicians** should review the Field Notes section and Appendix A.
- **Project managers** should review the Compliance section.

---

## 2. Scope

### 2.1 In Scope

- All professional AV system documentation: drawings, schedules, specifications, reports, commissioning documents, and handoff packages.
- All physical labels: rack labels, cable labels, equipment labels, patch panel designations, and signage.
- All filenames: CAD files, DSP configuration files, control system project files, firmware packages, and archived documentation.
- All digital systems: database fields, software identifiers, configuration keys, API endpoints, search indices, and content management systems.
- All project communications: emails, proposals, change orders, meeting minutes, and RFCs.
- All phases of project work: design, installation, programming, commissioning, service, and long-term maintenance.

### 2.2 Out of Scope

- The spoken pronunciation of "AV" (pronounced as the letters "A-V").
- Non-English abbreviations for "audiovisual" unless the target language uses the Latin alphabet in AV system documentation.
- Informal communication where no professional or contractual obligation to follow standards exists (personal notes, instant messaging).
- Manufacturer model numbers and proprietary product names that include "A/V" as part of a registered trademark or published part number; these are exempt from this standard but SHOULD be noted as exceptions when they appear in formal documentation (see the Exceptions section).

---

## 3. Definitions

**Audiovisual**: The standard English compound word referring to material, systems, or technology involving both sound and visual components. First known use in English: 1902 [Merriam-Webster, 2026].

**AV**: The standard two-letter initialism for "audiovisual." Written in capital letters, no periods, no slash, no hyphen. Pronounced as the letters "A-V."

**A/V**: A non-standard variant of the AV abbreviation that includes a forward slash. Prohibited by this standard in all formal AV documentation, labeling, and digital systems.

**A-V**: A non-standard variant of the AV abbreviation that includes a hyphen. Prohibited by this standard.

**Initialism**: An abbreviation formed from the initial letters of a compound term, pronounced as individual letters (e.g., "AV," "HDMI," "DSP"). Distinguished from an acronym, which is pronounced as a word.

---

## 4. Requirements

> **Requirement language:** This document uses **MUST**, **MUST NOT**, **SHOULD**, **SHOULD NOT**, and **MAY** per BCP 14, RFC 2119, and RFC 8174. Reserve MUST for safety, interoperability, or functional failures.

### 4.1 General Requirements

1. In formal professional AV deliverables, the abbreviation for "audiovisual" MUST be written as **AV**.
2. The forms **A/V** and **A-V** MUST NOT be used as abbreviations for "audiovisual" in new or revised formal professional AV deliverables.
3. When the full term is used, it SHOULD be written as **audiovisual**: one word, no hyphen, no slash.
4. When defining the abbreviation at first use, documents SHOULD use the form **audiovisual (AV)**.

### 4.2 Capitalization

1. The abbreviation "AV" MUST appear in capital letters in human-facing documentation, drawings, labels, filenames, schedules, and formal project records.
2. When "AV" appears as part of a compound term or prefix (e.g., "AV-over-IP," "AV rack," "AV system"), the "AV" component MUST remain capitalized.
3. In programming contexts where lowercase or mixed-case identifiers are required by local coding style, the letters "av" MAY appear as part of an identifier (e.g., `avInput`, `av_mute_state`, `avRouteTable`), provided the slash and hyphen forms are not used.
4. When the full word "audiovisual" appears at the beginning of a sentence, it follows standard sentence capitalization.

### 4.3 Documentation Requirements

The following document types MUST use "AV" and MUST NOT use "A/V" or "A-V":

1. **Drawings:** System line diagrams, signal flow diagrams, rack elevations, reflected ceiling plans, and floor plans. Every occurrence of the abbreviation (in title blocks, notes, equipment labels, signal designations, and detail callouts) MUST use "AV."
2. **Schedules:** Equipment schedules, cable schedules, I/O lists, and device inventories. Column headers and cell values containing the abbreviation MUST use "AV."
3. **Specifications:** Written specifications, scopes of work, and basis-of-design documents.
4. **Commissioning reports:** Test results, verification checklists, and punch lists.
5. **Handoff documentation:** As-built drawings, operations manuals, and owner training materials.

### 4.4 Labeling Requirements

1. All physical labels affixed to AV equipment, racks, cables, patch panels, wall plates, floor boxes, and junction boxes MUST use "AV" and MUST NOT use "A/V" or "A-V."
2. Multi-line labels MAY use the full word "AUDIOVISUAL" when space permits, but the abbreviation, when used, MUST be "AV."

### 4.5 Filename and Identifier Requirements

1. All AV project filenames MUST use "AV" and MUST NOT use "A/V." The slash character is an illegal filename character on all major operating systems (Windows, macOS, Linux). Any filename containing "A/V" will be rejected by the file system or will cause unpredictable behavior in file-management tools.
2. All software identifiers (DSP device names, control system object names, database keys, variable names, and API endpoints) MUST use "AV" and MUST NOT use "A/V" or "A-V."

### 4.6 Prohibited Practices

1. The form **A/V** MUST NOT appear in any new or revised professional AV deliverable.
2. The form **A-V** MUST NOT be used as a substitute for "AV."
3. The lowercase form "av" SHOULD NOT be used in human-facing formal AV documentation. It MAY be used in software identifiers where required by coding convention (see §4.2).
4. Mixing forms within the same document, project, or system (e.g., using "AV" in drawings but "A/V" in labels) MUST NOT occur.

### 4.7 Recommended Practices

1. Organizations SHOULD adopt this standard in their internal style guides, drawing templates, and label-printing software defaults.
2. Organizations SHOULD include a brief compliance note in project specifications referencing SANE-001.
3. When encountering legacy "A/V" labels, drawings, or configurations during service work, technicians SHOULD note the non-compliance and recommend remediation during the next scheduled maintenance.
4. Project templates and master document files SHOULD be updated to use "AV" so that new projects inherit the correct form by default.

---

## 5. Compliance

### 5.1 Compliance Requirements

A document, label set, drawing package, software configuration, or project deliverable claiming compliance with SANE-001 shall:

1. Contain no instances of "A/V" or "A-V" as an abbreviation for "audiovisual."
2. Use "AV" consistently in every location where the term "audiovisual" is abbreviated.
3. Use "audiovisual" (one word, no hyphen) consistently where the term is written in full.
4. Not mix abbreviation forms within the same deliverable or project.

### 5.2 Compliance Evidence

Evidence of compliance may include:

- Review of drawing title blocks, notes, and labels for slash or hyphen characters in the abbreviation.
- Spot-check of equipment labels and cable labels on site.
- Automated text search of project documentation (e.g., `grep -r "A/V"` across a document directory returning zero results).
- Review of DSP and control system configuration files for illegal or mixed abbreviation forms.
- Audit of filename conventions used in the project file repository.

### 5.3 Non-Compliance

The following conditions make a deliverable non-compliant:

1. Any occurrence of "A/V" on a drawing, label, schedule, or formal document.
2. Any occurrence of "A-V" used as the abbreviation for "audiovisual."
3. Mixed forms within a single project or document set.
4. Use of lowercase "av" as an abbreviation for "audiovisual" in human-facing formal documentation.
5. Filenames containing the slash character in the AV abbreviation position, regardless of whether the file system permitted the name: the intent is non-compliant.
6. A claim of compliance that cannot be verified against any written abbreviation, filename, label, or identifier is outside the scope of this standard.

---

## 6. Examples

### Example: Compliant drawing title block

```
ACME CONFERENCE CENTER
AV SYSTEM SIGNAL FLOW DIAGRAM
AV OVER-IP DISTRIBUTION, LEVEL 2
Drawn by: J. Smith | Date: 2026-03-15
```

All instances use "AV" consistently. The abbreviation is capitalized and contains no slash.

### Example: Compliant rack label

```
AV RACK 03
AV-OVER-IP SWITCH A
```

### Example: Compliant DSP object names

```
AV_Conf_Room_1_Program_L
AV_Conf_Room_1_Mic_1_In
AV_Lobby_Display_Control
```

These identifiers use "AV" as a prefix component with underscores as separators. They are valid in all file systems, databases, and programming environments.

### Example: Non-compliant drawing

```
ACME CONFERENCE CENTER
A/V SYSTEM SIGNAL FLOW DIAGRAM
```

The drawing uses "A/V"; non-compliant with SANE-001.

### Example: Non-compliant mixture within a project

- Drawing set uses "AV" ✓
- Equipment schedule uses "A/V" ✗
- Cable labels use "AV" ✓
- DSP configuration uses "A-V" ✗

The project is non-compliant due to mixed and incorrect forms. Both the "A/V" and "A-V" instances must be corrected.

---

## 7. Field Notes

- **CAD block libraries:** Many manufacturers ship CAD blocks with "A/V" in the block name or title. These SHOULD be renamed or annotated during project setup. Updating the master block library once prevents repeated non-compliance across projects.
- **Label printers:** Some label-printer software templates include "A/V" in default text fields. Templates SHOULD be updated at the organizational level.
- **Existing installations:** When servicing an existing system that uses "A/V" labels, do not replace labels solely for compliance with this standard. Note the non-compliance in the service report and remediate during the next scheduled upgrade.
- **Manufacturer product names:** Some products have "A/V" embedded in the manufacturer's model number (e.g., "ABC-A/V-SW4"). These are exempt (see the Exceptions section), but when the product is entered into an equipment schedule or project document, the surrounding text MUST follow this standard. The model number is treated as a proper noun, not an industry abbreviation.
- **Specification reuse:** When reusing specification text from a previous project, search for "A/V" and replace with "AV" before issuing. A single uncaught instance in a specification section can create ambiguity about which form governs.
- **Legacy shop drawings:** Subcontractor submittals may use "A/V" out of habit. Return submittals marked for correction if they will become part of the formal project record.

---

## 8. Safety, Security, and Privacy Considerations

This document defines an orthographic convention for written abbreviations. It introduces no technical requirements for AV systems and has no safety, security, or privacy considerations.

---

## 9. Exceptions

Exceptions to this standard MUST be documented and approved. A documented exception shall include:

1. The specific requirement being excepted.
2. The reason for the exception.
3. The alternate form being used and its scope of application.
4. The person or role approving the exception.
5. The date of approval.

**Permitted exceptions:**

- **Registered trademarks and product model numbers:** If a manufacturer's registered product name or model number includes "A/V" (e.g., as published in their official catalog or spec sheet), that string MAY appear verbatim in equipment schedules and procurement documents. This exception applies only to the specific product identifier, not to surrounding text, column headers, or general descriptions.
- **Direct quotation of legacy documents:** When quoting a historical document verbatim for archival, legal, or research purposes, the original form MAY be preserved.

Exceptions MUST NOT be used to avoid compliance on new work. Every new project that claims SANE-001 compliance MUST follow this standard regardless of legacy conventions at the organization.

---

## 10. Relationship to Other Standards

- This standard is independent. It does not modify, extend, or depend on any other SANE standard.
- This standard is consistent with editorial conventions used by the professional AV industry's primary trade association, AVIXA (Audiovisual and Integrated Experience Association) [AVIXA, 2026].
- This standard aligns with the orthographic guidance of standard English dictionaries: "audiovisual" is a single compound word [Merriam-Webster, 2026] [Wikipedia, 2026].
- This standard aligns with file-system constraints common to all major operating systems, where the forward slash (`/`) is a reserved character that cannot appear in filenames.

When this standard conflicts with an owner's published internal standards, contract documents, or an authority having jurisdiction, the higher authority governs. If the governing document mandates "A/V," the project documentation SHOULD note the deviation from SANE-001 and, where permitted by contract, include a recommendation to adopt the SANE-001 form in future revisions.

---

## 11. References

### 11.1 Normative References

**[RFC2119]** Bradner, S., "Key words for use in RFCs to Indicate Requirement Levels", BCP 14, RFC 2119, March 1997. <https://www.rfc-editor.org/rfc/rfc2119>

**[RFC8174]** Leiba, B., "Ambiguity of Uppercase vs Lowercase in RFC 2119 Key Words", BCP 14, RFC 8174, May 2017. <https://www.rfc-editor.org/rfc/rfc8174>

### 11.2 Informative References

- **Merriam-Webster.** "Audiovisual." *Merriam-Webster.com Dictionary.* Accessed July 2026. https://www.merriam-webster.com/dictionary/audiovisual
- **Wikipedia contributors.** "Audiovisual." *Wikipedia, The Free Encyclopedia.* Accessed July 2026. https://en.wikipedia.org/wiki/Audiovisual
- **AVIXA.** "About AVIXA." *AVIXA.org.* Accessed July 2026. https://www.avixa.org/about-avixa
- **Allen, William H.** (1975). "Intellectual Abilities and Instructional Media Design." *AV Communication Review*, 23(2), 139–170. <https://www.jstor.org/stable/30217831>

---

## Appendix A: Extended Guidance

### Legacy system remediation

When remediating a legacy installation that uses "A/V" throughout:

1. **Prioritize digital assets first:** Filenames and configuration files are the highest priority because they cause the most direct technical problems. Slashes in filenames can corrupt backup routines, break version control, and prevent cross-platform file sharing.
2. **Update drawings during the next revision:** Do not reissue drawings solely for abbreviation changes, but update all instances of "A/V" when drawings are revised for other reasons.
3. **Replace physical labels during upgrades:** When equipment is replaced or racks are reconfigured, replace adjacent "A/V" labels with "AV" labels at that time.
4. **Document the transition:** Maintain a brief log of which systems, drawings, and documents have been updated and which remain as legacy. This prevents duplicated effort and gives service technicians a clear picture of what they will encounter on site.

### Search-and-replace guidance

When updating documents programmatically, use word-boundary-aware search patterns to avoid false positives. For example, replacing all instances of "/" indiscriminately will corrupt dates (e.g., "01/15/2026") and other legitimate slash uses. Target the specific patterns "A/V" and "A-V" within the abbreviation context.

---

## Appendix B: Rationale

### Why the slash is incorrect

The forward slash (`/`) in "A/V" does not serve any editorial function that is consistent with English usage of the slash.

In standard English abbreviation conventions, the slash appears in a small set of specific contexts:
- To mean "per" (e.g., "km/h," "$450/week")
- To mean "or" (e.g., "and/or")
- In a few fixed abbreviations where the slash represents omitted letters (e.g., "n/a" for "not applicable," "w/o" for "without," "c/o" for "care of")

"A/V" fits none of these patterns. The slash does not mean "per," it does not mean "or" (the field is audio *and* visual, not audio *or* visual), and it does not represent omitted letters; "audiovisual" is a single word, not two words joined by missing text.

The slash form likely originates from the convention of using a stroke between two single-letter abbreviations (as in "I/O" for "input/output"). But "audio" and "visual" are not independent concepts being joined; they form the single concept "audiovisual," which the English language has treated as a single word since 1902.

### Why the hyphen is incorrect

The hyphenated form "A-V" is incorrect because "audiovisual" is not a hyphenated compound in standard English. Merriam-Webster lists it as a single word without a hyphen. The hyphen suggests two separate words being temporarily joined, which misrepresents the term.

### Industry precedent

The professional AV industry's primary trade association, AVIXA, consistently presents its name and public identity using "AV" and "Audiovisual" rather than "A/V."

The academic literature has used "AV" since at least the 1970s (see Allen, 1975, in the journal *AV Communication Review*).

### Practical impact

The slash in "A/V" is not a theoretical concern. The slash is a reserved character that breaks:
- **Filenames** on Windows, macOS, and Linux
- **URLs** (interpreted as path separator)
- **Database keys** and query strings
- **Search indices** and full-text search
- **Programming language identifiers**
- **Regular expression patterns**

Every professional AV practitioner who has tried to name a file "A/V System Diagram.pdf" has encountered this problem. The standard eliminates the issue at its source.

---

## Appendix C: Revision History

| Version | Date | Notes |
|---------|------|-------|
| 0.9 | 2026-07-02 | Initial publication as under-review. |
