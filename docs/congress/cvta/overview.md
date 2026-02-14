# Candidate Verification and Transparency Act

## Overview

### Published January 2026

Based on Rev 1.2 of the Candidate Verification and Transparency Act

---

## Problem Statement

American democracy operates on a simple premise: voters choose their representatives. Yet voters consistently lack access to verified factual information about candidates for federal office. The system relies on adversarial discovery -- campaigns conducting opposition research, media organizations investigating claims, watchdog groups publishing findings -- to surface biographical information. This approach fails systematically.

Coverage is inconsistent. Competitive Senate races attract investigative resources; safe House seats do not. A candidate running unopposed or in a gerrymandered district faces less scrutiny than one in a battleground race, though both seek federal office with identical constitutional responsibilities and equivalent power to shape national policy.

Information is fragmented. Findings appear across multiple outlets with varying credibility and permanence. No central repository exists for verified records. Voters must assemble information from partisan opposition research, media investigations of uneven quality, and social media claims of uncertain provenance. Those with time, resources, and media literacy can navigate this landscape. Others cannot.

Timing fails repeatedly. Adversarial discovery often produces findings after primaries conclude, after early voting begins, or after candidates have assumed office. The George Santos case demonstrated how comprehensive biographical fabrications can survive an entire campaign cycle -- primaries, general election, and certification -- without systematic verification identifying the discrepancies. Only after the candidate took office did the full scope of misrepresentations become clear.

These failures are not incidental. They are structural features of a system that never established infrastructure for verification. The Constitution specifies qualifications for federal office. It says nothing about verifying whether candidates meet those qualifications or whether their biographical claims are accurate. That gap has persisted for over two centuries.

## Solution Architecture

The Candidate Verification and Transparency Act (CVTA), hereafter referred to as "the Act," addresses these structural failures through a dedicated informational infrastructure. The framework rests on several core principles.

**Verification, not regulation.** The Act establishes an agency that verifies documentary records and publishes findings. It does not regulate political speech, restrict ballot access, or determine who may serve. Voters receive authenticated information; they remain the sole decision-makers.

**Uniformity across candidates.** Every candidate for federal office undergoes identical verification procedures regardless of party, ideology, incumbency, or electoral viability. The presidential nominee of a major party and the third-party candidate in a single House district face the same checklist.

**Structural constraints on authority.** The Act enumerates specific documentary domains subject to verification and explicitly prohibits expansion into political beliefs, associations, or character evaluation. Expanding authority requires a three-fifths supermajority of both houses of Congress. Reducing authority requires only simple majorities. This asymmetry ensures governmental power is difficult to expand and easy to contract.

**Separation of verification from adjudication.** The Agency verifies records and publishes findings. A separate judicial body -- the Federal Candidate Eligibility Panel -- adjudicates constitutional eligibility disputes. This separation prevents the verification agency from acquiring quasi-judicial powers and ensures eligibility questions receive appropriate due process.

**Public access as infrastructure.** Verification serves voters only if findings are accessible. The Act mandates free access through multiple formats: human-readable summaries, detailed reports, machine-readable datasets, and public APIs. No registration, fees, or geographic restrictions limit access.

## Title-by-Title Summary

### Title I: Establishment of the Agency

Title I establishes the Federal Candidate Verification Agency as an independent entity outside executive branch control. The Agency's mission is explicitly limited to verifying documentary records, compiling standardized reports, and publishing findings for public use. Congress finds that public access to accurate candidate information is foundational to democratic self-government, that existing adversarial systems produce inconsistent and fragmented information, and that neutral standardized verification strengthens accountability while preserving political speech.

### Title II: Definitions and Scope

Title II defines key terms and establishes the boundaries of verification authority. A "candidate" includes anyone who files with the FEC, qualifies for ballot access, or raises funds for federal office. "Verification" means examining documentary records from authorized sources without interpretation or commentary. The Title explicitly excludes political ideology, policy positions, religious beliefs, personal relationships, loyalty, and moral character from verification scope. It prohibits investigative powers including surveillance, subpoenas, and compelled testimony.

### Title III: Federal Candidate Eligibility Panel

Title III creates a nine-judge panel within the federal judiciary to adjudicate constitutional eligibility disputes. Members are sitting Court of Appeals judges appointed by the Chief Justice, with no more than four from the same party, serving non-renewable five-year terms. The Panel holds exclusive jurisdiction over questions of age, citizenship, residency, and constitutional qualifications. It may not consider ideology, loyalty, or character. Proceedings are primarily documentary, with expedited timelines: 60 days for pre-primary disputes, 30 days pre-general, 10 days post-ballot. The burden of proof rests on the party asserting ineligibility, who must demonstrate constitutional disqualification by clear and convincing evidence.

### Title IV: Verification Procedures

Title IV establishes mandatory verification for all federal candidates triggered by FEC filing, ballot qualification, or meeting the federal definition of candidacy. The Agency verifies eight objective documentary domains: identity and citizenship, age, residency, education, employment history, military service, criminal and civil court records, and financial disclosure consistency. Section 406 establishes a consent-based authorization system for records held by third parties -- educational institutions, employers, licensing boards, military repositories. Candidates may authorize or decline release; the verification report reflects the outcome through standardized status notations. This mirrors the routine background check authorizations that private employers use under existing FERPA provisions.

### Title V: Agency Permanence and Scope Limitations

Title V makes the Agency permanent while constraining its authority. The Agency continues in perpetuity and may be dissolved only by explicit Act of Congress. Its budget is submitted independently, not through executive departments. All verification personnel are civil service employees; no more than five percent may be political appointees, and no political appointee may participate in verification activities. The Title establishes a "scope lock" requiring three-fifths supermajority to expand authority while permitting simple majority reductions. Ambiguities must be resolved narrowly in favor of limiting governmental authority.

### Title VI: Constitutional Safeguards

Title VI prohibits the Agency from regulating political speech, evaluating political messaging, or imposing ideological tests. The Agency may not determine truth or falsity of campaign statements. It may not publish commentary identifying inconsistencies between verified records and candidate claims. The Title preserves constitutional qualifications as the exclusive eligibility criteria and prohibits Congress from adding qualifications through statute. It establishes a private right of action for citizens alleging the Agency exceeded its authority or introduced ideological criteria, with relief limited to declaratory and injunctive remedies.

### Title VII: Public Access and Publication Standards

Title VII mandates that all verified records be publicly available without fee, registration, or usage restrictions. The Agency must publish Summary Voter Sheets (concise overviews), full Verification Reports (detailed documentation with citations), and machine-readable datasets. Publication must occur within 30 days of verification completion and no later than 90 days before the earliest primary ballot printing. The Title requires immutable audit logs recording every change, cryptographic integrity checks, and a public API for automated access. User interface requirements specify that the search function must be visible without scrolling, with no registration barriers or intermediary screens.

### Title VIII: Agency Misconduct and Accountability

Title VIII governs internal accountability. Prohibited acts include verification outside enumerated domains, collecting ideological information, selective treatment based on political considerations, and altering or withholding verified information. Data manipulation and records tampering constitute felonies. Agency employees engaged in verification may not coordinate with campaigns, donate to federal candidates, or use their position to influence political outcomes. The Inspector General operates independently with authority to audit processes, investigate misconduct, and issue public reports. Whistleblower protections apply to all employees who disclose misconduct.

### Title IX: Federalism and State Cooperation

Title IX preserves state authority over ballot access and election administration. States may not deny ballot access based on federal verification status. The Act does not permit the Agency to influence state ballot decisions. States may voluntarily transmit records already in their possession but are not required to modify processes or privacy rules. States may not obstruct access to legally public documents or impose discriminatory fees. When contradictory records exist, the Agency publishes all versions and flags discrepancies for judicial review.

### Title X: General Provisions

Title X addresses codification, rulemaking, judicial review, and effective dates. The Act takes effect upon enactment, with mandatory verification following the phased implementation in Title V. Rulemaking authority is limited to procedural implementation and may not expand verification domains or add enforcement powers. The D.C. Circuit holds exclusive jurisdiction over challenges, applying de novo review with no deference to Agency interpretation. Future expansions require explicit statutory language and three-fifths supermajority approval.

## Implementation Overview

The Act implements through three phases spanning approximately five years before mandatory verification begins.

**Phase I (Year 1)** focuses on agency formation: establishing leadership, initiating civil service hiring, and developing verification methodologies and systems.

**Phase II (Years 2-3)** operates as a pilot program with voluntary verification. The Agency publishes preliminary reports, refines standards based on operational experience, and builds capacity for mandatory implementation.

**Phase III** begins mandatory verification with the first presidential election cycle occurring no sooner than four years after enactment. Senate and House verification becomes mandatory one year after presidential implementation.

This phased approach allows systems development, staff training, and procedural refinement before mandatory compliance. It also permits congressional oversight and adjustment based on pilot experience.

## Conclusion

The Candidate Verification and Transparency Act creates infrastructure where none currently exists. It does not solve every problem of electoral information -- voters will still encounter misleading campaign advertising, partisan interpretation of verified facts, and strategic framing of candidate records. But it establishes a baseline: a neutral, standardized, publicly accessible repository of verified documentary information about every candidate for federal office.

The framework treats verification as scheduled maintenance on informational infrastructure rather than reform activism. It acknowledges that democratic self-government requires voters to make informed choices, and that informed choices require access to verified facts. The current adversarial system fails to provide that access consistently, equitably, or reliably. The Act fills the gap through limited, constrained, transparent governmental action that empowers voters without restricting candidates.

The detailed legislative text contains the full statutory language. The Policy Rationale document explains the reasoning behind major design choices and addresses anticipated concerns.

---

## Revision History

**Revision 1.1** (Current)
- Applied self-reference convention per APAI Document Production Standards Rev 1.6.
- Corrected filename to standardized published naming convention.

**Revision 1.0**
- Initial publication based on CVTA Rev 1.2

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
