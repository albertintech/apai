# Why Not Condorcet?

## A Position Paper on the Structural Limitations of True Majority Rule and the Case for STAR Voting as a Single-Winner Method

### Published March 2026

Based on Rev 5.2 of the Federal Elections Modernization Act

---

The Condorcet criterion -- the principle that if a candidate would defeat every other candidate in a one-on-one majority comparison, that candidate should win -- is one of the most intuitively compelling ideas in voting theory. A candidate preferred by a majority over each alternative has a strong democratic claim to office. No serious electoral reformer disputes this.

The question is not whether the Condorcet criterion is desirable. The question is whether a voting system built around satisfying that criterion -- using ranked ballots and pairwise comparison as its primary counting logic -- is the best available single-winner method for American federal elections. The Federal Elections Modernization Act (FEMA), hereafter referred to as "the Act," uses STAR voting (Score Then Automatic Runoff) rather than any Condorcet-compliant method. This paper explains why.

The case for Condorcet methods -- often called "true majority rule" (TMR) in the Dasgupta-Maskin literature -- rests on a rigorous axiomatic framework developed over two decades by Partha Dasgupta and Eric Maskin, extended into practical reform proposals by Edward Foley and Wesley Holliday. This paper engages that framework at its strongest. It does not argue that Condorcet methods are bad. It argues that STAR is a better fit for the structural role it plays in the Act's architecture, and that the theoretical case for Condorcet's superiority depends on assumptions and omissions that the practical design context cannot sustain.

---

## What Condorcet Methods Are

A Condorcet method is any voting system that guarantees the election of the Condorcet winner -- the candidate who defeats every other candidate in head-to-head pairwise comparisons derived from voters' ranked ballots -- whenever such a winner exists.

The ballot is a ranking: voters order candidates from most preferred to least preferred. From these rankings, the system constructs a pairwise comparison matrix. For every pair of candidates A and B, the system counts how many voters ranked A above B and how many ranked B above A. If one candidate defeats all others in these pairwise contests, that candidate is the Condorcet winner.

When no Condorcet winner exists -- because preferences cycle (A beats B, B beats C, C beats A) -- a completion method is required to identify a winner. Different Condorcet methods use different completion rules: Minimax selects the candidate whose worst pairwise loss is smallest; Ranked Pairs locks in the strongest pairwise results and discards weaker ones that would create cycles; Schulze (Beatpath) traces indirect chains of pairwise victories; the Holliday-Maskin "smallest loss" rule, designed for Final Four elections, selects among candidates with at most one loss the one whose loss margin is narrowest.

The Condorcet family shares a ballot format (ranked) and a primary counting logic (pairwise majority comparison). Members differ only in their cycle-resolution rules. The axiomatic arguments advanced by Dasgupta and Maskin apply to the family as a whole, not to any single variant.

---

## The Strongest Case for Condorcet

Intellectual honesty requires engaging with the best version of the Condorcet argument, not a strawman. The case for TMR rests on several genuine strengths.

The axiomatic foundation is formidable. Dasgupta and Maskin (2008) proved the "majority dominance theorem": whenever any voting system satisfies anonymity, neutrality, the Pareto principle, independence of irrelevant alternatives, and decisiveness on a given class of preference domains, majority rule also satisfies those axioms on that domain -- and majority rule satisfies them on some domains where other systems do not. In 2020, they strengthened this to a uniqueness result: adding strategy-proofness to the axiom set uniquely characterizes majority rule on any domain where a satisfying rule exists. These are not minor results. They establish that within the ordinal framework, Condorcet is the best available method by a wide margin.

The immunity to specific pathologies is real. Condorcet methods satisfy monotonicity (giving a candidate more support never causes them to lose), are immune to center squeeze (a broadly preferred centrist cannot be eliminated before reaching the final comparison), and satisfy the independence of irrelevant alternatives in a way that neither plurality, RCV, nor the Borda count can. These are the pathologies that have caused documented failures in real elections -- Burlington 2009, Alaska 2022 -- and Condorcet methods would have produced the broadly preferred winner in both cases.

The "Maximum Convergence Voting" framing advanced by Foley and Maskin (2025) positions Condorcet within American constitutional theory, arguing that the Condorcet criterion aligns with the Madisonian goal of preventing factional capture and identifying candidates with the broadest possible electoral support. This is a politically resonant argument, not merely a mathematical one.

The Condorcet criterion is a good criterion. The question is whether satisfying it requires building the entire electoral system around it.

---

## Why Condorcet Falls Short

### The Strategy-Proofness Gatekeeping Argument

The centerpiece of the Dasgupta-Maskin case against cardinal methods is the claim that strategy-proofness implies ordinality: if voters can gain by misrepresenting their preferences, and cardinal scores are more manipulable than ordinal rankings, then only ordinal information can serve as reliable electoral input. This eliminates Approval, Score, and STAR from consideration before the comparison begins.

The argument is formally valid within its axiom set. It is also selectively applied. The Gibbard-Satterthwaite theorem (1973/1975) establishes that every deterministic, non-dictatorial voting system with three or more candidates is susceptible to strategic manipulation. Condorcet methods are no exception. Voters can bury strong competitors by ranking them dishonestly low. Voters can compromise by ranking a second choice above their true favorite when they believe their favorite cannot win. These are not theoretical curiosities -- they are the same strategic dynamics that exist under any ranked system.

What the Dasgupta-Maskin theorem actually shows is narrower than its rhetorical deployment suggests: cardinal systems have one additional dimension of strategic vulnerability (score exaggeration) beyond the ordinal manipulation that all systems share. This is a real observation. But it does not establish that ordinal systems are strategy-proof -- only that they have a smaller strategic attack surface. Applying a standard that no system meets to disqualify one class of systems while exempting another is a framing choice, not a mathematical necessity.

### The Preference Intensity Problem

Ordinal rankings capture the order of preferences but not their strength. A voter who slightly prefers Alice over Ben and a voter who passionately prefers Alice over Ben contribute identically to Alice's pairwise margin. This is a deliberate design choice in the Condorcet framework -- Maskin argues that preference intensity is subjective, interpersonally incomparable, and strategically unreliable.

The Act rejects this argument. Preference intensity is real information that voters possess and that affects democratic outcomes. The voter who rates Alice 5 and Ben 4 is expressing something meaningfully different from the voter who rates Alice 5 and Ben 1, and a voting system that treats these expressions identically is discarding data that bears on which candidate best represents the electorate.

The concern that intensity information is strategically unreliable assumes the worst case: that voters will universally exaggerate to the scale endpoints, collapsing cardinal scoring into binary approval. Under pure Score voting, this concern has empirical traction. Under STAR, the automatic runoff creates a structural deterrent to exaggeration. A voter who zeros out a tolerable compromise candidate risks excluding that candidate from the top two, potentially producing a worse runoff matchup. The Pivotal Voter Strategic Incentive (PVSI) modeling by Wolk, Quinn, and Ogren (2023) found that the peak strategic incentive under STAR is approximately 2%, confined to "honest inflation" -- mild exaggeration that preserves the voter's true preference order. Dishonest strategies (favorite betrayal, burial, bullet voting) are all strongly disincentivized.

The Dasgupta-Maskin framework evaluates strategy-proofness as binary: satisfied or violated. It has no mechanism for evaluating the magnitude of strategic incentives or the behavioral likelihood that voters will exploit them. A 2% incentive for preference-order-preserving exaggeration and a 100% incentive for outright dishonesty are treated identically -- both "violate" strategy-proofness. This binary lens is appropriate for proving theorems. It is not appropriate for designing elections.

### The Field Size Problem

Pairwise comparisons scale quadratically with the number of candidates. Four candidates produce 6 pairwise matchups. Ten produce 45. Fifteen produce 105. Each matchup requires the voter to have expressed a preference between those two candidates, which means the ranked ballot must contain a complete or near-complete ordering.

Asking voters to rank four candidates is cognitively manageable. Asking them to meaningfully rank ten or fifteen -- the candidate field sizes that open, nonpartisan elections routinely produce -- is the exact cognitive burden problem that the empirical literature has documented for ranked systems. Incomplete rankings are the observed norm in large-field ranked elections, and each incomplete ballot degrades the pairwise comparison matrix. A voter who ranks only their top three out of fifteen candidates provides preference information for three matchups out of 105. The system must either treat unranked candidates as tied-for-last (an assumption, not data) or treat the comparison as missing (weakening the majority finding). Either way, the information that the system needs to identify the Condorcet winner becomes unreliable as the field grows.

This is why the most developed practical Condorcet proposals are designed for small candidate fields. The Holliday-Maskin "smallest loss" rule was designed specifically for Final Four elections -- four candidates maximum. The Foley-Maskin (2025) "Maximum Convergence Voting" proposal pairs a Condorcet general election with a nonpartisan open primary that narrows the field to three finalists. The field-size limitation is not incidental to these proposals; it is structural.

### The Primary Dependency

If Condorcet methods require a preliminary filter to manage candidate field size, then the design question shifts: what method should the preliminary filter use?

The Foley-Maskin proposal uses a nonpartisan open primary, but does not specify a voting method for that stage in detail. Alaska's existing Final Four system uses a pick-one plurality primary. This means the preliminary filter -- the stage that determines which candidates TMR gets to evaluate -- is itself subject to all the pathologies that TMR exists to solve: vote-splitting, spoiler effects, the failure of independence of irrelevant alternatives. The theoretically optimal method depends on a structurally inferior method to select its inputs.

One could propose using a Condorcet method for the primary as well. But this reintroduces the field-size problem at the primary stage, where candidate fields are largest. Alternatively, one could propose using STAR or Approval voting for the primary -- but this concedes that cardinal methods are suitable for at least some electoral contexts, undermining the ordinal-supremacy argument.

The Act sidesteps this dependency entirely. STAR's scoring interface scales linearly with candidate field size: each candidate is evaluated independently on a 0-5 scale, regardless of how many others appear on the ballot. A voter who knows five candidates well scores those five and leaves the rest at zero. The cognitive burden does not compound the way ranking does. This is what enables the Act's Unified General Election Structure (UGES) -- the elimination of state-administered primaries for federal offices. STAR handles the full candidate field in a single stage. No preliminary filter is required, and no inferior method needs to do the work that the primary system was designed for.

### The Proportional Representation Gap

The Act does not use STAR solely for single-winner elections. It uses STAR-PR (Allocated Score) for multi-member House elections, producing proportional representation. The same 0-5 scoring ballot serves both single-winner Senate/Presidential contests and multi-winner House contests. This ballot-format consistency is a deliberate design feature: voters learn one interface and use it across all federal elections.

Condorcet methods have no natural proportional extension. The pairwise comparison logic that identifies a single Condorcet winner does not generalize to multi-winner proportional allocation. Proportional ranked methods exist (STV/PRCV), but they use an entirely different counting logic -- sequential elimination and surplus transfer -- that shares none of Condorcet's axiomatic properties. A reform architecture built on Condorcet for single-winner elections and STV for multi-winner elections would require voters to learn two different counting logics, use the same ranked ballot for fundamentally different purposes, and accept that the proportional method does not satisfy the Condorcet criterion that justified the single-winner method.

The Act's architecture avoids this incoherence. STAR and STAR-PR share a ballot format, a scoring logic, and a design philosophy: capture preference intensity, aggregate it transparently, and produce results that reflect the electorate's preferences. The single-winner and multi-winner methods are variations on the same mechanism, not unrelated systems that happen to share a ballot.

### Twenty Years Without Adoption

TMR's theoretical development began with Dasgupta and Maskin's 2004 Scientific American article and has been refined through publications in 2008, 2020, and 2025. In that time, no government at any level -- federal, state, local, or foreign -- has adopted any Condorcet method for public elections. This is not because the theory is wrong. It is because the practical barriers are real: perceived tabulation complexity, the need for a preliminary filter to manage field size, the lack of a natural proportional extension, and the absence of an institutional champion with the political infrastructure to drive adoption.

By contrast, STAR voting has been adopted for local elections in Oregon, has an active advocacy coalition (the Equal Vote Coalition), uses a ballot interface (star ratings) that maps onto everyday consumer behavior, and produces results that are auditable, deterministic, and explainable in a single sentence: "the two highest-scoring candidates go to an automatic runoff, and the one preferred by more voters wins."

Theoretical optimality that cannot be implemented is not optimality in any practical sense. The Act is designed to be enacted, administered, and sustained -- not to satisfy axioms.

---

## The Affirmative Case: STAR

The Act selects STAR voting for single-winner federal elections because it satisfies the practical requirements that Condorcet methods struggle with, while achieving comparable or superior democratic outcomes across the dimensions that matter most.

STAR captures preference intensity without requiring strategic sophistication. The 0-5 scoring scale is a familiar interaction -- people rate products, restaurants, and services on star scales routinely. The ballot action is identical regardless of candidate field size. No ranking is required, no transitivity is demanded, and a voter who knows only three candidates in a ten-candidate field scores those three and leaves the rest at zero without penalty.

STAR satisfies monotonicity: giving a candidate a higher score never causes them to lose. STAR avoids ballot exhaustion: every scored ballot contributes to the outcome through every phase of tabulation. STAR reduces strategic incentives to empirically negligible levels: the PVSI research finds a 2% peak incentive for mild, preference-order-preserving exaggeration, with dishonest strategies strongly disincentivized.

STAR's two-stage structure -- scoring to determine finalists, automatic runoff to determine the winner -- ensures that the winner has both broad aggregate support (reflected in advancing to the top two) and majority preference against the other finalist (reflected in winning the runoff). This is not the Condorcet criterion, but it is a meaningful majority-confirmation mechanism that applies to every election, not only those where a Condorcet winner happens to exist.

STAR enables the Act's Unified General Election Structure by tolerating large candidate fields without degradation. And STAR-PR extends the same ballot format and scoring logic to proportional representation, providing architectural coherence across all federal elections.

---

## Conclusion

The Condorcet criterion identifies a real and important property of electoral outcomes. When a candidate would defeat every other candidate head-to-head, that candidate has a strong claim to democratic legitimacy. Nothing in this paper disputes that principle.

But satisfying the Condorcet criterion as a system-level guarantee requires building the electoral architecture around ranked ballots, pairwise comparison matrices, and completion methods for cycles. That architecture discards preference intensity information, scales poorly with candidate field size, depends on a preliminary filter that reintroduces the pathologies it exists to solve, has no natural proportional extension, and has failed to achieve adoption in any public election in over two hundred years of theoretical development.

STAR voting does not guarantee the Condorcet winner. But it captures more information from voters, handles larger candidate fields, requires no preliminary filter, extends naturally to proportional representation, and produces outcomes that the simulation literature consistently ranks at or near the top of all evaluated methods. Its strategic vulnerability is empirically bounded and behaviorally negligible. Its ballot interface is familiar, its tabulation is transparent, and its results are auditable.

The Act's position is that a system which works well across all the dimensions that matter -- expressiveness, scalability, strategic resistance, proportional extensibility, administrative simplicity, and political durability -- is preferable to a system that achieves theoretical perfection on one dimension while requiring workarounds on every other. The standard for evaluation is not axiomatic purity. It is structural fitness for the role the voting method must play in an integrated federal electoral architecture.

Condorcet methods are theoretically admirable. STAR is architecturally superior.

---

## Works Cited

Dasgupta, Partha, and Eric Maskin. "The Fairest Vote of All." *Scientific American* 290, no. 3 (March 2004): 92-97.

Dasgupta, Partha, and Eric Maskin. "On the Robustness of Majority Rule." *Journal of the European Economic Association* 6, no. 5 (2008): 949-973.

Dasgupta, Partha, and Eric Maskin. "Strategy-Proofness, Independence of Irrelevant Alternatives, and Majority Rule." *American Economic Review: Insights* 2, no. 4 (December 2020): 459-474.

Foley, Edward B., and Eric Maskin. "Condorcet Voting." Working paper, Harvard University and Ohio State University, March 2025. https://maskin.scholars.harvard.edu/sites/g/files/omnuum10606/files/condorcet_voting_e.maskin_e.foley_march_2025_0.pdf

Gibbard, Allan. "Manipulation of Voting Schemes: A General Result." *Econometrica* 41, no. 4 (1973): 587-601.

Graham-Squire, Adam T., and David McCune. "An Examination of Ranked-Choice Voting in the United States, 2004-2022." *Representation* 61 (2023): 1-19.

Holliday, Wesley H. "A Simple Condorcet Voting Method for Final Four Elections." *Representation* (2025). https://www.tandfonline.com/doi/full/10.1080/00344893.2025.2473397

Ramos, Albert E. *Federal Elections Modernization Act, Rev 5.2*. The American Policy Architecture Institute, February 2026.

Satterthwaite, Mark Allen. "Strategy-Proofness and Arrow's Conditions: Existence and Correspondence Theorems for Voting Procedures and Social Welfare Functions." *Journal of Economic Theory* 10, no. 2 (1975): 187-217.

Wolk, Sara, Jameson Quinn, and Mark Ogren. "STAR Voting, Equality of Voice, and Voter Satisfaction: Considerations and Simulations." *Constitutional Political Economy* 34 (2023): 301-325.

---

<!--
## Revision History

**Revision 1.0** (Current)
- Initial publication
- Evaluates Condorcet/TMR family against STAR as single-winner method for the Federal Elections Modernization Act
- Engages the Dasgupta-Maskin axiomatic framework (2004, 2008, 2020), the Foley-Maskin "Maximum Convergence Voting" proposal (2025), and the Holliday "Final Four" simplification (2025)
- Identifies five structural limitations: strategy-proofness gatekeeping, preference intensity loss, field-size scaling, primary dependency, and proportional representation gap
- Draws on Wolk Quinn and Ogren 2023 (PVSI strategic incentive modeling), Gibbard 1973 and Satterthwaite 1975 (universal strategic vulnerability), Graham-Squire and McCune 2023 (empirical RCV data), and the Equal Vote Coalition analytical framework
- Classified as Position Paper per APAI Document Production Standards Rev 2.4
-->

*Revision history available in the raw file.*

> [Download this document](https://github.com/albertintech/apai/blob/main/docs/congress/cmf/fema/why-not-condorcet.md) (opens on GitHub -- click the download button)

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
