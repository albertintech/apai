# American Payment Network Act

## Overview

### Published February 2026

Based on Rev 3.7 of the American Payment Network Act

---

## Problem Statement

Participation in the modern American economy requires access to digital payment systems. Wages arrive via direct deposit. Bills are paid online. Government benefits flow through electronic transfers. Tax refunds, marketplace transactions, and peer-to-peer payments all assume that participants have a bank account and the ability to send and receive money digitally.

Yet millions of Americans remain outside this system. According to the FDIC's 2023 National Survey, approximately 5.6 million U.S. households have no bank account at all, and another 19 million are underbanked -- they have accounts but still rely on expensive alternative financial services for basic needs. These rates are significantly higher among low-income households, households with disabilities, Black and Hispanic families, and single-parent households. An unbanked worker cashing a $1,000 paycheck at a check-cashing store loses $30-50 in fees. Over a year, these costs can reach hundreds of dollars per household -- a meaningful burden for families already living on tight margins.

Beyond individual costs, financial exclusion creates broader economic friction. Employers bear costs when workers cannot receive direct deposit. Government programs operate less efficiently when they cannot reach recipients electronically. And programs like the American Prosperity Stability Payment (APSP) require reliable, nationwide payment infrastructure to function effectively.

## Solution Architecture

The American Payment Network Act (APNA), hereafter referred to as "the Act," establishes the American Payment Network (APN) -- a nationwide, utility-style digital payments infrastructure operated by the Treasury Department through a new Office of Digital Payment Infrastructure (ODPI). The design follows the model of rural electrification and the interstate highway system: public infrastructure that enables private participation rather than displacing it.

The Act takes a digital-first approach, prioritizing rapid nationwide access through web, mobile, and feature phone channels before physical infrastructure buildout. Financial institutions participate as APN Agents -- banks, credit unions, and fintechs that connect to the Treasury-operated backbone and provide front-end services to customers. This preserves private sector competition while guaranteeing that a fee-free baseline option exists for everyone.

The network is self-capitalizing. Rather than depending on annual appropriations, the Act establishes an American Payment Network Fund within Treasury that receives revenues from network transaction fees, interest earnings, agent certification fees, and state cost-sharing payments. Initial capitalization comes through Treasury borrowing authority capped at $15 billion, with mandatory repayment from operational revenues within fifteen years. This structure insulates the network from budget negotiations and ensures continuous operations during government shutdowns.

## Major Provisions

**Network Accounts.** Every lawful U.S. resident is entitled to hold a fee-free Network Account through the APN. Accounts carry no minimum balance, no maintenance or overdraft fees, and no credit check requirement. Features include instant payment capability, FDIC-equivalent insurance, optional debit card and mobile wallet functionality, and physical debit cards provided at no cost.

**Technology-Neutral Access.** The Act guarantees access through multiple channels: smartphone applications, web browsers, feature phones via SMS and USSD protocols, ATMs, physical debit cards, APN Agent locations, and USPS facilities. No person can be denied access to core services due to lack of smartphone ownership, broadband connectivity, or computing device ownership. Public libraries and community centers are integrated as secure access points.

**APN Agent Framework.** Regulated financial institutions, credit unions, and approved fintech providers may serve as APN Agents, connecting to the APN backbone under two tiers. Full-Service Agents provide direct cash handling at physical locations. Digital Agents operate primarily through digital channels and satisfy cash access requirements through ATM networks, retail partnerships, or fee reimbursement. Agents earn regulated service fees comparable to FedNow/ACH pricing and may not impose additional fees on basic accounts.

**USPS Physical Infrastructure.** The Act prioritizes agreements with the U.S. Postal Service to establish APN access points at post offices nationwide, targeting banking deserts, rural communities, and low-income urban neighborhoods first. USPS facilities provide cash services, in-person onboarding, account access terminals, and multilingual support. Purpose-built APN service centers are authorized only where USPS coverage is insufficient.

**Youth and Vulnerable Populations.** Section 4A establishes a comprehensive framework for minor accounts. Individuals aged 16 and older can open accounts independently without parental consent. Working minors under 16 can access accounts with parental consent and joint visibility. Special provisions guarantee independent access for emancipated minors, foster youth, homeless youth, and domestic abuse survivors, with enhanced privacy protections and confidential account services. Prohibitions against financial abuse by parents, guardians, or employers are enforced through APN Agent reporting to state authorities.

**Capitalization and Funding.** The American Payment Network Fund finances all network operations without ongoing appropriations. Treasury borrowing authority of up to $15 billion provides initial capitalization at Treasury's cost of borrowing, with mandatory repayment from Fund revenues within fifteen years. Network transaction fees, capped at five basis points (0.05%) of transaction value, fund ongoing operations. Congressional notification triggers at 50% and 75% of borrowing authority provide oversight of potential cost overruns. After repayment, a six-month operating reserve is maintained, with excess revenues available for fee reduction, service expansion, or transfer to the General Fund.

**Cash Access.** Every account holder has the right to deposit and withdraw cash without fee anywhere in U.S. jurisdiction. Full-Service Agents provide direct cash handling. Digital Agents satisfy cash access requirements through participation in nationwide ATM networks, retail partnerships, or automatic ATM fee reimbursement. The Treasury maintains a public, searchable registry of all access points coordinated with major mapping service providers.

## Implementation Overview

The Act employs a five-year implementation horizon with a digital-first sequencing strategy. The Foundation phase (months 1-12) stands up the ODPI, establishes regulatory frameworks, and deploys core technical architecture. A Pilot phase (months 13-18) launches in at least five states representing diverse geographies. USPS partnership agreements are executed within 24 months and initial access points operational within 36 months. Nationwide digital coverage is achieved within five years, with physical infrastructure continuing to expand based on demonstrated need.

An Advisory Board of nine members -- representing Treasury, the Federal Reserve, USPS, community financial institutions, consumer protection agencies, and the public -- advises on standards, security, and access. The Government Accountability Office audits the network every three years, and public quarterly reports disclose account uptake, transaction volume, service availability, and security metrics.

## Conclusion

The Act builds economic infrastructure rather than creating a transfer program. It solves the problem of financial exploitation through competition -- providing a free, reliable alternative that makes predatory pricing economically unviable -- rather than through regulation that can be gamed, litigated, or politically eroded. It creates the payment backbone on which the broader American Shared Prosperity Compact operates, connecting APSA's stability payments and SOCA's child benefits to every eligible American through a single, self-sustaining network.

---

## Revision History

**Revision 3.7** (Current)
- Updated reference line to Rev 3.7
- No changes to overview content

**Revision 3.6**
- Initial publication

> 📄 [Download this document](https://github.com/albertintech/apai/blob/main/docs/aspc/apna/overview.md) (opens on GitHub -- click the ⬇ download button)

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
