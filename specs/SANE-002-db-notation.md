---
saneId: "SANE-002"
title: "Decibel (dB) Notation for Professional AV Systems"
description: "Defines the correct written form of the decibel (dB) unit, its common suffixes, and prohibited variant forms in professional AV documentation, labeling, and digital systems."
status: "draft"
version: "0.8"
pubDate: 2026-07-02
authors: ["SANE Community"]
tags: ["notation", "units", "decibel", "audio", "acoustics", "documentation", "labeling"]
category: "Documentation"
type: "practice"
maintainer: "SANE AV"
updates: []
obsoletes: []
---

## Abstract

This document defines the correct written form of the decibel unit and its common professional AV suffixes. The forms `db`, `DB`, `Db`, and other case variants are prohibited in formal AV documentation. Absolute decibel values without a stated reference suffix are prohibited where the reference would not be clear from context.

## Status of This Memo

Draft. This standard is under active development and may change before publication. Feedback and proposed changes should be submitted through the SANE project repository.

---

## 1. Standard at a Glance

### 1.1 What This Standard Is About

This standard defines the correct written form for the decibel unit and its reference suffixes in professional AV documentation: **dB** (lowercase `d`, uppercase `B`, no space between them).

### 1.2 Why It Matters

The decibel expresses ratios on a logarithmic scale. Without a stated reference suffix, an absolute decibel value is ambiguous: -10 dB could mean -10 dBFS (digital full scale), -10 dBu (analog voltage), -10 dBV (consumer voltage), or -10 dB SPL (sound pressure). These represent wildly different quantities. Confusing them wastes time during commissioning, creates errors in gain structure, and can produce unsafe sound pressure levels.

The written form of the unit also suffers from persistent inconsistency across the industry. The correct form `dB` derives from the SI: `d` for deci (one-tenth) and `B` for Bel (named after Alexander Graham Bell). Forms such as `db`, `DB`, and `Db` violate SI conventions and look unprofessional in formal engineering documentation.

### 1.3 Core Rules

- The decibel unit MUST be written as **dB** (lowercase `d`, uppercase `B`, no space, no periods).
- The forms **db**, **DB**, **Db**, **DB.**, and any other case variants MUST NOT be used in formal AV documentation.
- When expressing an absolute level, the reference suffix MUST be present (e.g., `dB SPL`, `dBu`, `dBV`, `dBFS`, `dBm`, `dBA`) and MUST NOT be omitted if the reference would be unclear from context.
- The numerical value and the unit MUST be separated by a space (e.g., `85 dB SPL`, not `85dB SPL` or `85dBSPL`).

### 1.4 Compliance Snapshot

| Question | Answer |
|----------|--------|
| What must be present? | The unit `dB` (correct case); a reference suffix on absolute values where context does not make the reference obvious |
| What must match? | All documents, labels, drawings, DSP files, configuration files, and formal project records |
| What must be verified? | No lowercase `db`, uppercase `DB`, or mixed-case variant in any formal AV deliverable |
| What must be documented? | Any legacy configurations or labels using incorrect forms, with their remediation plan |
| What would clearly fail? | Use of `db`, `DB`, or `Db` in a new or revised professional AV deliverable; an absolute decibel value without a reference suffix |

### 1.5 Who Should Read This

- **Designers** should review the documentation and drawing requirements in the Requirements section.
- **DSP programmers** should review the configuration file requirements and the common suffixes table.
- **Installers** should review the labeling requirements.
- **Commissioning agents** should review the compliance criteria.
- **Service technicians** should review the Field Notes section.

---

## 2. Scope

### 2.1 In Scope

- All professional AV system documentation: drawings, schedules, specifications, reports, commissioning documents, and handoff packages.
- All physical labels: rack labels, equipment labels, metering legends, and signage.
- All digital systems: DSP configuration files, control system projects, audio processor presets, measurement system reports, and software identifiers.
- All phases of project work: design, installation, programming, commissioning, service, and long-term maintenance.

### 2.2 Out of Scope

- The spoken pronunciation of "dB."
- Mathematical derivations, formulas, or logarithmic properties of decibels.
- The engineering conventions for which reference suffix applies in a given context (e.g., when to use dBu vs dBV). This standard defines the form, not the application.
- Informal communication where no professional or contractual obligation to follow standards exists.

---

## 3. Definitions

**Decibel (dB)**: A logarithmic unit expressing the ratio of two quantities. The symbol `dB` is derived from the SI prefix `d` (deci, one-tenth) and the unit `B` (Bel), named after Alexander Graham Bell. Defined in IEC 60027-3 [IEC, 2002] and recognized by NIST and ISO.

**Reference suffix**: A letter or group of letters appended to `dB` indicating the reference value against which the ratio is computed. Common suffixes include `dB SPL`, `dBu`, `dBV`, `dBm`, `dBFS`, and `dBA`. Without a suffix, a decibel value expresses only a ratio, not an absolute level.

**Absolute level**: A decibel value stated with a reference suffix, representing a specific quantity relative to a fixed reference (e.g., `94 dB SPL` is an absolute sound pressure level; `+4 dBu` is an absolute voltage level).

**Relative level**: A decibel value stated without a reference suffix, representing only a ratio (e.g., "the amplifier provides 20 dB of gain").

**dB SPL**: Sound Pressure Level. Reference: 20 micropascals (µPa), the approximate threshold of human hearing. A root-power quantity; 20 dB increase = 10× pressure ratio.

**dBu**: Voltage level referenced to 0.775 V RMS (the voltage that dissipates 1 mW into a 600 Ω load). Standard for professional analog audio interconnects per SANE-001 (historical).

**dBV**: Voltage level referenced to 1.0 V RMS. Common in consumer and semi-professional equipment.

**dBFS**: Decibels relative to Full Scale. Used in digital audio systems. 0 dBFS is the maximum level before clipping; all valid signals are negative values.

**dBm**: Power level referenced to 1 milliwatt (mW).

**dBA or dB(A)**: A-weighted sound pressure level, applying a frequency weighting curve approximating human hearing sensitivity.

---

## 4. Requirements

> **Requirement language:** This document uses **MUST**, **MUST NOT**, **SHOULD**, **SHOULD NOT**, and **MAY** per BCP 14, RFC 2119, and RFC 8174. Reserve MUST for safety, interoperability, or functional failures.

### 4.1 General Requirements

1. In formal professional AV deliverables, the decibel unit MUST be written as **dB** (lowercase `d`, uppercase `B`, no space between the letters, no periods).
2. An absolute decibel value MUST include its reference suffix. The suffix MAY be omitted when the value expresses a relative ratio and the context makes this clear (e.g., "20 dB of gain," "attenuate by 6 dB").
3. A space MUST separate the numerical value from the unit (e.g., `94 dB SPL`). The suffix and the `dB` symbol SHOULD be separated by a space (e.g., `dB SPL`, `dB FS`), except for widely established single-block forms (`dBu`, `dBV`, `dBm`, `dBA`, `dBFS`).

### 4.2 Capitalization

1. The `d` in `dB` MUST always be lowercase. The `B` MUST always be uppercase.
2. The reference suffix follows its own capitalization rules per the defining standard (e.g., `SPL` is uppercase as an initialism; `u` in `dBu` is lowercase; `V` in `dBV` is uppercase as a volt symbol; `A` in `dBA` is uppercase as an A-weighting designation).
3. At the beginning of a sentence, the unit `dB` retains its case and is not capitalized.

### 4.3 Prohibited Forms

1. The form **db** (all lowercase) MUST NOT appear in any formal professional AV deliverable.
2. The form **DB** (all uppercase) MUST NOT appear in any formal professional AV deliverable.
3. The form **Db** (mixed case) MUST NOT appear in any formal professional AV deliverable.
4. The form **dB.** (with trailing period) MUST NOT appear.
5. Forms using a hyphen or other separator between `d` and `B` (`d-B`, `d.B`) MUST NOT appear.

### 4.4 Reference Suffix Requirements

1. When a decibel value expresses an absolute level, the reference suffix MUST be present (e.g., `94 dB SPL`, `+4 dBu`, `-20 dBFS`).
2. The reference suffix SHOULD use the form established by industry convention for that reference. Common forms are listed in the table below.
3. When the reference is ambiguous or multiple references are commonly used for the same signal type, the suffix MUST be included even if context might otherwise imply it.

| Suffix | Meaning | Common context |
|--------|---------|----------------|
| `dB SPL` | Sound pressure level (re 20 µPa) | Acoustics, room tuning, safety limits |
| `dBu` | Voltage (re 0.775 V) | Professional analog audio |
| `dBV` | Voltage (re 1.0 V) | Consumer / semi-pro audio |
| `dBm` | Power (re 1 mW) | RF, telecom, some audio |
| `dBFS` | Full scale (digital) | DSP, digital audio, DAW metering |
| `dBA` / `dB(A)` | A-weighted SPL | Environmental noise, safety compliance |

### 4.5 Documentation Requirements

The following document types MUST use `dB` and MUST NOT use prohibited forms:

1. **Drawings:** Title blocks, notes, signal designations, audio metering legends, and SPL coverage maps.
2. **Schedules:** Audio equipment schedules, DSP I/O lists, and gain structure tables.
3. **Specifications:** Performance specifications, acceptance criteria, and basis-of-design documents.
4. **Commissioning reports:** SPL measurements, gain structure verification, and signal-to-noise ratio test results.
5. **DSP configuration files:** Channel labels, meter references, gain stage values, and limiter thresholds.

### 4.6 Filename and Identifier Requirements

1. All AV project filenames containing a decibel reference MUST use `dB` (e.g., `Room_101_SPL_85dB_Reading.pdf`). Forms such as `db` or `DB` MUST NOT appear.
2. All software identifiers (DSP object names, control system variables, database fields) MUST use `dB` where the decibel unit is referenced.

### 4.7 Recommended Practices

1. Organizations SHOULD adopt this standard in their internal style guides, drawing templates, and DSP template files.
2. When documenting gain structure, designers SHOULD include the reference suffix on every decibel value (e.g., `+4 dBu` rather than `+4 dB`), even when the reference seems implied by context.
3. Measurement reports SHOULD state the reference and weighting explicitly on first use (e.g., "All SPL measurements are A-weighted relative to 20 µPa (dBA)").

---

## 5. Compliance

### 5.1 Compliance Requirements

A document, label set, drawing package, software configuration, or project deliverable claiming compliance with SANE-002 shall:

1. Contain no instances of `db`, `DB`, `Db`, or other prohibited case variants as the decibel unit.
2. Use `dB` consistently in every location where the decibel unit appears.
3. Include a reference suffix on every absolute decibel value where context does not make the reference obvious.
4. Not mix decibel unit forms within the same deliverable or project.

### 5.2 Compliance Evidence

Evidence of compliance may include:

- Review of drawing notes, DSP labels, and signal designations for incorrect case variants.
- Automated text search of project documentation (e.g., `grep -r "[Dd][Bb]"` across a document directory returning only valid forms).
- Review of DSP and control system configuration files for prohibited forms.
- Spot-check of physical labels and metering legends on site.
- Audit of measurement report conventions.

### 5.3 Non-Compliance

The following conditions make a deliverable non-compliant:

1. Any occurrence of `db`, `DB`, `Db`, or another prohibited form as the decibel unit.
2. An absolute decibel value without a reference suffix where the reference is not obvious from context.
3. Mixed forms within a single project or document set.
4. A claim of compliance that cannot be verified against any written decibel notation, label, filename, or identifier.

---

## 6. Examples

### Example: Compliant DSP channel labels

```
Input_01_Mic_L   +4 dBu nominal
Output_01_Zone_A  -6 dBFS headroom
SPL_Limit         94 dB SPL (A-weighted)
```

All values use `dB` with correct case. Absolute values include reference suffixes. Space between value and unit.

### Example: Compliant drawing note

```
ALL ANALOG AUDIO INTERCONNECTS SHALL OPERATE AT +4 dBu NOMINAL LEVEL WITH 20 dB OF HEADROOM.
```

Relative value `20 dB` omits suffix (ratio, context clear). Absolute value `+4 dBu` includes suffix.

### Example: Compliant measurement report

```
Test Point A: 85 dBA (1 kHz, slow response, 10 m from source)
```

### Example: Non-compliant DSP configuration

```
Input_01_Mic_L   +4 db
Output_01_Zone_A  -6 DB
SPL_Limit         94
```

All three lines are non-compliant: `db` (lowercase), `DB` (uppercase), and `94` without any unit.

### Example: Non-compliant drawing

```
SPEAKER COVERAGE TARGET: 95 DB @ 1 kHz
```

`DB` is the prohibited uppercase form. Correct form: `95 dB SPL @ 1 kHz`.

### Example: Ambiguous decibel values (non-compliant if reference unclear)

```
Set limiter threshold to -6 dB.
```

Without context, `-6 dB` could mean -6 dBFS, -6 dBu, or -6 dB below an unspecified reference. If the context does not make the reference obvious (e.g., on a DSP limiter where dBFS is universally implied), this is non-compliant.

---

## 7. Field Notes

- **DSP software defaults:** Many DSP platforms use `dB` correctly in their user interface but may export configuration files or reports using `db`. Review exported files during commissioning and correct before including them in handoff documentation.
- **Measurement microphones:** SPL meter apps and handheld meters often label readings as `dBA` or `dB SPL`. These are correct. The problem arises when a technician transcribes readings by hand into a report and writes `94 db` out of habit. Templates with pre-filled unit columns prevent this.
- **Spreadsheet formatting:** Excel and similar tools may auto-correct `dB` to `Db` or apply unwanted capitalization. Lock the format of measurement columns to plain text or use data validation to restrict entries.
- **Existing installations:** When servicing a system that uses `db` or `DB` in DSP labels or documentation, note the non-compliance in the service report and remediate during the next scheduled maintenance window.
- **Audio console scribble strips:** Many digital consoles allow custom channel labeling. Labels such as `+4 db` are common. Correct these during soundcheck or commissioning.
- **Manufacturer specifications:** Some equipment spec sheets use non-standard forms. When transcribing specifications into project documentation, correct the form to `dB` and note the deviation in project notes.

---

## 8. Safety, Security, and Privacy Considerations

Incorrect or ambiguous decibel notation can contribute to unsafe sound pressure levels. A limiter threshold documented as `-6` without a reference could be misinterpreted, resulting in output levels significantly higher than intended. Similarly, an SPL target of `95 DB` written in a commissioning report is unambiguous to most AV professionals, but the incorrect unit form erodes documentation quality and may contribute to confusion in safety-critical contexts such as hearing conservation compliance (e.g., OSHA, NIOSH exposure limits).

This document introduces no security or privacy considerations.

---

## 9. Exceptions

Exceptions to this standard MUST be documented and approved. A documented exception shall include:

1. The specific requirement being excepted.
2. The reason for the exception.
3. The alternate form being used and its scope of application.
4. The person or role approving the exception.
5. The date of approval.

**Permitted exceptions:**

- **Direct quotation of legacy documents:** When quoting a historical document verbatim for archival, legal, or research purposes, the original form MAY be preserved.
- **Registered trademarks and product model numbers:** If a manufacturer's registered product name includes a non-standard decibel form (e.g., as part of a model number), that string MAY appear verbatim in equipment schedules.

Exceptions MUST NOT be used to avoid compliance on new work.

---

## 10. Relationship to Other Standards

- This standard is independent. It does not modify, extend, or depend on any other SANE standard.
- This standard adopts the unit symbol conventions defined in IEC 60027-3:2002 and the writing conventions of NIST SP 811, applied to professional AV documentation.
- This standard is consistent with SANE-001 (AV abbreviation) in establishing correct orthographic forms for terms commonly used in AV engineering.

When this standard conflicts with an owner's published internal standards, contract documents, or an authority having jurisdiction, the higher authority governs.

---

## 11. References

### 11.1 Normative References

**[RFC2119]** Bradner, S., "Key words for use in RFCs to Indicate Requirement Levels", BCP 14, RFC 2119, March 1997. <https://www.rfc-editor.org/rfc/rfc2119>

**[RFC8174]** Leiba, B., "Ambiguity of Uppercase vs Lowercase in RFC 2119 Key Words", BCP 14, RFC 8174, May 2017. <https://www.rfc-editor.org/rfc/rfc8174>

### 11.2 Informative References

- **IEC 60027-3:2002.** Letter symbols to be used in electrical technology — Part 3: Logarithmic and related quantities, and their units. International Electrotechnical Commission.
- **NIST SP 811.** Guide for the Use of the International System of Units (SI). National Institute of Standards and Technology. <https://www.nist.gov/pml/special-publication-811>
- **Wikipedia contributors.** "Decibel." *Wikipedia, The Free Encyclopedia.* Accessed July 2026. <https://en.wikipedia.org/wiki/Decibel>
- **NIOSH.** "Occupational Noise Exposure." DHHS (NIOSH) Publication No. 98-126. <https://www.cdc.gov/niosh/docs/98-126/>

---

## Appendix A: Extended Guidance

### Common measurement suffixes

The table below provides additional detail on suffixes encountered in AV work. This appendix is informative.

| Suffix | Quantity | Reference | Typical AV use |
|--------|----------|-----------|----------------|
| `dB SPL` | Sound pressure level | 20 µPa | Room acoustics, system tuning |
| `dB(A)` | A-weighted SPL | 20 µPa, A-weighted | Noise compliance, hearing safety |
| `dB(C)` | C-weighted SPL | 20 µPa, C-weighted | Low-frequency assessment |
| `dBu` | RMS voltage | 0.775 V | Professional analog audio |
| `dBV` | RMS voltage | 1.0 V | Consumer / semi-pro audio |
| `dBm` | Power | 1 mW | RF, telecom, legacy audio |
| `dBFS` | Amplitude (digital) | Full scale | DSP, DAW, digital consoles |
| `dBTP` | True peak (digital) | Full scale | Broadcast, streaming compliance |

### Quick reference: prohibited forms

| Prohibited | Correct | Reason |
|------------|---------|--------|
| `db` | `dB` | deci is lowercase `d`, Bel is uppercase `B` |
| `DB` | `dB` | deci is lowercase `d`, not uppercase |
| `Db` | `dB` | deci precedes the unit name |
| `db SPL` | `dB SPL` | unit case error |
| `DBSPL` | `dB SPL` | case error, missing space |
| `dbu` | `dBu` | unit case error |
| `d.b.` | `dB` | periods not used with unit symbols |

---

## Appendix B: Rationale

### Why lower case d, upper case B

The decibel is a compound unit: the prefix "deci" (one-tenth, symbol `d`) combined with the unit "Bel" (symbol `B`). Per the International System of Units (SI), prefix symbols for factors less than 10^6 are written in lower case. Unit symbols derived from a person's name are written with an upper case first letter. The decibel follows both rules: `d` is the lowercase prefix for 10^-1, `B` is the uppercase symbol for Bel (Alexander Graham Bell).

### Why a space between the number and unit

Per NIST SP 811, a space separates the numerical value from the unit symbol in all SI and SI-recognized units. The decibel follows this convention: `94 dB SPL`, not `94dB SPL`.

### Why reference suffixes matter

The decibel is fundamentally a ratio. Stating `-10 dB` tells the reader nothing about the absolute quantity unless the reference is known. In professional AV, the same numeric value can represent radically different conditions:

- `-10 dBFS` — a digital signal with 10 dB of headroom (clean)
- `-10 dBu` — a very low analog level (near noise floor)
- `-10 dB SPL` — well below the threshold of human hearing

In a DSP configuration file where the context might not be visible (e.g., an exported preset reviewed by a different engineer), the ambiguity is a real source of commissioning errors and service delays.

---

## Appendix C: Revision History

| Version | Date | Notes |
|---------|------|-------|
| 0.8 | 2026-07-02 | Initial draft. |
