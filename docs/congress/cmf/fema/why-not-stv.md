# Federal Elections Modernization Act

## Why Not STV?

### Published March 2026

Based on Rev 5.2 of the Federal Elections Modernization Act

---

Proportional representation is the most important structural reform available to American democracy. The diagnosis is shared across the reform community: winner-take-all, single-member districts distort representation, suppress political competition, and entrench a two-party system that leaves millions of voters without meaningful representation. The question is not whether to adopt proportional representation. The question is which proportional method to use.

The Federal Elections Modernization Act (FEMA), hereafter referred to as "the Act," uses Allocated Score -- also called STAR Proportional Representation or STAR-PR -- for multi-member House elections. Voters score candidates from 0 to 5 stars on the same ballot used for single-winner STAR elections. Seats are filled in rounds: each round elects the highest-scoring candidate, then reduces the ballot weight of that candidate's supporters proportionally, ensuring the next round reflects the preferences of voters who are not yet fully represented.

The Single Transferable Vote (STV) -- now marketed in the United States as "Proportional Ranked Choice Voting" or PRCV -- is the most prominent competing proportional method and the one proposed in the Fair Representation Act (H.R. 4632), the only live federal proportional representation bill in Congress. FairVote, RepresentWomen, the League of Women Voters, the RCV Resource Center, and allied organizations have invested substantial institutional resources in positioning STV as the natural next step for the American ranked-choice voting movement.

This paper argues that STV inherits structural pathologies from its Instant Runoff Voting (IRV) elimination engine that Allocated Score avoids, that the multi-winner context amplifies several of these pathologies rather than mitigating them, and that STV creates an architectural dependency on surrounding electoral infrastructure -- particularly primary elections -- that the Act's design eliminates. The rebranding of STV as "Proportional Ranked Choice Voting" leverages growing voter familiarity with single-winner RCV but obscures rather than resolves these structural limitations.

---

## What STV Is

STV is a multi-winner electoral system in which voters rank candidates in order of preference on a ranked ballot. Tabulation proceeds through a combination of quota-based election and sequential elimination.

A quota -- typically the Droop quota -- is calculated by dividing the total number of valid ballots by the number of seats plus one, then adding one. In a five-seat district with 100,000 voters, the quota is approximately 16,668. Any candidate whose first-choice vote total meets or exceeds the quota is declared elected. That candidate's surplus votes -- the ballots beyond the quota -- are then transferred to each ballot's next-ranked candidate, at a fractional transfer value reflecting the surplus. If no candidate meets the quota after surplus transfers, the candidate with the fewest votes is eliminated and their ballots are transferred to the next-ranked active candidate at full value. This process of electing, transferring surpluses, and eliminating continues until all seats are filled.

The relationship between STV and IRV is not analogical -- it is mechanical. STV uses the same elimination algorithm as IRV: identify the candidate with the fewest first-choice votes, eliminate that candidate, and redistribute their ballots. When STV is applied to a single-winner election, it *is* IRV. The Irish Constitution does not distinguish between the two; both single-winner presidential elections and multi-winner parliamentary elections are conducted under "proportional representation by means of the single transferable vote." The systems share a ballot format and an elimination engine. What changes is the number of winners and the presence of surplus transfers.

STV has been used for national elections in Ireland since 1921 and Malta since 1921. Australia has used STV for its Senate since 1949. In the United States, Cambridge, Massachusetts has used STV for its city council since 1941, and Portland, Oregon adopted what it calls "proportional ranked choice voting" for its city council in 2024. The Fair Representation Act (H.R. 4632), introduced in the 119th Congress by Representatives Beyer, Raskin, Peters, McGovern, and Khanna, would mandate STV for multi-member House elections and IRV for Senate elections.

The recent rebranding of STV as "Proportional Ranked Choice Voting" or PRCV is a deliberate strategic choice by U.S. reform organizations. As the RCV Resource Center has described, single-winner RCV introduces voters to ranked ballots, which reduces resistance to adopting proportional systems that use the same ballot format. The terminology connects STV to the growing familiarity Americans have with RCV from implementations in Alaska, Maine, New York City, and dozens of municipalities. This is effective advocacy. It is also analytically imprecise: IRV is a single-winner, non-proportional method, and attaching "proportional" to the "ranked choice voting" brand elides the fundamental difference between electing one winner and achieving proportional representation across multiple seats.

---

## The Strongest Case for STV

Intellectual honesty requires engaging with the best version of the STV argument, not a caricature. STV has genuine structural strengths that any comparative analysis must acknowledge.

First, STV is candidate-centered rather than party-centered. Voters vote for individual candidates, not party lists. This makes STV compatible with nonpartisan elections -- a critical feature in the American context, where the majority of local elections are nonpartisan and where party-list systems are politically untenable. FairVote and RepresentWomen have correctly identified this as a decisive advantage over European-style list proportional representation for American adoption.

Second, STV produces proportional outcomes. Any faction that commands a Droop quota's worth of support can elect a representative. In a five-seat district, a group with 20% support wins approximately one seat. This is the core promise of proportional representation, and STV delivers it.

Third, STV has a century-long track record in functioning democracies. Ireland and Malta have conducted stable democratic governance under STV for over a hundred years. Whatever STV's theoretical limitations, these countries have not collapsed, have conducted peaceful transfers of power, and have maintained broadly representative parliaments. The Australian Senate has operated under STV since 1949. This accumulated institutional experience is not a trivial argument -- it demonstrates that STV is operationally viable at national scale, which is more than any competing proportional method can claim.

Fourth, ranked ballots capture genuine information about voter preferences. The ability to rank candidates in order of preference is more expressive than a single categorical choice and allows voters to support their true first choice while designating fallback candidates.

Fifth, and perhaps most importantly from a practical standpoint, STV has a political advocacy infrastructure that no alternative proportional method can match. The Fair Representation Act is the only federal proportional representation bill in Congress. FairVote's organizational capacity, its state and municipal track record with single-winner RCV, and its decade-long public education investment have created a viable political pathway for STV adoption. The argument that PRCV is the most politically achievable path to proportional representation in the United States is not wrong. It may be the strongest argument in STV's favor.

These are real strengths. But they are strengths of proportional representation as a principle, of candidate-centered electoral design, and of effective political organizing -- not of the specific elimination mechanism that STV uses to tabulate results. The question this paper addresses is whether that mechanism carries structural costs that a different proportional method avoids.

---

## Why STV Falls Short

STV's tabulation algorithm is built on sequential elimination -- the same mechanism used by single-winner IRV. This section examines six structural consequences of that design choice and one architectural dependency it creates, assessing in each case what the multi-winner context mitigates and what it amplifies.

### Non-Monotonicity Carries Over

A voting system is monotonic if giving a candidate more support can never cause that candidate to lose. Monotonicity is widely regarded among social choice theorists as a fundamental property -- a minimum standard for a system's internal logic to be coherent. Perversity, as the violation is formally called, means the system can respond backwards to voter preferences: popularity causes defeat, and unpopularity causes victory. The German Federal Constitutional Court has ruled that negative responsiveness violates the constitutional guarantee of equal and direct suffrage.

IRV fails monotonicity. This is well established in the literature and has been documented empirically. Graham-Squire and McCune's 2023 survey of 182 American IRV elections in which no candidate won a first-round majority found seven instances of non-monotonicity -- a rate of 3.8%. Theoretical models using the impartial culture assumption predict monotonicity failure in approximately 15% of three-candidate IRV elections, with the rate rising as elections become more competitive.

STV inherits this failure because it uses the same elimination engine. As the Electowiki's survey of voting criteria states, most variants of STV "are not monotonic, especially all that are currently in use for public elections (which simplify to IRV when there is only one winner)." No ranked voting method has been proven to satisfy both Droop proportionality and monotonicity. Gallagher's 2013 study of Irish PR-STV elections identified plausible non-monotonicity in 20 out of 1,326 elections between 1922 and 2011 -- a low empirical frequency, but not zero.

The multi-winner context does not mitigate this problem. It arguably amplifies it. Multi-winner STV elections involve more candidates and more elimination rounds than single-winner IRV elections. Each elimination round creates an opportunity for the kind of order perturbation that produces non-monotonic outcomes. As one analyst has observed, multi-winner STV elections can be approximately regarded as a sequence of single-winner IRV elections, and the more winners and candidates involved, the more likely non-monotonic outcomes become.

Allocated Score is monotonic. Giving a candidate a higher score increases their weighted score total; it cannot decrease it. There is no elimination sequence to perturb, no transfer chain to redirect. The property holds unconditionally.

### Center Squeeze Persists

The center squeeze is a class of spoiler effect in which a broadly preferred candidate -- one who would win head-to-head against any other candidate -- is eliminated in an early round because their support is distributed as second and third preferences rather than concentrated as first preferences. Systems that suffer from center squeeze incentivize candidates to avoid the political center, creating polarization pressure even if center squeezes seem empirically rare, because the system discourages broadly appealing candidates from running in the first place.

This is IRV's most consequential real-world failure mode. The 2022 Alaska special election, in which the Condorcet winner Nick Begich III was eliminated in the first round by Sarah Palin, is the most prominent American example.

STV inherits the center squeeze because it uses the same elimination trigger: the candidate with the fewest first-choice votes is eliminated, regardless of their broader support. The Droop quota provides partial mitigation -- in a five-seat district, a candidate needs only approximately 16.7% first-preference support to survive, compared to 50%+ in single-winner IRV. A broadly acceptable candidate with 20% first-preference support would survive in a five-seat STV district but might be eliminated in an IRV race. However, within any round where elimination is occurring among candidates below quota, the center-squeeze logic applies with full force. For the last seat in a district, the dynamics effectively collapse to a single-winner IRV contest among the remaining candidates, and the full center-squeeze vulnerability returns.

More importantly, Ogren's 2024 study of Candidate Incentive Distributions provides quantitative evidence that STV's incentive structure is worse than IRV's on this dimension. In simulations with four winners and twenty candidates, STV produced a more lopsided Candidate Incentive Distribution than any single-winner voting method in the study. The incentive for STV candidates to appeal to opposing voters was essentially zero -- a Candidate Incentive value of 3% at the most-opposed end of the spectrum, compared to 38% under STV-Minimax, a variant that replaces the fewest-first-preferences elimination rule with a Condorcet-based elimination rule while keeping everything else identical. This finding demonstrates that the incentive distortion is not an inherent cost of proportional representation -- it is a specific consequence of the elimination algorithm STV uses.

Allocated Score addresses center squeeze structurally. Broad support registers as high weighted scores even when a candidate is not anyone's top-rated choice. A candidate who receives a 3 from 80% of voters will outscore a candidate who receives a 5 from 30% and a 0 from everyone else. The scoring mechanism rewards breadth of support, not just intensity of first-choice concentration.

### Ballot Exhaustion Amplifies

In RCV systems, a ballot exhausts when all of its ranked candidates have been eliminated, leaving no further preferences to transfer. The ballot exits the count and no longer influences subsequent rounds.

In single-winner IRV, ballot exhaustion is already a documented concern. A 2015 study by Burnett and Kogan examined four American IRV elections and found inactive ballot rates ranging from 9.6% to 27.1%. These rates are sufficient to alter the meaning of "majority" -- the winner's majority is calculated from active ballots only, not from ballots cast.

The multi-winner context amplifies ballot exhaustion because it attracts larger candidate fields. A five-seat STV district may have fifteen to thirty candidates. Asking voters to rank all of them is unrealistic. Most voters will rank a handful of candidates and stop, which means their ballots can exhaust before all seats are filled. The Fair Representation Act itself acknowledges this reality: Section 322(b)(1)(C) includes a provision allowing states to cap the number of rankings at a "maximum feasible number" if it is "not feasible" for the ballot to accommodate enough ranking positions -- with a floor of five. This is the bill's authors conceding that the ranking interface has a practical ceiling that large candidate fields can exceed.

Allocated Score does not have a ballot exhaustion mechanism. The 0-5 scale captures information about all candidates simultaneously. A voter who scores three candidates at 5, two at 3, and leaves the rest blank has expressed preferences that remain operative throughout all allocation rounds. The ballot weight diminishes as preferred candidates win seats, but the ballot itself never exits the count. There is no structural equivalent of exhaustion.

### Surplus Transfer Arbitrariness

When an STV candidate exceeds the Droop quota, the surplus votes -- ballots beyond what was needed to elect that candidate -- must be redistributed to other candidates. How this redistribution is performed varies by implementation, and different methods can produce different winners from identical ballots.

The oldest approach is random selection: a subset of the elected candidate's ballots is physically drawn and transferred at full value. This introduces literal randomness into the outcome. The Gregory method, used in many modern implementations including the system specified by the Fair Representation Act, transfers all of the elected candidate's ballots at a fractional transfer value calculated from the surplus. The Meek method uses iterative recalculation of transfer values until the results converge. The Warren method extends the Meek approach. Each method operationalizes the concept of "surplus transfer" differently, and each can produce different seat allocations from the same set of ballots.

This is not a minor technical detail. It is a hidden design parameter that is outcome-determinative in contested elections but invisible to virtually all voters and most advocates. The Fair Representation Act specifies fractional transfer values truncated to four decimal places -- a reasonable implementation choice, but one that differs from the implementations used in Ireland, Malta, and Australia. Voters are told that STV is "proportional ranked choice voting" without being informed that the specific surplus transfer method chosen by the legislature can change who wins.

This pathology is unique to multi-winner STV. It does not exist in single-winner IRV (which has no surpluses) and it does not exist in Allocated Score. Under Allocated Score, the weight reduction formula is specified, deterministic, and proportional: each ballot's weight is reduced in exact proportion to its contribution to the elected candidate's total. The same ballots always produce the same result, regardless of implementation. There is no randomness, no rounding artifact, and no choice among competing transfer methods.

### Ballot Complexity and Spoiling

The ranked ballot grid -- in which voters must fill one bubble per row and one bubble per column in a matrix of candidates and rank positions -- is the most complex ballot format examined in the APAI *Voting Methods Explained* series. It creates multiple error modes that simpler ballot formats do not: overvoting a rank position (two candidates marked at the same rank), duplicate ranking (the same candidate appearing at more than one rank), skipped ranks, and exceeding the maximum permitted number of rankings.

The consequences of these errors are not uniform. Pettigrew and Radley's analysis of ranked-choice voting ballot data from Maine, New York City, San Francisco, and Alaska found that approximately 0.6% of ballots contained an overvoting error, of which 65.8% were rejected -- making overvoting the primary ballot-killing failure mode. Skipped rankings and overranking, while more common (2.0% and 2.4% respectively), had much lower rejection rates (5.8% and 1.5%), suggesting that most jurisdictions have recognized these errors as processable.

The demographic dimension is significant. Research on San Francisco RCV elections by Neely and McDaniel documented higher error rates in precincts with larger populations of elderly voters, voters with lower incomes, foreign-born voters, and voters from certain racial and ethnic communities. Cormack's 2023 analysis and 2026 follow-up provide additional evidence that ballot complexity and error rate are not independent variables. This is not an argument against any particular system in isolation. It is an observation that when ballot complexity increases, the voters most likely to encounter difficulty are often those whose voices are already underrepresented.

Multi-winner STV amplifies ballot complexity because the candidate field is larger. A ranked ballot grid for a five-seat district with twenty candidates is a 20-row, 20-column matrix containing 400 bubbles. The error surface expands in proportion to the grid's size. Every additional candidate adds another row and column of opportunities for mismarking.

The 0-5 star ballot used by Allocated Score presents a simpler interface: each candidate occupies one row with six bubbles (0 through 5). There is no column constraint -- scoring Candidate A a 5 and Candidate B a 5 is valid, not an overvote. Leaving a candidate unscored defaults to 0. The error modes are narrower: out-of-range marks (if a paper ballot allows them) and ambiguous marks. There is no rank-ordering constraint, no column-uniqueness constraint, and no skip logic.

### Architectural Dependency: The Field Size Problem

The five pathologies discussed above -- non-monotonicity, center squeeze, ballot exhaustion, surplus transfer arbitrariness, and ballot complexity -- share a common characteristic: they scale with the number of candidates. More candidates mean more elimination rounds (increasing non-monotonicity and center-squeeze risk), more preferences to rank (increasing exhaustion and complexity), and more surplus transfers to manage (increasing arbitrariness). Multi-member districts naturally attract large candidate fields. STV does not resolve this tension internally. It transfers the problem outward onto the surrounding electoral architecture.

The available mechanisms for managing candidate field size each carry structural costs.

Primaries are the most obvious American approach. The Fair Representation Act explicitly preserves and regulates them. Section 203 of H.R. 4632 devotes three subsections to establishing minimum candidate requirements for partisan primaries, nonpartisan blanket primaries, and states that skip primaries entirely. The bill's authors understood that STV with unmanaged fields creates problems, and they built an entire section of federal legislation to regulate the winnowing process. But primaries reintroduce the very problems proportional representation is supposed to solve: the question of what kind of primary to use (open, closed, blanket), what voting method to use for the primary (often plurality, which reintroduces spoiler effects at an earlier stage), chronically low turnout that produces unrepresentative nomination outcomes, substantial cost to taxpayers for administering a separate election, and vulnerability to partisan manipulation. The voters most harmed by primary systems are those who do not participate in them -- and non-primary voters are disproportionately younger, lower-income, and members of racial and ethnic minorities.

Party nomination discipline -- the Irish model -- is the alternative that has sustained STV for a century. Irish parties carefully manage how many candidates they nominate per constituency and instruct supporters on how to distribute preferences to avoid splitting first-choice votes among co-partisans. This works mechanically, but it concentrates gatekeeping power in party organizations. It is the opposite of the candidate-centered, voter-empowerment pitch that PRCV advocates make in the American context. It also has no mechanism in nonpartisan elections, which are a major share of American local races and one of PRCV's primary selling points.

Ballot access thresholds -- signature requirements, filing fees -- are blunt instruments that disproportionately affect the minor-party and independent candidates that proportional representation is supposed to empower.

Accepting large fields without winnowing means voters face ballot grids with twenty to forty candidates to rank, which is where exhaustion, spoiling, and demographic disparities in error rates become severe.

STV does not just have internal pathologies. It creates a dependency on external mechanisms to manage the conditions under which it can function tolerably. It pushes complexity outward -- onto parties, onto primary elections, onto voters.

The Act's Single Unified General Election is structurally enabled by the choice of Allocated Score, whose ballot interface degrades gracefully with large candidate fields rather than catastrophically. Scoring thirty candidates on a 0-5 scale is cognitively different from ranking thirty candidates in strict preference order. A voter scores their known favorites 5, their known opponents 0, and assigns middling scores to candidates they know something about. Leaving a candidate unscored defaults to 0 and does not exhaust the ballot. The voter does not need to have an opinion about the relative ordering of their fourteenth versus fifteenth preference.

Because Allocated Score does not require field winnowing, the Act eliminates state-administered primaries for federal offices entirely. Parties retain full autonomy to conduct internal nominations through caucuses, conventions, or other processes -- at their own expense, without state election infrastructure. This enfranchises the millions of voters who do not participate in primaries, returns time and money to taxpayers, and removes a structural leverage point for partisan manipulation. This is not a convenience feature. It is architecturally enabled by the proportional method's tolerance of large candidate fields. STV-based proposals cannot make the same promise without either accepting severe ballot complexity or quietly relying on the very primary architecture they claim to improve.

---

## The Affirmative Case: Allocated Score

The Act provides Allocated Score as a proportional method designed to achieve the same representational goals as STV while avoiding the structural costs of sequential elimination.

Under Allocated Score, voters score all candidates from 0 to 5 stars -- the same ballot action used for single-winner STAR elections. Seats are filled in rounds. In each round, the candidate with the highest weighted score total is elected. That candidate's supporters then have their ballot weight reduced in proportion to their contribution to the elected candidate's total. The weight reduction ensures that each elected candidate "costs" an equal share of the electorate's total voting power. Voters who gave strong support to an elected candidate have more weight spent than those who gave weaker support, preserving the remaining weight for use in subsequent rounds. The process repeats until all seats are filled.

This mechanism addresses each of the structural limitations identified in the preceding section.

Allocated Score is monotonic. Scores are summed; there is no elimination sequence whose order can be perturbed by changes in support. Giving a candidate a higher score increases their weighted score total unconditionally -- it can never backfire.

Allocated Score resists center squeeze. Broad support registers as high weighted scores. A consensus candidate who receives moderate scores from a wide base will outscore a polarizing candidate who receives maximum scores from a narrow base but zeros from everyone else. The system rewards the breadth of a candidate's appeal, not just the concentration of their first-choice support.

Allocated Score does not produce ballot exhaustion. The 0-5 scale captures preferences for all candidates simultaneously. Ballot weight diminishes as preferred candidates win seats, but the ballot itself remains in the count throughout all allocation rounds.

Allocated Score uses deterministic weight reduction rather than surplus transfers. The formula is specified, proportional, and produces identical results from identical ballots regardless of implementation. There is no randomness, no rounding-method dependency, and no hidden design parameter.

Allocated Score uses a simpler ballot interface that scales gracefully with large candidate fields. The same 0-5 star ballot is used for single-winner STAR elections (President, Senate) and multi-winner Allocated Score elections (House). Voters learn one ballot action for all federal contests. The error surface is narrower than the ranked ballot grid, and the absence of a rank-ordering constraint means there is no ballot exhaustion from incomplete expression.

And because the ballot interface tolerates large fields without degrading, the Act's Single Unified General Election eliminates state-administered primaries for federal offices entirely -- placing all qualified candidates directly on the November ballot and removing a structural leverage point that STV-based proposals must either preserve or replace.

The tradeoff must be acknowledged honestly. Allocated Score has no century-long track record in national government elections. Ireland has used STV since 1921; no country has used Allocated Score for a parliamentary election. This is a legitimate concern that deserves transparency, not dismissal.

But the characterization of Allocated Score as untested requires qualification. The 0-5 star ballot is not a novel interface -- it is among the most widely used rating scales in the world. Hundreds of millions of people rate products, services, drivers, and businesses on star scales through Google, Amazon, Yelp, Uber, and similar platforms every day. The cognitive task -- assign a score reflecting your assessment -- is deeply familiar to the modern electorate in a way that ranking fifteen candidates in strict preference order is not. The system was deliberately named "STAR Voting" to leverage this cultural ubiquity.

STAR voting has been used in binding political elections. The Independent Party of Oregon conducted its 2020 statewide primary entirely using STAR, with over one million eligible participants across multiple offices. The Democratic Party of Oregon used STAR for its 2020 presidential delegate elections. The city of Astoria, Oregon used STAR for a 2025 council appointment. In organizational governance, the Python Software Foundation's core development team adopted Bloc STAR for its 2025 and 2026 Steering Council elections after concluding that Approval voting did not capture sufficient preference intensity. The Democratic Socialists of America's Los Angeles chapter implemented both single-winner STAR and STAR-PR for its 2024 leadership elections -- deliberately replacing STV, finding that STAR-PR provided proportionality while maintaining a consensus incentive and avoiding what the chapter described as the polarizing aspects of elimination rounds. Growing numbers of labor unions, professional associations, and political organizations use STAR through platforms like BetterVoting.com.

None of this is equivalent to a century of national parliamentary elections. But Allocated Score is not where STV was in 1921 -- launching into democratic governance with no tools for predicting its behavior. The advantage the field has today is the capacity for rigorous pre-adoption evaluation. Voter Satisfaction Efficiency simulations, Candidate Incentive Distribution analysis, Monte Carlo modeling of strategic behavior, and formal criterion compliance testing allow electoral scientists to characterize a method's structural properties with high confidence before a single ballot is cast. STV and MMP were adopted into national governance without these tools. The structural arguments presented in this paper -- monotonicity, resistance to center squeeze, absence of exhaustion and surplus transfer arbitrariness, ballot simplicity, and architectural independence from primaries -- are grounded in mathematical properties and simulation evidence that were simply unavailable when STV was first adopted. Advocates of STV are entitled to weigh accumulated operational experience heavily, and this paper does not dismiss that consideration. It argues that structural soundness and operational familiarity are both relevant criteria, and that the former points decisively toward Allocated Score.

---

## The Advocacy Landscape and Opportunity Cost

FairVote is the dominant advocacy organization for ranked-choice voting in the United States. Its institutional capacity -- built over decades of state and municipal campaigns, policy research, public education, and legislative advocacy -- has no parallel among organizations supporting alternative voting methods. The PRCV branding strategy extends this capacity directly into the proportional representation space: if voters are already comfortable ranking candidates in single-winner RCV elections, the argument goes, extending that experience to multi-winner elections is a natural and achievable step.

This institutional advantage is real. The Fair Representation Act has congressional sponsors. It has been introduced in multiple sessions of Congress. It builds on growing public familiarity with RCV from implementations in Alaska, Maine, New York City, and elsewhere. No comparable federal legislation exists for Allocated Score, STAR voting, approval voting, or any other alternative voting method. The Act developed by APAI has not been introduced as legislation. On the dimension of immediate political viability, PRCV is further along.

The structural critique of STV comes from a dispersed set of voices with nothing approaching FairVote's institutional weight: the Equal Vote Coalition, individual academics like Ogren, Quinn, and Wolk, the Center for Election Science (historically), and scattered social choice theorists. The asymmetry between the PRCV advocacy infrastructure and the structural critique is striking.

This asymmetry matters because it can create the impression that the debate is settled -- that STV is the proportional method, rather than a proportional method with specific structural properties that can be compared against alternatives. The terminological framing reinforces this: calling STV "Proportional Ranked Choice Voting" positions it as the proportional extension of an already-familiar system, rather than as one of several competing approaches to proportional representation, each with different tradeoffs.

It is worth noting that the scholarly literature reflects a gap similar to the one identified in the fusion voting position paper. No published peer-reviewed study systematically compares STV against score-based proportional alternatives like Allocated Score using common evaluative criteria. Ogren's 2024 Candidate Incentive Distribution study comes closest, including STV and STV-Minimax in its multi-winner analysis, but it does not evaluate Allocated Score. The comparative case that PRCV advocates implicitly make -- that STV deserves reform energy over structural alternatives -- has not been subjected to the rigorous empirical testing that the resource investment demands. The advocacy literature is predominantly a conversation among proponents, and the absence of head-to-head comparative analysis is itself a gap that the field should address.

Political viability and structural soundness are separate questions. A proposal can be politically easier to pass and still be the wrong mechanical choice. The relevant question for institutional design is not which method has the best advocacy infrastructure, but which method produces the best representational outcomes with the fewest structural failure modes. The evidence presented in this paper argues that Allocated Score is the stronger design on those criteria.

---

## Conclusion

STV is a historically significant proportional method with genuine strengths. Its advocates are correct that proportional representation is superior to winner-take-all, that candidate-centered systems suit American nonpartisan elections, and that STV has served democracies tolerably for a century.

But "tolerably" is not the correct standard when structural alternatives exist that achieve the same proportional goals without the elimination engine's pathologies. STV's sequential elimination produces non-monotonicity, enables center squeeze, generates incentive distributions more lopsided than any single-winner method studied, and creates surplus transfer arbitrariness that can change election outcomes through hidden design parameters. Its ranked ballot interface degrades under the large candidate fields that multi-member districts naturally attract, amplifying ballot exhaustion, spoiled ballot rates, and demographic disparities in error rates. And it creates an architectural dependency on primary elections or party nomination discipline to manage candidate field size -- pushing complexity outward onto surrounding institutions rather than resolving it internally.

The Act selected Allocated Score because it produces proportional representation that is monotonic, resistant to center squeeze, free of ballot exhaustion and surplus transfer arbitrariness, and administratively simpler -- while using the same ballot format as single-winner STAR voting for a consistent voter experience across all federal elections. And because Allocated Score tolerates large candidate fields gracefully, it enables the Single Unified General Election -- eliminating the primary system entirely rather than depending on it.

The question is not whether STV is better than plurality. It is. The question is whether STV is the best available proportional method given what we now know about electoral system design. The evidence presented in this paper argues that it is not.

---

## Works Cited

Burnett, Craig M., and Vladimir Kogan. "Ballot (and Voter) 'Exhaustion' Under Instant Runoff Voting: An Examination of Four Ranked-Choice Elections." *Electoral Studies* 37 (2015): 41-49.

Cormack, Lindsey. "More Choices, More Problems: Ballot Error and Voter Engagement with Ranked Choice Voting in New York City." Working Paper, 2023.

Cormack, Lindsey. "Deficiencies in Recent Research on Ranked Choice Voting Ballot Error Rates." Report, 2026.

Equal Vote Coalition. "Proportional Representation." https://www.equal.vote/proportional. Accessed March 2026.

Equal Vote Coalition. "Leading Voting Methods." https://www.equal.vote/voting_methods. Accessed March 2026.

Gallagher, Michael. "Monotonicity and Non-Monotonicity at PR-STV Elections." Paper presented at the Annual Conference of the Elections, Public Opinion and Parties (EPOP) Specialist Group, University of Lancaster, September 2013.

Graham-Squire, Adam T., and David McCune. "An Examination of Ranked-Choice Voting in the United States, 2004-2022." *Representation* 61 (2023): 1-19.

McCune, David, and Adam Graham-Squire. "Monotonicity Anomalies in Scottish Local Government Elections." *Social Choice and Welfare* 63, no. 1 (August 2024): 69-101.

Miller, Nicholas R. "Closeness Matters: Monotonicity Failure in IRV Elections with Three Candidates." *Public Choice* 173, no. 1-2 (October 2017): 91-108.

Neely, Francis, and Jason McDaniel. "Overvoting and the Equality of Voice Under Instant-Runoff Voting in San Francisco." *California Journal of Politics and Policy* 7, no. 4 (2015): 1-27.

Ogren, Mark. "Voting Methods Shape Electoral Incentives: Candidate Incentive Distributions." Working Paper, 2024.

Pettigrew, Stephen, and Dylan Radley. "Ballot Marking Errors in Ranked Choice Voting." Working Paper, 2024.

Ramos, Albert E. *Federal Elections Modernization Act, Rev 5.2*. The American Policy Architecture Institute, February 2026.

United States Congress. *Fair Representation Act*. H.R. 4632, 119th Congress, 1st Session. Introduced July 23, 2025.

Wolk, Sara, Jameson Quinn, and Mark Ogren. "STAR Voting: Considerations and Simulations." *Constitutional Political Economy* 34 (2023): 301-325.

---

<!--
## Revision History

**Revision 1.1** (Current)
- DPS 2.8 compliance pass: migrated download link path from electoral/cmf/fema/ to congress/cmf/fema/; added 📥 prefix and ⬇ parenthetical emojis per DPS Rev 2.8 Section 1.9; added "Last revised April 2026" line per DPS Rev 2.5 Section 1.3
- Restructured header per DPS Rev 2.8 Section 1.2 Supporting Document format: H1 changed from paper title to proposal name; paper title moved to H2; descriptive subtitle retired (framing preserved in opening paragraphs)

**Revision 1.0**
- Initial publication
- Evaluates STV/PRCV against Allocated Score as proportional method for the Federal Elections Modernization Act
- Draws on Ogren 2024 (Candidate Incentive Distributions), Graham-Squire and McCune 2023 (empirical RCV pathology catalog), Gallagher 2013 (Irish PR-STV monotonicity), Burnett and Kogan 2015 (ballot exhaustion), Pettigrew and Radley 2024 (ballot marking errors), Cormack 2023/2026 (RCV ballot error analysis), Neely and McDaniel 2015 (demographic error disparities), Wolk Quinn and Ogren 2023 (STAR voting simulations), Equal Vote Coalition proportional representation and voting methods analyses, and the Fair Representation Act (H.R. 4632) legislative text
- Identifies six structural pathologies carried over or amplified from IRV to STV: non-monotonicity, center squeeze, ballot exhaustion, surplus transfer arbitrariness, ballot complexity, and architectural dependency on primary elections for field size management
- Classified as Position Paper per APAI Document Production Standards Rev 2.3
-->

*Revision history available in the raw file.*

> 📥 [Download this document](https://github.com/albertintech/apai/blob/main/docs/congress/cmf/fema/why-not-stv.md) (opens on GitHub -- click the ⬇ download button)

*Last revised April 2026*

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
