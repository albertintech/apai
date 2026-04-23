# Federal Elections Modernization Act

## The Case for Blind Districting

### Published April 2026

Based on Rev 5.3 of the Federal Elections Modernization Act

---

Every redistricting cycle, Americans watch the same drama unfold. A census is conducted. Mapmakers -- legislators, commissions, consultants -- begin drawing lines. Lawsuits follow. Courts intervene. Maps are redrawn, sometimes multiple times. Elections are held under boundaries that may be struck down next year. The process consumes years, hundreds of millions of dollars, and whatever residual public trust remains in the fairness of the system. Then the next census arrives, and the cycle repeats.

The Federal Elections Modernization Act (FEMA), hereafter referred to as "the Act," proposes to end this cycle by removing human judgment from congressional boundary placement entirely. Under the Act's Blind Districting architecture, all congressional district boundaries are determined by algorithmically neutral, deterministic methods -- no mapmaker, no commission, no discretion. The algorithm accepts census population data and a seat count. It produces one and only one output. Anyone with the same inputs can verify they get the same map.

This paper makes the case that Blind Districting is not merely feasible but structurally superior to every alternative -- including the independent redistricting commissions that represent the current reform consensus. That case, however, depends on a specific architectural pairing: algorithmic districting works because the Act pairs it with proportional representation in multi-member districts, which eliminates the representational harm that suboptimal boundaries would otherwise cause. Neither component achieves this result alone. Together, they produce manipulation-proof, litigation-proof, representation-preserving districting that no human-drawn process can match.

---

## The Problem with Human-Drawn Lines

The argument for Blind Districting begins with a structural observation about the status quo: every human who draws a district boundary makes a choice. Even well-intentioned redistricting commissions exercise subjective judgment about communities of interest, geographic compactness, competitiveness, and boundary placement. That judgment creates two problems that no institutional design can fully resolve.

The first is manipulation. Sophisticated mapping software allows mapmakers to predict electoral outcomes at the precinct level, and the temptation to exploit that capability is bipartisan. In the 2020 redistricting cycle alone, more than 225 cases impacting congressional or state legislative lines were filed in state and federal courts, with maps challenged in at least 30 states (Levitt, All About Redistricting; Brennan Center, Redistricting Litigation Roundup). North Carolina's 2010-cycle litigation cost taxpayers at least $5.6 million. Wisconsin spent nearly $3.5 million defending its post-2011 maps. Pennsylvania lawmakers spent at least $3 million on outside lawyers in the most recent cycle. No authoritative aggregate national cost figure exists -- the spending is diffused across state treasuries, party organizations, legal nonprofits, and federal court resources, and no institution has incentive to track the total. That opacity is itself part of the problem.

The second problem is subtler and more fundamental. Even when mapmakers act in good faith, discretionary redistricting guarantees litigation because the criteria governing boundary placement are inherently contestable. How much weight should compactness receive relative to preserving county lines? Which communities of interest deserve priority when they overlap? How should competitiveness be balanced against minority representation? These are legitimate questions with no objectively correct answers -- which means that any map produced by human judgment can be challenged by someone applying different weights to the same criteria. The lawsuits are not aberrations. They are structural features of a process that asks humans to exercise judgment that is inherently disputable.

Blind Districting eliminates both problems by eliminating the judgment. The algorithm has no political preferences, cannot be lobbied, does not deadlock, and produces identical outputs from identical inputs. There is nothing left to manipulate and nothing left to litigate -- except the narrow question of whether a specific Voting Rights Act adjustment was truly the minimum necessary, a dramatically smaller attack surface than the current system provides.

---

## What the Computational Literature Shows

The academic literature on computational redistricting has matured substantially over the past decade. Three research groups have driven most of the methodological innovation: the MGGG Redistricting Lab at Tufts University (Moon Duchin, Daryl DeFord, Justin Solomon at MIT), the Quantifying Gerrymandering group at Duke University (Jonathan Mattingly, Gregory Herschlag), and the ALARM Project at Harvard University (Kosuke Imai, Cory McCartan). The algorithmic landscape is broader than most policy discussions acknowledge, spanning deterministic geometric methods like shortest splitline (Warren D. Smith), optimization approaches using integer programming (Validi, Buchanan, and Lykhovyd 2022), Voronoi-based and weighted k-means clustering methods (Cohen-Addad, Klein, and Young 2018), and the ensemble methods -- ReCom, Forest ReCom, Sequential Monte Carlo -- that now dominate court-facing analysis (DeFord, Duchin, and Solomon 2021; McCartan and Imai 2023).

The most important finding for this paper is that fully automated congressional map generation is technically feasible when criteria are formalized. Levin and Friedler (2019) demonstrated that a divide-and-conquer algorithm can generate valid congressional plans for nearly every multi-district state while achieving strong population equality. The computational infrastructure exists and has been proven at scale.

Equally important is what the literature does *not* endorse. No peer-reviewed paper advocates for fully automated, human-discretion-free redistricting as a policy reform. Researchers in this space tend to present their tools as evaluative baselines rather than as replacements for human judgment. Duchin has explicitly argued that ensemble-generated plans "are not likely to be good plans without extensive human vetting and adaptation." The reason is specific and consistent across the literature: blind algorithms ignore communities of interest, and under winner-take-all rules, a community split across two single-member districts loses all representation. That objection is serious. Under winner-take-all rules, it is disqualifying.

Two additional findings shape the structural argument. First, Altman (1997) established that optimal redistricting is computationally intractable -- NP-hard in the formal sense -- and Najt, DeFord, and Solomon (2019) proved that even approximately uniform sampling from all valid plans is intractable. This means that any sophisticated optimization-based redistricting method involves implementation choices that reintroduce discretion at the algorithm-design stage. Simple deterministic methods like shortest splitline sidestep this problem entirely by accepting narrow criteria and producing a unique output. Second, Levin (2023) raises the "Hal-mander" concern: that automation can be used to launder partisan choices by embedding bias in an objective function's weights, producing maps that appear algorithmic but encode human preferences. The Hal-mander objection is real -- but it is an objection to sophisticated optimization algorithms, not to simple deterministic methods that have no tunable parameters.

The literature's objections to blind districting are genuine and well-documented. This paper does not argue that the computational redistricting community has it wrong. It argues that their objections apply to blind districting as a standalone reform within a winner-take-all system -- and that the Act's architectural pairing with proportional representation resolves the specific vulnerabilities they identify.

---

## The Counterarguments at Their Strongest

A position paper that does not engage its strongest objections is not worth publishing. Four counterarguments deserve serious treatment.

### "Algorithms ignore communities of interest"

This is the most frequently cited objection to blind districting, and under winner-take-all rules, it is the strongest. The argument holds that geographic communities -- neighborhoods, cultural enclaves, economic regions, groups with shared infrastructure or environmental concerns -- have representational interests that require conscious boundary placement to protect. An algorithm that processes only population and geography cannot identify these communities, and if it splits one across two single-member districts, that community loses all representation.

The factual premise is correct: blind algorithms cannot identify communities of interest. But the claim that this causes representational harm depends on a winner-take-all electoral structure that the Act does not use.

Under STAR-PR in a five-seat district, a community constituting 20% of the district's population elects roughly one representative regardless of where the boundary falls. The representation is emergent from the math -- from voter preferences expressed through scored ballots -- not dependent on a mapmaker's judgment about where to place a line. The algorithm's blindness to community geography stops being a defect because proportional representation ensures representation through voting patterns rather than boundary packaging.

The objection also rests on an unstated assumption: that "communities of interest" is a stable, operationalizable concept that human mapmakers can reliably identify. The evidence suggests otherwise. By Justin Levitt's count (All About Redistricting, Loyola Law School), state definitions of "community of interest" vary from Alabama's expansive inclusion of racial, ethnic, partisan, and cultural interests to California's explicit exclusion of relationships with political parties or incumbents. The Brennan Center's survey identified 24 states that address communities of interest in some form, but with definitions so varied that a community qualifying under one state's standard might not qualify under another's. Makse (2012) describes existing definitions as "nebulous." In practice, redistricting commissions typically identify communities of interest through public testimony and self-identification -- qualitative and participatory rather than rigorous in any measurable sense.

The strongest contemporary defense of communities of interest as a rigorous standard comes from Chen, Wang, Grofman, Ober, Barnes, and Cervas (2022), who argue that technological advances -- crowdsourced mapping platforms like Representable and large-scale survey data -- now make data-driven community identification possible. This paper takes their argument seriously. Even if rigorous community identification is technically achievable, the process still requires prioritization choices when communities overlap or conflict, which reintroduces the discretion that generates litigation. More fundamentally, the overhead of running a rigorous community-identification process every redistricting cycle is substantial, while the alternative -- blind algorithm plus proportional representation -- is low-overhead, deterministic, and verifiable. And under proportional representation, the representational claims that communities of interest are meant to protect are addressed through voting patterns without requiring geographic packaging.

The residual version of the objection -- advanced most carefully by Stephanopoulos (2012) -- holds that some interests are inherently territorial: land use, environmental regulation, infrastructure planning, and neighborhood-level cultural preservation require geographic representation that proportional voting alone cannot capture. This is the strongest form of the argument, and this paper acknowledges it. The response is that under multi-member districts of 3-7 seats, geographic communities are still substantially preserved within the larger district. Representatives serve overlapping geography, and constituents can approach whichever member is most responsive to local concerns. The geographic bond is diluted relative to single-member districts but not severed -- and the tradeoff is a redistricting process free of the manipulation, litigation, and contested judgment that characterize the status quo.

### "Algorithms cannot handle VRA compliance"

The Voting Rights Act requires that redistricting not dilute the voting strength of racial and linguistic minorities. Becker, Duchin, Gold, and Hirsch (2021) have shown that ensemble methods can miss VRA concerns if the underlying model lacks the right demographic and legal structure. A blind algorithm operating without reference to racial data cannot, by definition, assess whether its output complies with the VRA.

This objection is correct on its face, and the Act does not attempt to override it. Instead, the Act's architecture treats VRA compliance as a bounded, transparent exception to algorithmic neutrality rather than a reason to abandon it. The algorithm runs first. The Department of Justice reviews the output. Only if there is a documented VRA violation does any human touch a boundary -- and when they do, the adjustment is governed by four constraints: specificity requirements explaining the violation, the minimum adjustment principle (the smallest number of census blocks reassigned necessary to cure the violation), dual map publication (before and after adjustment), and expedited three-judge-panel judicial review with direct Supreme Court appeal (Section 410(d)).

The critical distinction is between the status quo -- where human discretion is the starting point and every subsequent review tries to determine whether that discretion was properly exercised -- and the Act's architecture, where human intervention is the exception, bounded by statute, and fully transparent. The VRA exception is the narrowest possible departure from algorithmic neutrality.

Moreover, the Act's combination of algorithmic districting and proportional representation offers a structurally stronger protection for communities of color than the current system of human-drawn majority-minority districts. Under single-member plurality, a community of color constituting 30% of a region's population receives zero representatives unless a mapmaker deliberately draws a majority-minority district. Even when such districts are created, they pack the community into one seat while bleaching surrounding districts -- a dynamic both parties have historically exploited. Under STAR-PR in a five-seat district, that same community likely elects one and possibly two representatives without any human drawing a line on their behalf. The representation is emergent from the math, not dependent on the goodwill or legal obligation of whoever holds the redistricting pen.

### "Algorithmic gerrymandering is the next frontier"

Levin (2023) argues that automation can launder partisan choices -- that a programmer can subtly tune an objective function's weights to favor one party while the output appears algorithmic and neutral. The "Hal-mander" objection is serious because it identifies a genuine vulnerability in sophisticated optimization-based algorithms where tunable parameters create space for hidden bias.

The Act addresses this through two reinforcing mechanisms. First, the statutory default is shortest splitline -- a deterministic geometric method that accepts only population data and state boundaries as inputs. There are no tunable parameters, no objective function to weight, and no implementation choices that could embed partisan preference. Shortest splitline's simplicity is itself a structural safeguard against algorithmic gerrymandering, not a limitation.

Second, if the Electoral Science Office certifies a more sophisticated replacement algorithm, the change must pass through Tier 3 review: supermajority Commission approval (5 of 7 commissioners), public comment, Congressional review with joint resolution disapproval authority, published source code, independent verification by two external bodies, and public replication rights (Section 410). The source code is published so that anyone can verify the algorithm produces the maps it claims to produce. Two independent bodies verify it. Any member of the public can replicate the output. No one has to trust the ESO's judgment because there is no hidden judgment involved.

The Hal-mander concern applies to systems where algorithmic sophistication masks discretionary choices. It does not apply to a system designed around radical transparency, simplicity, and multi-layered verification.

### "No democracy has done this"

This objection is partially correct but overstated. Mexico's National Electoral Institute (INE) has used optimization algorithms -- simulated annealing and artificial bee colony methods -- as the primary input to federal redistricting since the late 1990s (Trelles, Altman, Magar, and McDonald 2016; Gutierrez-Andrade et al. 2019). Political parties may propose counter-maps, but those proposals must score better on the same pre-defined objective criteria as the algorithm's output. The move to computational redistricting helped transform Mexico from a one-party dominant system into a competitive democracy by ensuring boundary changes were driven by population shifts rather than ruling-party discretion.

Mexico's process is not fully human-discretion-free -- a technical committee selects the objective function, and party input is permitted. But it demonstrates that algorithmic redistricting is feasible at national scale and has operated successfully for nearly three decades. The Act's approach extends the Mexican precedent by eliminating the party-input phase and pairing algorithmic districting with proportional representation to address the representational concerns that the Mexican model still accommodates through human adjustment.

Trelles et al. (2023) identify real implementation problems with Mexico's process: insufficient source-code transparency and inability of external parties to replicate the algorithm's outputs. The Act's Section 410 algorithm integrity provisions -- source code publication, independent verification, public replication rights, and tamper detection -- directly address every documented weakness of the Mexican model. The Act does not merely borrow from Mexico's experience; it learns from its failures.

Beyond Mexico, every other democracy that uses single-member districts and redraws them periodically relies on independent commissions rather than algorithms. The United Kingdom, Canada, Australia, New Zealand, India, and Germany all use statutory criteria, public consultation, and commission judgment (Handley and Grofman 2008; DeSilver 2025). None uses an algorithm as the primary decision-maker. The international consensus has settled on commissions as the alternative to partisan legislative control -- Blind Districting represents a further step in the same anti-discretionary direction.

The novelty is real, and this paper does not pretend otherwise. The 1967 Uniform Congressional District Act had no precedent either. The question is not whether another democracy has done this exact thing but whether the structural logic holds. It does.

---

## The Affirmative Case: Why the Pairing Works

The case for Blind Districting is not a case for algorithms in isolation. It is a case for a specific architectural pairing that resolves a trilemma the computational redistricting literature has identified but not solved.

The trilemma is this: optimal redistricting is computationally intractable (Altman 1997; Najt, DeFord, and Solomon 2019). Sophisticated algorithms that incorporate legal criteria reintroduce discretion through implementation choices. Simple deterministic algorithms avoid discretion but ignore criteria that matter for representational outcomes. The literature's response has been to use algorithms as evaluative baselines while preserving human judgment for final maps -- a pragmatic compromise that accepts the costs of discretionary redistricting as unavoidable.

The Act resolves the trilemma by changing the underlying electoral structure. Under proportional representation in multi-member districts, the criteria that simple algorithms ignore -- communities of interest, competitiveness, minority representation -- are addressed through voting patterns rather than boundary placement. A community constituting 20% of a five-seat district elects roughly one representative regardless of where the boundary falls. Competitiveness is inherent because every seat in a multi-member district is contested. Minority representation is emergent from the math rather than dependent on a mapmaker's judgment.

This means the Act can use a simple, deterministic, fully transparent algorithm -- shortest splitline as the statutory default -- without accepting the representational harm that simplicity would cause under winner-take-all. The algorithm's blindness to community geography is not a defect to be mitigated; it is a feature that ensures no actor can embed preferences in the boundary-drawing process. And proportional representation ensures that blindness does not translate into representational failure.

Each component covers the other's weakness:

- Blind Districting eliminates human discretion from boundary-drawing, but algorithms alone cannot guarantee fair representation under winner-take-all rules.
- STAR-PR ensures proportional representation regardless of boundary placement, but someone still has to draw the district lines, and under human-drawn maps, that discretion is the attack surface for manipulation.
- Together, they produce districting that is manipulation-proof (no discretion to exploit), litigation-proof (no subjective judgment to contest), and representation-preserving (proportional allocation makes boundary placement irrelevant to outcomes).

This is the structural insight the existing literature has not engaged with, because the existing literature evaluates algorithmic redistricting within the winner-take-all framework. Once proportional representation is stipulated as a design constraint, the objections that have kept blind districting out of serious policy discussions dissolve -- not because they were wrong, but because they were answering a different question.

---

## The Gerrymandering Problem Blind Districting Solves

The empirical evidence on partisan gerrymandering reinforces the case for eliminating human discretion from redistricting. The most rigorous recent study -- Kenny, McCartan, Simko, Kuriwaki, and Imai (2023), published in the Proceedings of the National Academy of Sciences -- used ensemble simulations to compare enacted 2020-cycle maps against non-partisan baselines across all 50 states. Their central finding: partisan gerrymandering is widespread but mostly cancels at the national level, producing a net Republican advantage of approximately 2 seats. The primary harm is not net partisan seat advantage but the systematic destruction of electoral competition.

The competitiveness data is stark. Under 2020-cycle maps, the Brennan Center documented approximately 30 Biden-won districts with margins under 8 points and 30 Trump-won districts with margins under 8 points -- the fewest competitive districts in at least 52 years. The Cook Political Report in early 2026 rated just 18 of 435 House races as toss-ups, less than 5% of the chamber. This is not a one-cycle aberration. It is the structural product of a system where mapmakers can predict outcomes at the precinct level and draw boundaries accordingly.

The metrics literature is now mature enough to support this diagnosis from multiple angles. The efficiency gap (Stephanopoulos and McGhee 2015), mean-median difference (McDonald and Best 2015), partisan bias (Gelman and King 1994), and declination (Warrington 2018) each capture different dimensions of redistricting distortion. No single metric is dispositive -- Ratliff, Somersille, and Veomett (2025) have shown that any individual metric can be gamed -- but the family of metrics converges on a consistent picture: discretionary redistricting systematically reduces electoral competition, and the harm compounds over time as mapping technology becomes more precise.

Blind Districting addresses this problem at its source. An algorithm that processes only population data and state boundaries cannot draw safe seats because it has no information about partisan composition. And even if, by geometric accident, an algorithmically drawn district happened to favor one party heavily, STAR-PR in multi-member districts ensures that the minority party's voters still elect representation proportional to their numbers. The combination eliminates both the intentional gerrymandering that the metrics literature documents and the unintentional geographic sorting that Chen and Rodden (2013) have shown produces substantial partisan bias even under neutral redistricting.

---

## The Independence Architecture

Blind Districting's structural advantages are only as durable as the institutional protections preventing its capture. The Act addresses this through Section 410, which establishes layered independence protections designed so that no single point of failure can compromise the neutrality of the boundary-drawing process.

Executive non-interference prohibits any executive branch official from directing, influencing, or attempting to influence any districting determination. Commissioners and staff must document and report prohibited contacts to the Government Accountability Office. Commissioner removal protections prevent politically motivated dismissal during active redistricting cycles, and recess appointments to the Commission are prohibited. Budget independence ensures a mandatory minimum appropriation with sequestration protection and OMB-independent disbursement, preventing the ESO from being defunded into incapacity. Algorithm integrity requires source code publication, independent verification by two external bodies, public replication rights, and tamper detection. Anti-circumvention provisions prevent any other entity from drawing federal maps, prohibit conditional appropriations attached to ESO funding, and bar reorganization that would place the ESO under another agency.

Each defense covers a different attack surface. Capturing appointments does not help if existing commissioners cannot be removed during redistricting. Starving the budget does not help if the default algorithm is self-executing -- the Clerk of the House applies shortest splitline directly from census data, and the maps draw themselves. Weaponizing the Department of Justice does not help if any voter can obtain expedited three-judge-panel review. The architecture is designed for a hostile political environment, not a cooperative one.

---

## Conclusion

The case for Blind Districting is not that algorithms are perfect mapmakers. It is that human judgment in redistricting is the vulnerability -- the attack surface that enables manipulation, guarantees litigation, and produces the systematic destruction of electoral competition that the empirical literature documents.

The computational redistricting literature has identified this problem but settled on a pragmatic compromise: use algorithms as evaluative tools while preserving human judgment for final maps. That compromise is reasonable within a winner-take-all framework, where boundary placement determines representational outcomes and suboptimal boundaries cause real harm. But it accepts the costs of discretionary redistricting -- the lawsuits, the manipulation, the safe seats, the hundreds of millions spent litigating lines -- as unavoidable.

The Act rejects that compromise by changing the underlying electoral structure. Proportional representation in multi-member districts makes boundary placement irrelevant to representational outcomes. Communities achieve representation through voting patterns rather than geographic packaging. Minority groups elect representatives proportional to their numbers without depending on a mapmaker's judgment. Competitiveness is inherent in every multi-member district rather than dependent on how lines are drawn.

This pairing -- algorithmically neutral districting plus proportional representation -- produces a redistricting process with no human discretion to manipulate, no subjective criteria to litigate, and no representational harm from suboptimal boundaries. The algorithm provides process integrity: given a set of inputs, the outputs are arrived at deterministically and are auditable by anyone. Lines are touched by a human only when the Voting Rights Act requires it, and those minimal adjustments are fully transparent -- bounded by statute, documented through dual map publication, and subject to expedited judicial review.

The players do not get to write the rulebook. Blind Districting ensures the rulebook writes itself.

---

## Works Cited

Altman, Micah. 1997. "Is Automation the Answer: The Computational Complexity of Automated Redistricting." *Rutgers Computer & Technology Law Journal* 23(1): 81-142.

Becker, Amariah, Moon Duchin, Dara Gold, and Sam Hirsch. 2021. "Computational Redistricting and the Voting Rights Act." *Election Law Journal* 20(4): 407-441.

Becker, Amariah, and Justin Solomon. 2020. "Redistricting Algorithms." In Moon Duchin and Olivia Walch, eds., *Political Geometry*. Birkhauser. Chapter 16, pp. 303-340.

Brennan Center for Justice. 2010. "Communities of Interest." Redistricting series monograph.

Brennan Center for Justice. 2022. "Gerrymandering Competitive Districts to Near Extinction."

Brennan Center for Justice. 2025. "Redistricting Litigation Roundup."

Chen, Jowei, and Jonathan Rodden. 2013. "Unintentional Gerrymandering: Political Geography and Electoral Bias in Legislatures." *Quarterly Journal of Political Science* 8(3): 239-269. DOI: 10.1561/100.00012033.

Chen, Sandra J., Samuel S.-H. Wang, Bernard Grofman, Richard F. Ober Jr., Kyle T. Barnes, and Jonathan R. Cervas. 2022. "Turning Communities of Interest into a Rigorous Standard for Fair Districting." *Stanford Journal of Civil Rights and Civil Liberties* 18(1): 101-189.

Cohen-Addad, Vincent, Philip N. Klein, and Neal E. Young. 2018. "Balanced Centroidal Power Diagrams for Redistricting." arXiv preprint.

DeFord, Daryl, Moon Duchin, and Justin Solomon. 2021. "Recombination: A Family of Markov Chains for Redistricting." *Harvard Data Science Review* 3(1). DOI: 10.1162/99608f92.eb30390f.

DeSilver, Drew. 2025. "U.S. Stands Out Globally in How It Draws Legislative Districts." Pew Research Center, December 19, 2025. https://www.pewresearch.org/short-reads/2025/12/19/us-stands-out-globally-in-how-it-draws-legislative-districts/.

Gelman, Andrew, and Gary King. 1994. "A Unified Method of Evaluating Electoral Systems and Redistricting Plans." *American Journal of Political Science* 38(2): 514-554.

Gutierrez-Andrade, Miguel Angel, Eric Alfredo Rincon-Garcia, Sergio Gerardo de-los-Cobos-Silva, Pedro Lara-Velazquez, Roman Anselmo Mora-Gutierrez, and Antonin Ponsich. 2019. "Simulated Annealing and Artificial Bee Colony for the Redistricting Process in Mexico." *Interfaces* 49(3): 189-200. DOI: 10.1287/inte.2019.0992.

Handley, Lisa, and Bernard Grofman, eds. 2008. *Redistricting in Comparative Perspective*. Oxford: Oxford University Press.

Herschlag, Gregory, Han Sung Kang, Justin Luo, Christy Vaughn Graves, Sachet Bangia, Robert Ravier, and Jonathan C. Mattingly. 2020. "Quantifying Gerrymandering in North Carolina." *Statistics and Public Policy* 7(1): 30-38. DOI: 10.1080/2330443X.2020.1796400.

Kenny, Christopher T., Cory McCartan, Tyler Simko, Shiro Kuriwaki, and Kosuke Imai. 2023. "Widespread Partisan Gerrymandering Mostly Cancels Nationally, but Reduces Electoral Competition." *Proceedings of the National Academy of Sciences* 120(25): e2217322120. DOI: 10.1073/pnas.2217322120.

Levin, Harry A. 2023. "The Rise of the Hal-mander: Is Gerrymandering by Algorithm the Next Frontier of Partisan Gerrymandering?" *Georgetown Law Journal* 111(4): 891.

Levin, Harry A., and Sorelle A. Friedler. 2019. "Automated Congressional Redistricting." *ACM Journal of Experimental Algorithmics* 24: 1.10:1-1.10:24. DOI: 10.1145/3316513.

Levitt, Justin. *All About Redistricting*. Loyola Law School. https://redistricting.lls.edu.

Makse, Todd. 2012. "Defining Communities of Interest in Redistricting Through Initiative Voting." *Election Law Journal* 11(4): 503-517. DOI: 10.1089/elj.2011.0144.

McCartan, Cory, and Kosuke Imai. 2023. "Sequential Monte Carlo for Sampling Balanced and Compact Redistricting Plans." *Annals of Applied Statistics* 17(4): 3300-3323. DOI: 10.1214/23-AOAS1763.

McDonald, Michael D., and Robin E. Best. 2015. "Unfair Partisan Gerrymanders in Politics and Law: A Diagnostic Applied to Six Cases." *Election Law Journal* 14(4).

Najt, Elle (Lorenzo), Daryl DeFord, and Justin Solomon. 2019. "Complexity and Geometry of Sampling Connected Graph Partitions." arXiv:1908.08881. https://arxiv.org/abs/1908.08881. [Peer-reviewed companion: Najt, DeFord, and Solomon, "Empirical Sampling of Connected Graph Partitions for Redistricting," *Physical Review E* 104(6), 064130 (2021). DOI: 10.1103/PhysRevE.104.064130.]

Ratliff, Thomas, Stephanie Somersille, and Ellen Veomett. 2025. "Don't Trust a Single Gerrymandering Metric." *La Matematica* 4(3): 764-809. DOI: 10.1007/s44007-025-00172-y.

Ricca, Federica, Andrea Scozzari, and Bruno Simeone. 2013. "Political Districting: From Classical Models to Recent Approaches." *Annals of Operations Research* 204(1): 271-299. DOI: 10.1007/s10479-012-1267-2.

Stephanopoulos, Nicholas O. 2012. "Redistricting and the Territorial Community." *University of Pennsylvania Law Review* 160: 1379-1477.

Stephanopoulos, Nicholas O., and Eric M. McGhee. 2015. "Partisan Gerrymandering and the Efficiency Gap." *University of Chicago Law Review* 82(2): 831-900.

Trelles, Alejandro, Micah Altman, Eric Magar, and Michael P. McDonald. 2016. "Open Data, Transparency and Redistricting in Mexico." *Politica y Gobierno* 23(2): 331-364.

Trelles, Alejandro, Micah Altman, Eric Magar, and Michael McDonald. 2023. "No Accountability Without Transparency and Consistency: Evaluating Mexico's Redistricting-by-Formula." *Election Law Journal: Rules, Politics, and Policy* 22(1): 80-99. DOI: 10.1089/elj.2021.0061.

Validi, Hamidreza, Austin Buchanan, and Eugene Lykhovyd. 2022. "Political Districting to Minimize Cut Edges." *Mathematical Programming Computation* 14(4): 623-672. DOI: 10.1007/s12532-022-00221-5.

Warrington, Gregory S. 2018. "Quantifying Gerrymandering Using the Vote Distribution." *Election Law Journal* 17(1): 39-57.

Warshaw, Christopher, Eric McGhee, and Michal Migurski. 2022. "Districts for a New Decade -- Partisan Outcomes and Racial Representation in the 2021-22 Redistricting Cycle." *Publius: The Journal of Federalism* 52(3): 428-451. DOI: 10.1093/publius/pjac020.

---

<!--
## Revision History

**Revision 1.0** (Current)
- Initial publication
- Covers: computational redistricting literature, counterarguments (communities of interest, VRA compliance, algorithmic gerrymandering, international precedent), affirmative case for algorithmic-plus-PR pairing, comparative evidence (Mexico, international commissions), quantified gerrymandering effects, independence architecture
-->

*Revision history available in the raw file.*

> 📥 [Download this document](https://github.com/albertintech/apai/blob/main/docs/congress/cmf/fema/the-case-for-blind-districting.md) (opens on GitHub -- click the ⬇ download button)

*Last revised April 2026*

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
