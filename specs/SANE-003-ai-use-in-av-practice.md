---
saneId: "SANE-003"
title: "AI Use in Professional AV Practice"
description: "Defines recommended guidelines for AI use in professional AV practice, covering AI-generated text in communications and AI operational tools, with a focus on keeping human expertise and presence at the center of AV work."
status: "draft"
version: "0.1"
pubDate: 2026-07-05
authors: ["SANE Community"]
tags: ["communication", "ethics", "AI", "professional practice", "service", "sales"]
category: "Professional Practice"
type: "practice"
maintainer: "SANE AV"
updates: []
obsoletes: []
---

## Abstract

This document defines recommended guidelines for AI use in professional AV practice. **This is not an anti-AI document.** AI tools are powerful, increasingly capable, and a legitimate part of modern AV work. This standard defines where they help, where they require oversight, and where human authorship and human judgment are the professional standard.

Two categories of AI use are addressed: communication tools (text generation used in proposals, responses, service reports, and correspondence) and operational tools (AI systems that perform or assist with specific AV tasks such as network diagnostics, signal management, and automated commissioning). In both categories, the underlying principle is the same: AI is most valuable as an amplifier of human expertise, not a substitute for it. AV is a human-centered industry. Every system we build exists to serve a human experience, and the professional practices that support it should reflect that.

## Status of This Memo

Draft. This document is under active development and may change before publication. Feedback and proposed changes should be submitted through the SANE project repository.

---

## Table of Contents

- [1. Standard at a Glance](#1-standard-at-a-glance)
- [2. Scope](#2-scope)
- [3. Definitions](#3-definitions)
- [4. Requirements](#4-requirements)
  - [4.1 Client and Stakeholder Communications](#41-client-and-stakeholder-communications)
  - [4.2 Service Reports and Field Documentation](#42-service-reports-and-field-documentation)
  - [4.3 Technical Responses and Expert Opinion](#43-technical-responses-and-expert-opinion)
  - [4.4 Permitted Uses of AI Assistance](#44-permitted-uses-of-ai-assistance)
  - [4.5 AI Operational and Automation Tools](#45-ai-operational-and-automation-tools)
- [5. Compliance](#5-compliance)
- [6. Examples](#6-examples)
- [7. Field Notes](#7-field-notes)
- [8. Safety, Security, and Privacy Considerations](#8-safety-security-and-privacy-considerations)
- [9. Relationship to Other Standards](#9-relationship-to-other-standards)
- [10. References](#10-references)
- [Appendix A: Rationale](#appendix-a-rationale)
- [Appendix B: Revision History](#appendix-b-revision-history)

---

## 1. Standard at a Glance

### 1.1 What This Standard Is About

This standard defines recommended guidelines for AI use in professional AV practice. It covers two categories: AI communication tools (text generation in proposals, client correspondence, technical responses, and service reports) and AI operational tools (systems that perform or assist with specific AV tasks such as network diagnostics, signal management, or automated commissioning).

The standard defines when AI assistance adds genuine value, when it should be used with oversight, and where human authorship and human judgment remain the professional standard. It applies to all AV practitioners: designers, sales professionals, installers, programmers, commissioning agents, service technicians, and project managers.

### 1.2 Why It Matters

The audiovisual industry is fundamentally human-centered. Every system we design, install, and maintain exists to mediate human experience: a display a person looks at, a speaker a person hears, a conference system that connects people across distances. This relationship between AV technology and human experience is not incidental. It is the reason the industry exists.

AI tools are genuinely useful in professional AV work. They surface information quickly, assist with drafting and editing, automate repetitive tasks, and are increasingly capable of performing specific AV operations with real accuracy. Using them where they add value is not just acceptable. It is sensible. This standard is not a case against AI in professional AV. It is a framework for using it well.

**Knowledge is not the same as execution.** AI tools can retrieve high-level information, general theory, and documented procedures faster than most humans. What they cannot do is replicate the accumulated judgment of a practitioner who has run a thousand cable pulls, commissioned a hundred DSP systems, or built a client relationship over years. That expertise lives in the practitioner. When a client or colleague seeks out a specific person for advice, they are seeking that execution-level knowledge, not a retrieval of general information. Knowing the theory of acoustic echo cancellation is not the same as knowing how to tune it in a difficult room. The value of the expert is in their trained, contextual judgment.

AI text generation tools are now widely available and can produce fluent prose on any topic in seconds. The business case for using them is obvious. The professional cost is less visible but real.

**AV is a technical language industry.** The terms, conventions, and precision of AV engineering do not map cleanly onto general knowledge. When a client or colleague receives an AI-generated response to an AV question, the quality of the answer reflects what a language model trained on general text can approximate, not what an experienced AV practitioner actually knows. The unique knowledge that makes an expert valuable is exactly what gets flattened out.

**Relationships drive the industry.** AV work runs on trust built over time between people. Proposals, service reports, and ongoing correspondence are how practitioners demonstrate their thinking and build that trust. When a client discovers that an expert they rely on is sending AI-generated text, the relationship changes. The expert's voice, and with it their credibility, is called into question.

**Service is personal.** A service technician arrives on site, solves a problem, and then sends a report. The report and the person are two parts of the same experience. A service report that does not sound like the person who was in the room misrepresents the engagement and degrades the value of it.

### 1.3 Core Rules

- Direct professional communications to clients and stakeholders SHOULD be written by the practitioner in their own voice.
- Service reports SHOULD reflect the technician's actual observations, written in their own words.
- AI tools MAY be used for boilerplate administrative copy, internal drafts, search assistance, and template generation.
- AI-generated text MUST NOT be submitted as the practitioner's own expert opinion or technical analysis without substantive review and revision.
- Practitioners responding to technical questions from clients or colleagues SHOULD provide their own answer rather than forwarding unreviewed AI-generated output.
- AI operational tools (diagnostics, automated signal management, commissioning aids) MAY be used to assist AV work, but their outputs SHOULD be reviewed by a qualified practitioner before being acted upon or delivered to a client.
- AI operational tools SHOULD NOT be deployed in ways that remove the human craft and presence from the AV experience.

### 1.4 Compliance Snapshot

| Question | Answer |
|---|---|
| What must be present? | Human-authored content in client-facing proposals, technical responses, and service reports |
| What must match? | The communication should reflect the practitioner's actual knowledge, voice, and observations |
| What must be verified? | Not formally verifiable; compliance is a matter of professional conduct and organizational culture |
| What must be documented? | Where AI tools contributed substantially to a deliverable, the practitioner SHOULD personally review and attest to its accuracy |
| What would clearly fail? | Sending AI-generated responses to technical questions without reading them; service reports that do not reflect the technician's actual observations |

### 1.5 Who Should Read This

- **Sales professionals** should review [Section 4.1](#41-client-and-stakeholder-communications).
- **Service technicians** should review [Section 4.2](#42-service-reports-and-field-documentation).
- **Designers and engineers** should review [Section 4.3](#43-technical-responses-and-expert-opinion).
- **Project managers** should review [Section 4.4](#44-permitted-uses-of-ai-assistance) and the [Field Notes](#7-field-notes).
- **Integrators and system programmers** should review [Section 4.5](#45-ai-operational-and-automation-tools).

---

## 2. Scope

### 2.1 In Scope

- Professional communications sent by AV practitioners to clients, colleagues, or other stakeholders in a professional context.
- Proposals, quotations, scope of work documents, and RFP responses.
- Service reports, field observation notes, and commissioning documentation.
- Email correspondence and written responses to technical questions in a professional context.
- Any written work product where the practitioner's expertise, judgment, or voice is implicit in the communication.
- AI-powered operational tools used in the delivery, commissioning, or servicing of AV systems, including automated diagnostics, signal management systems, and AI-driven commissioning aids.

### 2.2 Out of Scope

- Internal tooling, scripts, or automation that generates machine-readable output.
- Marketing copy, advertising, or public-facing website text where AI assistance is widely understood and expected.
- AI-powered search, document summarization, or knowledge retrieval used to help a practitioner form their own answer.
- Software, DSP configurations, control system programming, or any technical output not intended as direct human communication.
- Communications that explicitly disclose AI generation to the recipient.

---

## 3. Definitions

**AI-generated text**: Text produced primarily by a large language model or similar AI system, where the AI's output constitutes the substance of the communication rather than assisting the practitioner in forming their own.

**Authentic communication**: Written communication whose substance, reasoning, and voice originate from the practitioner, even if tools were used to assist with grammar, spelling, or formatting.

**Service report**: A written record produced by a field technician or commissioning agent documenting work performed, observations made, and actions taken during a service visit or commissioning engagement.

**Expert opinion**: A written response to a technical question where the practitioner's knowledge, experience, or professional judgment is the implicit basis for the answer.

**Boilerplate copy**: Standardized administrative or legal text, such as terms and conditions, warranty language, or standard scope language, that does not represent the practitioner's individual voice or expertise.

**AI operational tool**: An AI-powered system designed to perform or assist with a specific AV task: network diagnostics, automated signal path verification, fault detection, room correction, or similar functions. Distinguished from general-purpose AI text generation by its task-specific design and direct integration with AV systems or workflows.

---

## 4. Requirements

The key words **MUST**, **MUST NOT**, **SHOULD**, **SHOULD NOT**, and **MAY** in this section are interpreted as described in BCP 14 [RFC2119] [RFC8174] when they appear in all capitals.

### 4.1 Client and Stakeholder Communications

**R-4.1.1** The substantive sections of proposals, quotations, and scope of work documents, including technical approach, system design rationale, scope definition, and pricing rationale, SHOULD reflect the practitioner's own understanding and SHOULD be authored or substantively revised by the practitioner before submission. *(why: this content is a statement of how the practitioner understands the problem and intends to solve it; that understanding is the service being sold)*

**R-4.1.2** Routine sections of proposals, such as company background, cover letter language, standard introduction paragraphs, and administrative terms, MAY be AI-generated and require only practitioner review before submission.

**R-4.1.3** Written responses to client questions, technical or otherwise, SHOULD reflect the practitioner's own answer. *(why: the client is seeking the practitioner's knowledge, not a language model's approximation of it)*

**R-4.1.4** When AI tools assist in drafting a client communication, the practitioner SHOULD review the output for technical accuracy, appropriate professional tone, and fidelity to their actual position before sending.

**R-4.1.5** AI-generated text MUST NOT be submitted to a client as the practitioner's expert technical opinion without the practitioner reading and attesting to its accuracy.

### 4.2 Service Reports and Field Documentation

**R-4.2.1** Service reports SHOULD be written in the service technician's own words, reflecting their actual observations and actions during the engagement. *(why: the report and the technician are two parts of the same service experience; a disconnect between them degrades the value of both)*

**R-4.2.2** Observations recorded in a service report SHOULD be based on what the technician actually observed, not AI-generated summaries of what typically occurs in a given scenario.

**R-4.2.3** Commissioning documentation and punch list items SHOULD reflect the commissioning agent's own findings, written clearly and accurately.

### 4.3 Technical Responses and Expert Opinion

**R-4.3.1** When a colleague, client, or stakeholder asks a practitioner a technical question, the practitioner SHOULD answer from their own knowledge. *(why: AV technical knowledge is specialized, contextual, and hard for general language models to approximate accurately; the human expert is sought out precisely because of what they know)*

**R-4.3.2** Forwarding an AI-generated response to a technical question SHOULD NOT substitute for the practitioner's own answer unless the AI output has been read, verified for technical accuracy, and revised to reflect the practitioner's actual position.

**R-4.3.3** Practitioners SHOULD NOT represent AI-generated content as their own original analysis or expert judgment.

### 4.4 Permitted Uses of AI Assistance

**R-4.4.1** AI tools MAY be used to generate or assist with boilerplate administrative copy, standard terms and conditions, and template language. *(why: this text does not represent the practitioner's individual voice or expertise)*

**R-4.4.2** AI-powered search, document retrieval, and summarization tools MAY be used to help a practitioner research and form their own answer.

**R-4.4.3** AI tools MAY be used to assist with grammar checking, spell checking, and formatting of practitioner-authored text.

**R-4.4.4** AI tools MAY assist in generating initial internal drafts that the practitioner substantially revises before the content becomes a professional communication.

### 4.5 AI Operational and Automation Tools

**R-4.5.1** AI operational tools MAY be used to assist with network diagnostics, signal path verification, fault detection, automated room correction, and other task-specific AV functions. *(why: these tools can surface problems faster and more completely than manual inspection in many cases, and their use is appropriate)*

**R-4.5.2** The output of an AI operational tool SHOULD be reviewed by a qualified practitioner before being acted upon or communicated to a client. *(why: AI diagnostic and automation tools can produce incorrect results, particularly in non-standard configurations; the practitioner is accountable for the outcome regardless of which tool surfaced it)*

**R-4.5.3** When an AI operational tool produces a finding, recommendation, or automated action that will affect a client's system, the practitioner SHOULD verify the result makes sense given their knowledge of the system. *(why: a tool that correctly identifies a problem in 95% of cases will still produce wrong outputs; the practitioner's contextual knowledge is the check on that)*

**R-4.5.4** AI operational tools SHOULD NOT be used as a substitute for practitioner presence, inspection, or judgment where that presence and judgment are part of what the client is receiving. *(why: the value of professional AV service includes the practitioner's eyes, ears, and experience in the room, not only the corrective action taken)*

**R-4.5.5** AI automation that performs tasks previously requiring a practitioner SHOULD be disclosed to the client when the client's expectation is that a practitioner performed the work. *(why: clients make decisions about service relationships based on what they believe they are receiving)*

---

## 5. Compliance

### 5.1 Compliance Requirements

This standard defines professional conduct norms. Unlike technical specifications, compliance cannot be verified by automated inspection. Conformance is a matter of professional practice and organizational culture.

A practitioner meets this standard when:

1. Proposals, quotations, and client communications reflect the practitioner's own understanding of the project and proposed solution.
2. Service reports are written by the attending technician and reflect their actual observations and actions.
3. Technical responses to questions are based on the practitioner's own knowledge, or are reviewed and revised by the practitioner before submission.
4. AI assistance is confined to permitted tasks: boilerplate, formatting, search, and internal drafts.
5. AI operational tool outputs are reviewed by the practitioner before being acted upon or delivered.

### 5.2 Non-Compliance

Non-compliant practices include:

- Sending AI-generated text to a client as the practitioner's expert answer to a technical question without reading it.
- Submitting a service report that does not reflect what the attending technician actually observed or did.
- Representing AI-generated analysis as the practitioner's own professional judgment.
- Acting on AI operational tool outputs without practitioner review when those outputs affect a client's system.
- Using AI automation in a way that removes the human experience from a service engagement without disclosing this to the client.

---

## 6. Examples

### 6.1 Permitted: AI assists with boilerplate administrative text

A project manager uses an AI tool to generate a standard terms and conditions attachment for a proposal. The AI produces legal and administrative boilerplate language. The project manager reviews it and attaches it to a proposal whose scope of work, pricing rationale, and technical approach were written by the practitioner.

**Result: Compliant.** The administrative boilerplate is not the practitioner's individual voice or expertise. The substantive content of the proposal remains human-authored.

### 6.2 Permitted: AI helps research an answer

A designer is asked about the signal loss for a long cable run. They use an AI tool to quickly surface reference values, then verify the figures against the manufacturer's specification sheet, and write their own response explaining the calculation.

**Result: Compliant.** The AI was used as a research and retrieval aid. The practitioner formed and wrote their own answer.

### 6.3 Non-compliant: AI answers a client's technical question

A client emails a sales engineer asking why their videoconferencing system has echo. The engineer pastes the email into a chatbot, copies the response, and forwards it to the client without reading it.

**Result: Non-compliant.** The client asked the engineer for their expert knowledge. The engineer sent a language model's output without verifying its technical accuracy or relevance to this client's specific system. The client is receiving the engineer's name attached to advice the engineer never reviewed.

### 6.4 Non-compliant: AI writes a service report

A service technician completes a service call and asks an AI chatbot to write their service report from a few bullet points. The AI produces a fluent, detailed report. The technician submits it without reviewing it carefully.

**Result: Non-compliant.** The service report is part of the service experience. A client who had a good interaction with the technician in person, and then reads a report that does not sound like that person, experiences a disconnect that reduces the perceived quality of the engagement. If the report contains inaccurate details, which AI can introduce, the technician has submitted incorrect documentation without knowing it.

### 6.5 Requires judgment: AI assists in drafting a complex proposal

A lead designer uses an AI tool to draft the narrative sections of a large proposal. They substantially revise every section to reflect their actual design decisions, rationale, and understanding of the client's needs. The technical specifications and system design remain entirely their own.

**Result: Likely compliant, depending on the degree of revision.** If the final text reflects the designer's actual understanding and voice, the AI assistance functioned as a drafting tool rather than a substitute for the practitioner's contribution. If the final text is mostly AI-generated narrative with minimal revision, it trends toward non-compliance.

### 6.6 Permitted: AI diagnostic tool identifies a network AV problem

A commissioning engineer uses an AI-powered network AV diagnostic tool that identifies a bandwidth congestion issue causing video dropouts. The tool surfaces the problem and suggests a QoS configuration change. The engineer reviews the recommendation, confirms it is appropriate for this network, makes the change, and verifies the system is stable.

**Result: Compliant.** The AI tool was used as an efficient diagnostic aid. The practitioner reviewed the output, applied their knowledge of the specific system, and was accountable for the result.

### 6.7 Non-compliant: AI automation replaces a service visit without disclosure

A service firm deploys an AI tool that automatically detects and corrects common AV issues remotely. A client calls reporting a problem, the AI resolves it in the background, and the firm sends a service report describing the resolution as if a technician had reviewed and resolved it manually.

**Result: Non-compliant.** The resolution itself may have been technically correct. The problem is that the client was led to believe a practitioner reviewed their system when none did. The client's decision to continue paying for managed service is based in part on that expectation.

---

## 7. Field Notes

### On AV as a human-centered industry

Every AV system exists to mediate a human experience. The display someone looks at, the speaker someone hears, the microphone that carries their voice: these are not abstract technical objects. They serve real people in real moments, and the professionals who design and maintain them earn their position by understanding those human contexts. The same logic applies to communication: the proposals, reports, and responses that practitioners send are themselves a human experience for the people receiving them.

### On why AI approximates AV knowledge poorly

AV is a field built on specialized, precise, and sometimes counterintuitive technical language. The correct answer to an AV question often depends on context that a language model cannot see: the room acoustics, the equipment model, the control system version, the client's actual use pattern. A fluent AI response to an AV question often sounds authoritative while being wrong in ways that an experienced practitioner would immediately recognize. When a practitioner forwards that response to a client, they are lending their name and credibility to advice they have not checked.

This problem is not hypothetical. AV clients and colleagues ask questions precisely because they trust the person they are asking. They are not asking for a general answer from a general source. They are asking for this person's answer, based on this system, in this building. AI tools are not equipped to provide that.

### On service technicians and the service experience

Service technicians build a specific kind of professional relationship with the clients they regularly visit. They know the system, the room, and often the people who work there. The service report is the written record of that visit. When a service report is generated by AI and does not reflect the technician's actual voice and observations, it is not just an impersonal document. It is a small misrepresentation of who was in the room and what they actually found.

The personality and competence that make a service technician good at their job are not visible on-site alone. They are communicated in every interaction, including the written ones.

### On communication as a competitive differentiator

In a field where many technical outcomes are similar between qualified firms, communication quality is often the actual differentiator. The practitioner who writes a clear, specific, and honest proposal stands out from one who sends a generic AI-generated response. The service technician whose reports are brief, accurate, and written in their own voice demonstrates competence more effectively than any AI-polished prose. The investment of time required to write one's own communications in this industry is small relative to the professional return.

### On expertise versus knowledge

AI tools are very good at surfacing information. They are not good at the thing that makes an experienced AV practitioner valuable: knowing what to do with it. The difference between knowing that a room's RT60 is too long and knowing how to treat it given the ceiling height, the wall materials, the budget, and the client's aesthetic preferences is the difference between a lookup and a career. That execution-level judgment is what clients and colleagues are paying for. AI tools surface information. Practitioners apply it.

This matters practically because AI responses to technical questions often sound complete and authoritative even when they are missing the contextual judgment that would make them actually useful. A practitioner who forwards that response is not saving time. They are lending their name to advice that has not been filtered by their expertise.

### On AI operational tools and the human experience of AV

A new category of AI tools is emerging specifically for AV work: systems that diagnose network AV problems, automate signal path verification, correct room acoustics, and perform tasks that previously required a practitioner to be present and engaged. Many of these tools are genuinely impressive and will change how AV work is done.

The concern is not their capability. It is their deployment. AV is fundamentally about human experience. A well-tuned room, a reliable conference system, a display that looks right: these are not just technical outcomes. They are the result of a practitioner who cared about the result. When AI automation is deployed in ways that remove that human presence from the experience, clients lose something real, even if they cannot always name it. The goal is to use AI operational tools to make practitioners more capable and present, not to replace them.

### On legitimate AI assistance

This standard is not a rejection of AI tools. AI-powered search helps practitioners find answers faster. Tools that assist with document editing, grammar, and draft generation are part of modern professional work. AI operational tools that surface problems faster than manual inspection save time and catch issues that might otherwise be missed. The distinction is between tools that make practitioners more capable and tools that replace the practitioner's contribution without acknowledgment. The former is unremarkable and welcome. The latter is the practice this standard addresses.

---

## 8. Safety, Security, and Privacy Considerations

### 8.1 Privacy

Client communications and service reports often contain confidential information: system configurations, access credentials, room layouts, organizational structures, and security-relevant details. Practitioners MUST NOT paste client-confidential information into third-party AI tools without verifying that doing so is consistent with their data handling obligations and any applicable confidentiality agreements.

### 8.2 Security

AI-generated text submitted without careful review creates a risk of inadvertently confirming, disclosing, or misrepresenting technical details that should not be shared. Practitioners SHOULD NOT use AI tools to draft responses to questions involving security-sensitive system configurations without carefully reviewing the output for unintended disclosures.

### 8.3 Professional Risk

Submitting AI-generated technical content as one's own expert opinion without verification creates professional risk if the content is inaccurate. In the context of system design, safety systems, or access control, technically inaccurate advice can have consequences that extend beyond the professional relationship.

---

## 9. Relationship to Other Standards

This standard is independent of other SANE documents and introduces no technical requirements for AV systems.

Future SANE documents addressing commissioning records, service documentation formats, or handoff packages may reference this standard for authorship requirements applicable to those records.

---

## 10. References

### Normative References

- [RFC2119] Bradner, S., "Key words for use in RFCs to Indicate Requirement Levels," BCP 14, RFC 2119, March 1997.
- [RFC8174] Leiba, B., "Ambiguity of Uppercase vs Lowercase in RFC 2119 Key Words," BCP 14, RFC 8174, May 2017.

### Informative References

None.

---

## Appendix A: Rationale

### Why This Standard Exists

This document emerged from a recognized pattern in the professional AV industry: the increasing use of AI text generation tools in professional communications, at the cost of authentic practitioner voice, and the parallel emergence of AI operational tools that can automate tasks previously performed by practitioners. The AV industry is unusual in that it combines highly technical engineering work with deeply personal service relationships. These two dimensions reinforce each other when AI is used to amplify practitioner capability, and undermine each other when it is used to replace practitioner contribution without acknowledgment.

This standard does not take a position against AI tools. It defines appropriate use. Search, drafting assistance, boilerplate generation, grammar tools, and task-specific AI operational tools all fall within appropriate use and are explicitly permitted. The concern is narrower: AI substituting for the practitioner's voice, judgment, or presence in contexts where clients and colleagues expect and are paying for those things.

### Why SHOULD, Not MUST

The majority of requirements in this document use SHOULD rather than MUST. This reflects the nature of a professional conduct standard. MUST in SANE documents is reserved for requirements whose violation constitutes a failure of safety, interoperability, serviceability, or functional correctness. Sending an AI-generated email is a professional judgment failure, not a technical failure in that sense. SHOULD communicates that this is the recognized professional standard, while acknowledging that practitioners make contextual judgments.

The two MUST requirements (R-4.1.5 and the privacy requirement in Section 8.1) reflect cases where the failure mode is not a judgment call: forwarding unread AI technical content to clients as expert opinion, and pasting client-confidential data into AI tools without authorization, are clear violations regardless of context.

---

## Appendix B: Revision History

| Version | Date | Summary |
|---|---|---|
| 0.1 | 2026-07-05 | Initial draft |
