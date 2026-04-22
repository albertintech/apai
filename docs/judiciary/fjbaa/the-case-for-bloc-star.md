# Federal Judicial Balance and Accountability Act

## The Case for Bloc STAR

### Position Paper

### Published April 2026

Based on Rev 2.3 of the Federal Judicial Balance and Accountability Act

---

This paper defends the Federal Judicial Balance and Accountability Act's (FJBAA) selection of Multi-winner Bloc STAR voting as the mechanism by which the Senate selects nominees from a presidential nomination slate, hereafter referred to as "the Act." The Act's broader documentation establishes that the slate-based confirmation process transforms the strategic landscape of judicial appointments by making obstruction irrational rather than dominant. This paper addresses a narrower and prior question: given the decision to use scored multi-winner selection, why is Bloc STAR the right method -- and not Approval Voting, Score Voting, Ranked Choice, or any of the other alternatives the election science literature has considered?

This question matters because Bloc STAR is not a well-known method outside specialist circles. Unlike plurality voting, ranked-choice voting, or even Approval Voting -- all of which have received sustained public attention -- Bloc STAR remains largely unfamiliar to general audiences, legislators, and policy analysts. That unfamiliarity creates a burden of explanation the Act's other documents do not fully discharge. The argument for the slate mechanism relies on Bloc STAR's specific mathematical properties; a reader who does not understand why those properties were chosen over alternatives cannot fully evaluate whether the architecture is sound.

This paper proceeds in five parts. Part I establishes the taxonomy of voting methods and the criteria relevant to the confirmation context. Part II evaluates the principal alternatives and explains why each fails on at least one critical criterion. Part III makes the affirmative case for Bloc STAR. Part IV presents comparative institutional evidence from organizations that have already worked through this selection problem. Part V addresses the strongest counterarguments.

---

## Part I: The Taxonomy and the Criteria

### A Brief Taxonomy

Voting methods divide into two fundamental families based on the information a ballot captures.

**Ordinal methods** ask voters to rank candidates in sequence. Plurality voting is the degenerate case -- rank only your first choice. Ranked Choice Voting (RCV), also called Instant Runoff Voting (IRV), extends this by asking voters to rank multiple candidates and uses sequential elimination rounds to produce a winner. The Borda Count assigns point values to each rank position and aggregates them. What these methods share is that they capture only the *order* of preferences, not the *intensity*. A voter cannot indicate that their second choice is nearly as good as their first, or nearly as bad as their last.

**Cardinal methods** ask voters to assign numeric scores to candidates along a scale. Score Voting (also called Range Voting) uses the average or total score across all ballots to select a winner. Approval Voting is the binary special case: voters assign each candidate either a 1 (approved) or a 0 (not approved). Cardinal methods capture preference intensity, which ordinal methods cannot.

**Bloc STAR** (Score Then Automatic Runoff, multi-winner variant) is a cardinal-ordinal hybrid. Voters score candidates on a 0-5 scale (the cardinal phase), identifying the two highest-scoring candidates. Those two then enter a head-to-head comparison in which the candidate preferred by more voters -- based on which scored higher on each ballot -- wins the seat (the ordinal runoff phase). For multi-winner elections, this process repeats iteratively until all seats are filled. The cardinal phase captures intensity; the ordinal runoff phase provides a majority-preference check.

### The Criteria

The Act's slate confirmation process has specific structural requirements that constrain the appropriate voting method. These requirements are not identical to those of general elections, which has implications for which methods transfer well.

**Multi-winner selection.** The Senate selects n nominees from a presidential slate of at least n x 2 candidates in a single proceeding. The method must handle multiple winners natively, without converting to a sequential series of single-winner races.

**Consensus orientation, not proportional representation.** The Senate is not a legislature selecting representatives for distinct factions. It is a deliberative body selecting the most broadly acceptable nominees from a slate that the president has already screened for basic acceptability. The goal is consensus, not proportionality. A method designed for proportional representation -- one that allocates seats to factions in proportion to their share of voter support -- would be structurally mismatched to this purpose.

**Resistance to strategic bullet voting.** An opposition Senate has strong incentives to engage in strategic voting: giving every presidential nominee a 0 and every preferred candidate a maximum score, regardless of actual preferences. The method must either make honest expression the dominant strategy or substantially reduce the payoff from strategic bloc scoring.

**Summability and transparency.** Senate votes are public record. The tabulation method must be transparent enough that any senator, staffer, or observer can verify the result independently. Methods that require centralized iterative processing across multiple elimination rounds -- and that cannot produce precinct-level tallies that aggregate to a correct statewide total -- impose opacity costs that are unacceptable in a legislative confirmation context.

**Decisiveness.** The method must reliably produce a result within the 120-day consideration period without requiring multiple re-votes or producing contested outcomes that require external resolution.

---

## Part II: Why the Alternatives Fall Short

### Binary Confirmation (Status Quo)

Binary confirmation -- the Senate votes yes or no on a single nominee -- is not formally a voting method within the Act's framework, but it is the baseline against which the Act's design must be compared. Its failure mode is the motivation for the entire slate mechanism. Under binary confirmation, the strategic calculus for an opposition Senate is straightforward: any nominee the president wants is presumptively unacceptable, and a vacancy costs the opposition nothing. The method concentrates all leverage in a single rejection decision and provides no mechanism for expressing qualified support or influencing who among several candidates is selected.

Binary confirmation is not merely imperfect -- it is the documented source of the nomination wars, strategic vacancies, and escalating confirmation battles that have characterized the last four decades of Supreme Court appointments. The case against it is made at length in the Act's Policy Rationale and is not rehearsed here.

### Approval Voting

Approval Voting is the most frequently proposed alternative to both binary confirmation and more complex scored systems. Its appeal is obvious: it is simple, familiar in concept (voters mark which candidates they "approve"), and expands the information available to selectors beyond a single choice. Several academic proposals for Supreme Court reform have suggested Approval Voting-style Senate selection as an improvement over binary confirmation.

Approval Voting has two structural weaknesses that disqualify it in the Act's context.

**First, it cannot capture intensity.** Approval Voting is a cardinal method only in the degenerate sense: its "scale" has two values, 0 and 1. A senator who strongly supports nominee A and weakly supports nominee B cannot express that difference. Both receive the same "approved" mark. This matters in the Act's confirmation context because the degree of preference among a slate of nominees -- all of whom the president has identified as acceptable -- is precisely the information that the Senate's selection process needs to surface. A method that collapses intensity information into a binary signal wastes the most valuable input the slate process could provide.

**Second, it incentivizes bullet voting under strategic conditions.** When Approval Voting is used in multi-winner elections with adversarial participants, the strategically dominant move is to approve only the candidates from your preferred faction and withhold approval from all others. This is identical to binary confirmation's failure mode, reproduced within a multi-candidate framework. An opposition Senate under Approval Voting would simply approve none of the president's nominees, producing the same vacancy outcome as under binary confirmation -- or, in a divided government scenario where the opposition lacks enough votes to block entirely, would approve only the least objectionable nominees without any mechanism for expressing nuanced preference among the rest.

This is not a theoretical concern. The Python Software Foundation used Approval Voting for its Steering Council elections until 2024, when core developer Gregory P. Smith and others concluded that Approval Voting was producing outcomes that did not fully reflect the community's preferences because it could not distinguish between strong support and weak acceptance. The community replaced Approval Voting with Bloc STAR explicitly to capture preference intensity -- the same reason the Act requires Bloc STAR rather than Approval Voting.

### Score Voting (Range Voting)

Pure Score Voting -- in which voters rate candidates on a scale and the highest average or total score wins -- addresses the intensity problem that Approval Voting cannot. A senator who strongly prefers nominee A and weakly accepts nominee B can express that distinction through their scores.

Score Voting's weakness is its vulnerability to bullet voting: voters giving maximum scores to their preferred candidates and minimum scores to all others, regardless of genuine preferences. In an adversarial multi-party setting, bullet voting is individually rational. If every opposition senator gives all presidential nominees a 0 and every majority senator gives them all a 5, the outcome is determined entirely by which party has more senators -- exactly the majority-rules outcome of the status quo, with additional procedural overhead.

STAR voting's automatic runoff phase is specifically designed to address this vulnerability. By requiring a head-to-head comparison between the two finalists, the runoff phase ensures that a nominee who receives maximum scores from a narrow faction but minimum scores from everyone else will lose to a nominee who receives moderate scores from a broad cross-section of the Senate. Pure Score Voting lacks this check.

### Ranked Choice Voting (RCV/IRV)

Ranked Choice Voting has attracted substantial reform advocacy and is the most widely discussed alternative to plurality voting in American public discourse. It has genuine advantages over plurality voting in single-winner races. In the Act's confirmation context, however, it has two disqualifying properties.

**First, RCV is not summable.** Tabulating an RCV election requires centralized access to all ballots simultaneously to perform sequential elimination rounds. Vote tallies from individual precincts cannot be added together to produce a correct aggregate result -- a property that most voting methods, including Bloc STAR, do possess. In a Senate confirmation proceeding, non-summability means the result cannot be independently verified from publicly available score data without access to the full ballot database. Every other Senate vote is a matter of public record that any observer can verify in seconds. An RCV confirmation would be opaque by structural necessity.

**Second, RCV's sequential elimination rounds can produce counterintuitive results and require extensive explanation.** The Condorcet paradox -- in which candidates A beats B, B beats C, and C beats A in pairwise comparisons, producing no clear winner -- is a known failure mode of ordinal systems that RCV does not fully resolve. More practically, a confirmation process that requires senators, their constituents, and the public to understand sequential vote-transfer mechanics and potential elimination-order sensitivity introduces unnecessary complexity into a proceeding that must have legitimate and comprehensible results.

RCV is well-suited to single-winner public elections where its sequential-elimination properties produce more representative results than plurality voting. It is poorly suited to a small-body multi-winner selection proceeding where summability and transparency are essential.

### The Borda Count

The Borda Count assigns points to each rank position (a first-place vote is worth n-1 points, second place n-2, and so on) and selects the candidate with the highest total. It is summable and handles multi-winner elections naturally. Its failure mode is susceptibility to strategic ranking: voters have strong incentives to rank their preferred candidate first and their nearest competitor last, regardless of actual preferences. In an adversarial confirmation context, Borda scoring would quickly collapse into maximally strategic behavior, eliminating the preference-expression benefit that distinguishes it from Approval Voting.

---

## Part III: The Affirmative Case for Bloc STAR

### The Cardinal-Ordinal Hybrid Advantage

Bloc STAR combines the information richness of cardinal scoring with the majority-preference protection of an ordinal runoff. No purely cardinal or purely ordinal method achieves both simultaneously.

The cardinal scoring phase captures what no ordinal method can: the intensity of a senator's preferences across the full slate. A senator who genuinely accepts three nominees and strongly prefers one of them can express that structure through their scores. A senator who finds two nominees excellent and two unacceptable can express that too. The scoring phase does not ask senators to pretend all acceptable nominees are equally acceptable -- it asks them to report their actual preferences as accurately as a 0-5 scale allows.

The ordinal runoff phase then provides a check on the strategic vulnerabilities of pure scoring. If two nominees are closely scored, the runoff determines which one more senators actually prefer when forced to choose between them directly. This prevents a minority faction from gaming the score totals through exaggerated scoring without winning the head-to-head comparison.

Crucially, Bloc STAR is compatible with Arrow's Impossibility Theorem in a way that ordinal methods are not. Arrow's theorem establishes that no ordinal voting method can simultaneously satisfy a set of fundamental fairness criteria -- including transitivity, unanimity, independence of irrelevant alternatives, and non-dictatorship -- when there are more than two candidates. This is not a flaw in any particular ordinal method; it is a mathematical property of the class. Cardinal methods partially sidestep Arrow's theorem because they operate on a different information basis. Bloc STAR's cardinal scoring phase captures utility information that ordinal methods cannot represent, enabling the system to identify broadly preferred outcomes that ordinal elimination sequences might miss.

### Aggregation Mathematics and the Consensus Incentive

The most important structural property of Bloc STAR in the Act's confirmation context is what its aggregation mathematics do to the incentive structure.

Under Bloc STAR, a nominee who receives moderate scores from a broad cross-section of the Senate -- many 3s and 4s from senators of both parties -- can outscore a nominee who receives intense support from one party and maximum opposition from the other. This is not a designed requirement for bipartisanship. It is a mathematical consequence of summing scores across all 100 senators. A nominee with 55 senators scoring them 5 and 45 senators scoring them 0 accumulates 275 stars. A nominee with 55 senators scoring them 3 and 45 senators scoring them 4 accumulates 345 stars. The broadly acceptable nominee wins, not through any explicit mandate but through arithmetic.

This property -- that broad acceptability outscores narrow intensity in aggregate -- is precisely the structural feature the Act's confirmation design requires. The slate is the president's; Bloc STAR is the Senate's mechanism for selecting from among the president's nominees in a way that rewards cross-partisan acceptability without requiring cross-partisan agreement. No alternative method produces this property. Binary confirmation maximizes narrow partisan intensity. Approval Voting cannot distinguish intensity at all. Pure Score Voting produces the same result as Bloc STAR only when no strategic bullet voting occurs -- an assumption that fails under adversarial conditions.

### Public Scoring and Reduced Lockstep Pressure

Binary confirmation maximizes pressure on every senator to vote the party line. A yes or no vote on a single nominee is a test of party loyalty, and senators who cross party lines face unambiguous political exposure. Bloc STAR's multi-nominee scored format reduces this pressure in two reinforcing ways.

First, the comparative nature of scoring makes each individual score a statement about relative preference, not an absolute commitment. A senator who gives a presidential nominee a 2 rather than a 0 is not "approving" that nominee -- they are expressing that this nominee is preferable to a lower-scored alternative. That framing gives senators rhetorical cover that binary confirmation denies them.

Second, the lower stakes per nominee -- each individual score contributes to a multi-nominee evaluation rather than determining the fate of a single candidate -- reduce the political cost of nuanced scoring. A senator can give the president's most moderate nominee a 4, their most ideological nominee a 1, and two intermediate nominees a 2 and 3, respectively, without any single vote becoming a campaign issue. Under binary confirmation, every vote is a dispositive choice; under Bloc STAR, every vote is one data point in a comparative assessment.

Public scoring -- consistent with the public nature of all other Senate votes -- supports the Act's transparency requirements without imposing the political costs that transparency imposes under binary confirmation. The visibility of scored preferences is an accountability feature, not a liability.

### Summability

Bloc STAR is summable: the scores each senator assigns to each nominee can be tallied by any observer with access to the public score record and added together to reproduce the official result without access to a central database. This is a non-trivial property. RCV is not summable; neither are most proportional representation methods. The summability of Bloc STAR means that the Senate's selection from a presidential slate can be verified by any interested party -- a senator's staff, a journalist, a legal challenger -- from the public record alone.

### Why Bloc STAR Specifically, Not Single-Winner STAR or STAR-PR

Within the STAR family, three variants serve distinct purposes. Single-winner STAR is appropriate for executive roles where one person must be selected. STAR-PR (Proportional Representation) is appropriate for legislative bodies where different factions should be represented in proportion to their share of support. Bloc STAR is appropriate for multi-winner elections where the goal is selecting a set of representatives who command broad consensus from the same electorate -- not allocating seats to competing factions.

The Act's confirmation context fits the Bloc STAR use case exactly. The Senate is not a legislature selecting ideological representatives; it is a deliberative body selecting the nominees who command the broadest consensus from a qualified slate. Proportional representation would be structurally wrong: it would guarantee that a faction representing 40% of senators could elect nominees reflecting that faction's preferences regardless of broader acceptability, which is precisely the partisan capture dynamic the Act's architecture is designed to prevent. Single-winner STAR would require the Senate to conduct n separate confirmation proceedings rather than evaluating the full slate together. Only Bloc STAR -- iterative multi-winner selection oriented toward consensus rather than proportionality -- maps onto the Act's requirements.

---

## Part IV: Comparative Institutional Evidence

### The Python Software Foundation: From Approval to Bloc STAR

The most directly relevant real-world precedent for the Act's selection of Bloc STAR over Approval Voting is the Python Software Foundation's Steering Council election process. The Python Steering Council is a five-member governing body elected annually by the Python core development team -- a deliberative community of approximately 106 eligible voters selecting multiple winners in a single proceeding.

Prior to 2024, the Python core team used Approval Voting. The community's experience with Approval Voting produced the same concern the Act's design anticipates: Approval Voting does not allow voters to specify the intensity of their preferences, and outcomes therefore did not reliably reflect the community's genuine judgment about relative candidate quality. Following sustained discussion among core developers, the team formally adopted Multi-winner Bloc STAR voting, codified it into the community's governance document (PEP 13), and used it for the first time in the 2025 Steering Council election.

The structural analogy to the Act's confirmation process is close. Both involve a deliberative body of fixed size selecting multiple winners from a candidate pool in a single proceeding. Both operate in an environment where participants have genuine preferences of varying intensity across a field of qualified candidates. Both require a transparent, summable result that the community can verify independently. Both moved away from simpler methods -- the Python community from Approval Voting, the Act from binary confirmation -- because those simpler methods failed to capture preference information necessary for representative outcomes.

### The Independent Party of Oregon: Cardinal Ballots at Scale

The first binding, multi-jurisdiction use of STAR voting in a public election occurred during the Independent Party of Oregon's 2020 statewide primary. The election covered multiple statewide offices and included over one million eligible voters. Critics had predicted that voters would engage in bullet voting -- scoring only their top candidate at the maximum and all others at zero -- effectively collapsing the system to plurality. The election results disproved this: voters consistently used the middle of the 0-5 scale to express nuanced preferences, providing the differentiated information the system is designed to capture.

This empirical finding addresses a concern that might otherwise be raised about Bloc STAR in the Senate confirmation context: that senators will strategically bullet vote regardless of the method's design. The Oregon evidence suggests that when a scored system is actually used, participants engage with it honestly rather than gaming it to its binary minimum. The automatic runoff phase reinforces this: a senator who bullet votes at 5 for all preferred nominees and 0 for all others sacrifices any influence over which nominees advance in the iterative runoff sequence, because they have provided no information distinguishing among their preferred candidates.

### The Democratic Socialists of America, Los Angeles: STAR-PR vs. Bloc STAR

The Los Angeles chapter of the Democratic Socialists of America used both STAR and STAR-PR for its 2024 internal leadership elections, with a deliberate division of use cases. Single-winner STAR was used for individual leadership roles. STAR-PR was used for the five at-large steering committee seats -- a proportional representation context where factional diversity was an explicit goal.

The chapter's documented experience with this division illustrates the criterion for choosing between STAR variants. When the goal is proportional representation -- seats allocated to factions in proportion to their support -- STAR-PR is appropriate. When the goal is selecting a unified leadership body where all members should command broad support from the full electorate, the iterative consensus-oriented Bloc STAR approach is appropriate. The Act's confirmation context falls squarely in the second category: the Senate is selecting nominees who should command broad support, not allocating confirmation slots to ideological factions.

---

## Part V: Addressing Counterarguments

### "Senators Will Simply Bullet Vote"

The most persistent objection to Bloc STAR in the confirmation context is that strategic bullet voting by a majority party will produce the same partisan outcomes as binary confirmation, making the additional complexity pointless. This objection misunderstands the mechanism's structure under divided government -- the condition where the method matters most.

When the president and Senate majority are aligned, Bloc STAR does not change outcomes relative to binary confirmation: the majority can score the president's nominees highly and opposition nominees at 0, selecting the most ideologically aligned candidates. But when the president and Senate majority are opposed -- divided government, the condition under which obstruction incentives are strongest -- Bloc STAR fundamentally changes the minority's available responses.

Under binary confirmation, an opposition Senate can simply refuse to confirm anyone. Under Bloc STAR, an opposition Senate faces a different choice: bullet vote at 0 for all nominees (triggering the slate rejection mechanism and its costs, as analyzed in the Policy Rationale) or engage with the scoring process and use it to influence which nominees are selected. For opposition senators who genuinely prefer some nominees on the slate to others -- a near-universal condition when the president has submitted a slate of 10 or more qualified candidates -- scoring honestly is individually rational because it influences the outcome. A senator who gives three nominees a 3, two a 1, and five a 0 is not "approving" any of them; they are using their scored influence to tilt selection toward the least objectionable candidates.

Bullet voting is not individually rational under Bloc STAR in the same way it is under binary confirmation. Under binary confirmation, refusing to confirm costs nothing. Under Bloc STAR, refusing to engage with the scoring process surrenders influence over which nominees are selected from among the president's slate.

### "The Method Is Too Complex for a Legislative Proceeding"

A related objection is that Bloc STAR's two-phase mechanism -- scoring round followed by iterative runoffs -- is too complex for senators, their staffs, and the public to understand and trust. This concern conflates the complexity of the tabulation algorithm with the complexity of the ballot.

Senators do not perform the tabulation; they assign scores. Assigning a score of 0 to 5 to each nominee on a slate requires no more cognitive complexity than rating a product on a standard review platform. The tabulation -- identifying the two highest-scoring candidates, comparing them head-to-head, advancing the winner, and repeating -- can be performed by staff with a spreadsheet and verified by any observer with the public score record. The iterative structure produces n winners in n rounds, a sequence that is straightforward to explain and audit.

More complex tabulation algorithms than Bloc STAR are already used in congressional processes. Budget reconciliation requires scoring, classification, and sequencing across thousands of line items. The Bloc STAR tabulation is simpler than any of these.

### "Why Not Just Use Approval Voting, Which Is Simpler?"

The simplicity argument for Approval Voting is addressed at length in Part II and confirmed by the Python Software Foundation's experience. Approval Voting's simplicity is also its limitation: it cannot capture the preference intensity information that makes scored selection superior to binary confirmation in the first place. An Act that replaces binary confirmation with Approval Voting would inherit binary confirmation's core failure mode -- the collapse of all preference distinctions into a binary yes/no signal -- while adding procedural complexity without corresponding benefit.

The Act's design chooses the minimum complexity necessary to achieve the goal. Bloc STAR is more complex than Approval Voting, but it is the minimum complexity required to capture intensity, resist bullet voting through the runoff phase, and produce summable transparent results. The alternatives that are simpler than Bloc STAR fail on at least one critical criterion; the alternatives that are more complex than Bloc STAR add no benefits relevant to the confirmation context.

---

## Conclusion

Bloc STAR is the right voting method for the Act's slate confirmation process because it is the minimum-complexity cardinal-ordinal hybrid that satisfies all four of the confirmation context's structural requirements simultaneously: multi-winner capability, consensus orientation, strategic resilience, and summable transparency.

No simpler method satisfies all four. Binary confirmation fails on all of them. Approval Voting fails on intensity capture and bullet-voting resilience. Pure Score Voting fails on bullet-voting resilience. Ranked Choice fails on summability and transparency. No more complex method adds benefits relevant to this context: proportional methods misalign with the consensus orientation requirement, and more sophisticated cardinal methods add computational opacity without improving the confirmation outcome.

The Python Software Foundation's documented experience replaces Approval Voting with Bloc STAR provides the closest institutional analogue: a deliberative body of fixed size, selecting multiple winners from a qualified field, concluding through working experience that only a method that captures preference intensity can produce genuinely representative outcomes. The Oregon and organizational evidence confirms that scored ballots produce honest, differentiated expression rather than strategic degeneration to plurality behavior.

The Act's use of Bloc STAR is not an arbitrary or borrowed choice. It is the methodologically correct response to the confirmation context's specific requirements -- requirements that no other voting method in the literature satisfies as completely.

---

## Works Cited

Equal Vote Coalition. "Multi-Winner Bloc STAR Voting." starvoting.org. Accessed April 2026. https://www.starvoting.org/multi_winner

Frohnmayer, Mark. "STAR Voting." starvoting.org. Accessed April 2026. https://www.starvoting.org

Independent Party of Oregon. "STAR Voting Announcement." indparty.com. Accessed April 2026. https://www.indparty.com/election-notice

Python Software Foundation. "Changing PEP 13 to Adopt Bloc STAR Voting." discuss.python.org. September 25, 2024. https://discuss.python.org/t/changing-pep-13-to-adopt-bloc-star-voting/64971

Python Software Foundation. "PEP 8107 -- 2026 Term Steering Council Election." peps.python.org. October 2025. https://peps.python.org/pep-8107/

Python Software Foundation. "PEP 13 -- Python Language Governance." peps.python.org. Accessed April 2026. https://peps.python.org/pep-0013/

Smith, Warren D. "Bayesian Regret for Dummies." RangeVoting.org. Accessed April 2026. https://rangevoting.org/BayRegDum.html

---

<!--
## Revision History

**Revision 1.0** (Current)
- Initial publication
-->

*Revision history available in the raw file.*

> [Download this document](https://github.com/albertintech/apai/blob/main/docs/judiciary/fjbaa/the-case-for-bloc-star.md) (opens on GitHub -- click the download button)

*Last revised April 2026*

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
