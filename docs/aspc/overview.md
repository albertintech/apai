# American Shared Prosperity Compact

## Overview

### Published February 2026

Based on Rev 5.4 of the American Shared Prosperity Compact

---

## Problem Statement

The American economy generates extraordinary aggregate wealth while failing to deliver financial stability to most of its participants. This instability is not primarily a failure of individual effort or specific programs -- it reflects missing infrastructure that other developed nations take for granted. Three structural gaps create compounding vulnerability across the lifecycle.

The first is a payment gap. Over 20 million Americans lack bank accounts entirely, and millions more are underbanked -- relying on check-cashing services, prepaid cards, and payday lenders that extract billions annually in fees. When the federal government needs to reach these households with stimulus payments, tax refunds, or emergency assistance, it struggles. The 2020-2021 pandemic relief experience demonstrated this failure at scale: months of delays, lost payments, and hastily constructed workarounds that left the most vulnerable waiting longest.

The second is a stability gap. American workers face extraordinary economic volatility with no baseline income floor to prevent catastrophic descent. Nearly half of American adults lack savings to cover three months of expenses. Even households with two earners often cannot absorb modest disruptions -- a car breakdown, a medical bill, a seasonal layoff -- without crisis. Existing safety net programs are fragmented, means-tested, stigmatized, and often unavailable to those who need them most. Unlike peer nations, the United States provides no structural mechanism for maintaining household stability during working years.

The third is a child investment gap. The United States remains the only developed nation without a meaningful child allowance. American families bear extraordinary costs during the years that matter most for child development, and children in low-income families face developmental disadvantages that compound across generations -- not because their parents lack effort, but because the country lacks infrastructure to support families during critical periods. The 2021 temporary Child Tax Credit expansion proved dramatic improvement is possible (child poverty dropped by nearly half), but when it expired, poverty rates rebounded immediately.

These gaps interact destructively. Without payment infrastructure, benefits cannot reach people efficiently. Without adult stability, households cannot weather disruptions or invest in their children's futures. Without child investment, poverty transmits across generations. The result is an economy where precarity undermines productivity, household instability dampens long-term planning, consumer demand fluctuates unpredictably, and children's potential is constrained by circumstances of birth.

## Solution Architecture

The American Shared Prosperity Compact addresses all three gaps through a unified legislative framework consisting of three acts. Each act solves a distinct problem, has its own dedicated funding mechanism, and delivers independent value. When combined, the three acts create integrated economic infrastructure covering the full lifecycle -- from birth through retirement.

The framework's modularity is a deliberate architectural choice, not a concession. Major reforms rarely pass in single moments of political alignment. The Compact is built for the long game: any act that passes creates foundation for the others and builds constituencies for further reform. Each act uses conditional integration language -- "when available" clauses that automatically activate enhanced functionality when companion legislation is in place, without requiring the companion to exist.

Three core design principles govern the architecture. First, modularity: each act delivers tangible value on its own merits and can pass independently, in different legislative sessions, under different political coalitions. Second, integration-ready design: each act connects seamlessly when companion acts become available, with APNA providing payment rails, APSA providing enrollment infrastructure, and SOCA coordinating benefit calculations to prevent clawbacks. Third, political durability: separate funding streams prevent resource competition, broad-based participation creates constituencies that make repeal costly, and visible monthly benefits create the kind of tangible relationship between program and recipient that has sustained Social Security for nine decades.

## Component Overview

### American Payment Network Act (APNA)

APNA establishes a nationwide interoperable payment network that provides every eligible American with a fee-free Network Account. The network operates as public utility infrastructure -- comparable to the interstate highway system or rural electrification -- on which private innovation can operate.

Network Accounts are digital accounts administered by Treasury, accessible through mobile apps, web portals, ATM networks, and physical locations. They provide core financial services including direct deposit, bill pay, transfers, and debit access without the fees that burden low-income households. Users can link their existing bank accounts or use the Network Account as their primary account.

APN Agents form the service layer. Banks, credit unions, fintech companies, and the U.S. Postal Service become certified agents providing account access in their communities. This distributed model ensures geographic coverage -- including rural areas and underserved communities -- without requiring Treasury to build branch infrastructure.

Federal payments route through Network Accounts by default, including Social Security, tax refunds, veterans benefits, and stability payments under APSA and SOCA. Recipients can still choose direct deposit to private banks or paper checks, but Network Accounts provide the fastest, most reliable delivery.

The network is self-capitalizing. An American Payment Network Fund within Treasury receives revenue from transaction fees, interest earnings, and certification fees, repaying initial Treasury borrowing within fifteen years. No ongoing taxpayer cost is required, and operations continue uninterrupted during government shutdowns.

### American Prosperity and Stability Act (APSA)

APSA provides the American Prosperity Stability Payment (APSP) -- monthly income-adjusted payments that create an economic floor for adult households. The payment structure combines a $200/month baseline available to all eligible adults with an income-adjusted stability component that provides larger payments to lower-income households. As income rises, the stability component phases out smoothly through a logarithmic taper -- no benefit cliffs, and work always pays. At the clean exit threshold of 10x FPL (approximately $150,600), the baseline phases out, but this affects only about 10% of American adults. Nine in ten adults receive direct payments.

The American Prosperity Contribution (APC) funds the system at a rate of 12% on goods and services sold for domestic consumption. The APC is collected at each stage of production and distribution, similar in mechanics to a value-added tax but dedicated to stability payments rather than general revenue. This creates a clear reciprocal relationship: everyone contributes through consumption, everyone benefits through stability payments.

Revenue allocation splits 80% to federal APSP payments and administration (approximately $1.25 trillion annually) and 20% to state governments (approximately $312 billion annually). State revenue is distributed via pure population share with no federal mandates on usage. States report annually on fund allocation through a standardized transparency framework, enabling citizen oversight while preserving state autonomy.

APSA also contains integrated enrollment infrastructure (Section 10: Rapid Deployment and Enrollment) that enables rapid initial deployment through existing Treasury and IRS systems, with transition to Network Account distribution as APNA comes online. This consolidated approach replaced the originally separate American Economic Participation Act (AEPA), whose functions were absorbed into APSA as of Rev 4.0.

A Bridge Period Funding framework addresses the transition challenge -- how to begin payments before APC revenue reaches steady state. The framework uses three components: bounded deficit spending with statutory payback provisions (capped at $400 billion), progressive bridge taxes that sunset as APC revenue scales, and early APC pre-collection at reduced rates during the phase-in period.

### Secure Our Children Act (SOCA)

SOCA establishes a permanent, fully refundable child tax credit with monthly payments, a one-time Birth Support Payment, and dedicated funding through the Child Security Contribution.

The enhanced child tax credit provides $3,600 per year ($300/month) for children under 6 and $3,000 per year ($250/month) for children ages 6-17. Benefits are fully refundable regardless of earned income, eliminating the phase-in that excludes the poorest children under current law. The credit is universal -- every qualifying child receives the full amount regardless of parental income, with progressivity achieved entirely through the contribution mechanism. Monthly advance payments match family cash flow needs, with safe harbor provisions protecting families from overpayment clawbacks of up to $2,000 per child.

The Birth Support Payment provides $2,000 upon birth or adoption, with an advance payment option up to 60 days before the expected due date. The payment includes compassionate provisions for stillbirth and infant loss, indexed to inflation and available to adoptive parents and surrogacy arrangements.

The Child Security Contribution funds the system through a base rate of 1.50% of adjusted gross income plus a kicker rate of 3.00% on AGI above $500,000 (single) / $1,000,000 (joint). This generates approximately $270 billion annually, fully funding the approximately $257 billion program with a surplus flowing to the Family Security Stabilization Account. An automatic rate adjustment mechanism responds to funding fluctuations without requiring Congressional action, with bounds preventing extreme changes.

SOCA's funding stream is entirely separate from APSA's American Prosperity Contribution. This separation ensures the two programs do not compete for resources and creates distinct political constituencies defending each. Child tax credit amounts and Birth Support Payments are excluded from income calculations for APSA stability payments and federal means-tested programs, preventing benefit clawbacks.

## Implementation Overview

The Compact is designed for rapid deployment when passed as a package, with full integration achieved over approximately five years.

During the first year after enactment, foundation-building proceeds in parallel across all three acts. APNA begins infrastructure buildout and agent certification. APSA activates bridge taxes, launches rapid deployment through existing Treasury systems, and begins delivering first stability payments. SOCA activates the Child Security Contribution and begins child payments via existing IRS infrastructure, with Birth Support Payments available from January 1 following enactment and monthly advance child payments by July 1.

During years two and three, integration accelerates. APNA pilot programs become operational and expand nationwide digitally. APC pre-collection begins at reduced rates and scales toward the launch phase. Simple Form filers begin receiving Network Accounts. All payments transition to Network Accounts where available.

By years four and five, the system reaches maturity. APNA achieves full infrastructure operation. The APC reaches its full 12% rate. Bridge Period borrowing is retired. Legacy program consolidation is evaluated where functional overlap is demonstrated.

If acts pass separately rather than as a package, each proceeds on its own implementation timeline while including conditional language that enables integration when companion acts become available. APSA can deliver payments through existing Treasury systems if APNA never materializes. SOCA operates through existing IRS infrastructure regardless of whether APSA or APNA exist. Any act that passes first builds infrastructure that makes subsequent acts easier to implement.

## Conclusion

The American Shared Prosperity Compact addresses infrastructure gaps that perpetuate economic precarity across the lifecycle. Three integrated acts build the payment systems, adult stability floor, and child investment infrastructure that enable households to participate fully in economic life.

The Compact's modular design means partial success is still success. Any act that passes delivers immediate value and creates constituencies for further reform. This flexibility is not a weakness but a deliberate design choice reflecting the reality that major structural reform rarely happens in a single legislative moment.

The alternative to building this infrastructure is continued reliance on fragmented, means-tested, crisis-reactive programs that reach people too late, impose administrative burdens on those least equipped to navigate them, and remain perpetually vulnerable to budget politics. The Compact offers a different path: permanent infrastructure that makes stability possible across generations.

---

## Revision History

**Revision 5.4** (Current)

- Created fresh Overview document per APAI Document Production Standards Rev 1.6
- Replaces prior "Executive Summary" documents (retired document type)
- Content drawn from ASPC Executive Summary Publication (January 2026) and ASPC Rev 5.3 Executive Summary, updated to reflect APSA Rev 4.7 and current component act revisions
- SOCA child benefit amounts aligned to SOCA Rev 2.4 legislative text ($3,600/$3,000 age-differentiated structure)

> 📄 [Download this document](https://github.com/albertintech/apai/blob/main/docs/aspc/overview.md) (opens on GitHub -- click the ⬇ download button)

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
