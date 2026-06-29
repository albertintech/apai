# Building On Ranked Choice Voting

## A Congressional Elections Modernization Act (CEMA) paper in conversation with the ranked choice voting movement

*Prepared by Albert Ramos for The American Policy Architecture Institute*

---

The people who built the ranked choice voting movement have moved American elections farther than any reform effort in a generation. FairVote, RepresentWomen, the League of Women Voters, the ranked choice campaigns in Alaska and Maine, the organizers who carried the method into New York City and dozens of municipalities — they took a better way of counting votes and put it on real ballots, in real elections, where millions of people have now used it. That is the hard part. Most reforms never leave the page.

The Congressional Elections Modernization Act (CEMA) is built on a different counting method, and this paper is honest about that. But the disagreement is narrow and technical, and it sits downstream of a great deal of agreement. CEMA and the ranked choice movement want the same thing and diagnose the same disease. Where they part ways is on one question: which counting method best delivers what both are after. What follows is offered in that spirit — one more contribution to a conversation the ranked choice movement started.

---

## Where American Elections Stand Today

Most American elections run on a choose-one ballot where winners are declared by plurality: mark a single name, and whoever collects the most names wins. That rule records one preference from each voter and nothing else - no backup preferences and no indication of how strongly a voter supports a candidate. In a two person contest, the person with the most votes wins - fair enough, right?

Actually, it is. And that is a strength of choose-one voting: in a two candidate contest, races either end with a majority preference or a tie. This makes choose-one voting the simplest to administer, vote count, and anytime there is not a tie, produce a winner preferred by the majority of participating voters. So far so good.

The major tradeoff for this simplicity is this: our fair majoritarian system becomes something else as soon as a three or more candidates enter the race. Imagine if we have a race between two opposing factions and neither faction will vote for the other's candidate(s). Alice is backed by the Gold faction, then Bill and Carol are backed the Maroon faction. There are 40 Gold voters and 60 Maroon voters. With 100 votes total, one realistic outcome is an Alice win for Gold as long as Maroon voters split their votes between Bill and Carol such that neither candidate gets 41 or more votes. A win under these circumstances means that the winner doesn't represent a majority of voters. This is the potential plurality trap known as vote-splitting.

Since the vote-splitting problem is well known, there are mitigations available to either dampen or eliminate it. These include runoff elections, party primaries, candidate coordination or withdrawal, strategic voting by citizens, and coordination signals around candidate viability. However, none are guaranteed to work. Even under a two-party dominated system like the US, doesn't mean there won't be an independent alternative on the ballot that acts as a 'spoiler' to one of the two major party candidates. The existence of potential spoilers and a citizen's real fear of "wasting" votes on "non-viable" candidates has a chilling effect on party formation - third parties must grow under the shade of one of the two major parties or become irrelevant.

The following figure sums up how plurality voting works:

<iframe
  src="/assets/visualizations/plurality-voting.html"
  width="100%"
  height="700"
  frameborder="0"
  style="border: 1px solid #333; border-radius: 4px;">
</iframe>

Now that we have a solid understanding of Plurality Voting and its major tradeoffs and mitigations, wouldn't it be nice if we could have a way to eliminate both vote-splitting and the spoiler effect, not just dampen them? Enter one response: Ranked Choice Voting.

---

## Ranked Choice Voting Is a Real Improvement on Plurality

Set Ranked Choice Voting beside Plurality Voting and the improvement is immediate.

The choose-one ballot stops listening after one name. The ranked ballot keeps going: it asks the voter to put the candidates in order, first to last, so the count knows not only who a voter most prefers but who they would turn to next, and next after that. When a voter's top choice cannot win, that voter is not simply discarded — their next preference can still speak. That is a genuine advance, and it is why ranked choice has drawn the support it has.

It is also a method with a real operational record. Ranked elections have been run and administered in single-winner contests across the country and abroad, their results certified, their procedures refined through repeated use. This is not a theoretical proposal. It is a working method with working machinery, and the people who built that machinery earned the credibility it carries.

How does Ranked Choice Voting work, exactly?

---

## How Ranked Choice Voting Works

To see how Ranked Choice Voting (RCV) achieves its desireable qualities such as eliminating spoilers and vote-splitting, it helps to look at RCV as a machine with separable parts. Every voting method has two main components to do two distinct jobs: a way to collect voter preferences as information and a way to process that information to produce a winner.

The first component is the **ballot** — the input. It is the format the voter fills out, and it determines what information the method collects. The second part is the **counting rule** — the procedure that takes a stack of those ballots and produces a winner. The ballot is what the voter hands over; the counting rule is what the method does with it. The same kind of ballot can, in principle, be handed to different counting rules, which is exactly the possibility this paper will reach for later.

Ranked choice voting pairs a ranked ballot with a specific counting rule called **instant-runoff voting (IRV)** — the algorithm most people mean when they say "ranked choice." Here are its two parts:

<iframe
  src="/assets/visualizations/rc-voting.html"
  width="100%"
  height="700"
  frameborder="0"
  style="border: 1px solid #333; border-radius: 4px;">
</iframe>

The counting rule is the part to watch. It works by **sequential elimination**: count first choices, drop the last-place candidate, transfer that candidate's ballots to each voter's next surviving choice, and repeat until someone holds more than half. This is the engine running. And running this way produces three consequences worth understanding before choosing it.

<iframe
  src="/assets/visualizations/irv-flowchart.html"
  width="100%"
  height="1000"
  frameborder="0"
  style="border: 1px solid #333; border-radius: 4px;">
</iframe>

## Tradeoffs of Using Sequential Elimination

They are not malfunctions — the method is behaving exactly as designed. They are properties of the design, and they have names in the election-methods literature, where the family is sometimes called the method's [pathologies](https://example.com/pathology-citation). The plainer label is what this paper will use: these are **structural consequences** of counting by elimination.

All three share a common thread. Each is a way the count can fail to reflect what voters actually marked on their ballots — and each enters through the same part, the elimination procedure.

**Support can backfire.** Ordinarily, more support helps a candidate. Under sequential elimination, it can sometimes do the opposite: giving a candidate *more* first-choice support can, in certain configurations, cause that candidate to lose a race they would otherwise have won. The reason is that added first-choice support changes who gets eliminated in an earlier round, and that change reshuffles how every later ballot transfers. The literature calls this a **monotonicity failure**. It is real, it is documented, and it is also genuinely uncommon and hard to spot — but it follows from the elimination procedure, not from any mistake by voters or officials.

**A broadly liked candidate can be eliminated early.** Sequential elimination decides who to drop by counting first choices, and only first choices. A candidate who is the broadly acceptable second or third choice of most of the electorate — the candidate a majority might be content to live with — can hold very few *first*-choice rankings, and so be dropped in an early round, before the rounds that would have revealed that broad support. The count rewards concentrated first-choice support, not broad acceptability, and a candidate strong on the second measure but weak on the first does not survive to be counted. This is **center squeeze**.

**A ballot can run out of choices.** A voter ranks the candidates they have an opinion about. If every candidate that voter ranked is eliminated, the ballot has no next choice left to transfer to, and it is set aside for the remainder of the count. The voter showed up and marked a sincere ranking, but once their ranked candidates are gone, the ballot has nothing left to say, and the final rounds that decide the seat proceed without it. This is **ballot exhaustion**, and it follows from the elimination procedure meeting a ballot that — like nearly every real ballot — ranked fewer than all the candidates.

These three are the engine's behavior, stated plainly. A reader who prefers ranked choice after understanding them is entitled to that view, and the next section is part of why.

---

## The Mitigations Ranked Choice Has Developed

The ranked choice movement is not unaware of any of this. A method with a long record of practice and decades of academic study has accumulated real responses, and they deserve a fair hearing.

For ballot exhaustion, the most direct response is to let voters rank more candidates. Where early ranked ballots capped voters at three or five rankings, longer ballots — or ballots that let voters rank every candidate — give each ballot more next-choices to fall back on, so fewer run out. Alongside that, sustained voter education encourages people to rank deeper rather than stopping at one or two names, which keeps more ballots alive through more rounds. Jurisdictions have tuned ballot rules — minimum and maximum ranking allowances, ballot design, field-size management — to reduce the rate at which ballots are set aside. These are genuine improvements, and they have measurably reduced exhaustion where applied.

What unites every one of these responses is where it operates. Each works on the *input* to the count — how many candidates a voter may rank, how well voters understand the ballot, how the field is shaped before counting begins. None changes the counting rule itself. The elimination procedure that produces the three consequences runs exactly as before; the mitigations work around it, adjusting what flows into the engine rather than altering the engine. That is not a criticism of the mitigations. It is an observation about their reach.

---

## A Better Engine, or a Better Patch?

Engines improve over time. A modern one delivers more power from less fuel, runs cleaner, and fits in a smaller space than its ancestor of a century ago — not because someone kept bolting accessories onto the old design, but because the design itself was rethought.

The sequential-elimination count is, in its essentials, a nineteenth-century design. The mitigations of the previous section are real, but they are accessories bolted onto that design: longer ballots, better voter education, tuned rules. Each helps. None reaches the counting rule that produces the consequences in the first place. So the honest question is the one an engineer would ask. Is the field limited to patching the old engine — or is there a different one, a counting rule that does not produce these consequences because it never runs the elimination procedure that causes them?

There is. It begins by changing the part the mitigations never touch.

---

## A Scored Engine

Recall that a voting method has two separable parts, the ballot and the counting rule. The mitigations of the previous section all worked on the ballot and never touched the counting rule. A scored engine starts at the other end. It changes the ballot, and then it changes the counting rule itself — the part elimination's accessories never reached.

Begin with the simplest version, score voting, also called range voting:

<iframe
  src="/assets/visualizations/score-voting.html"
  width="100%"
  height="440"
  frameborder="0"
  style="border: 1px solid #333; border-radius: 4px;">
</iframe>

The voter scores every candidate on a fixed scale — zero to five, the same rating tens of millions of Americans give to products and restaurants. The counting rule then does one thing: add up each candidate's scores across every ballot, and the highest total wins. There is no elimination, no transfer, no round-by-round dropping of candidates. The engine adds rather than eliminates.

Look at what changing the counting rule buys. Because nothing is ever eliminated, none of the three structural consequences from the ranked engine has a procedure to enter through. There is no elimination order, so support cannot backfire. Broad support is weighed directly in the sum, so a broadly liked candidate is not dropped for holding few first-choices — center squeeze does not occur. And no ballot is ever transferred from an eliminated candidate, so no ballot runs out of choices and gets set aside — there is nothing to exhaust. The whole family of consequences that came from counting by elimination is simply absent, because the engine does not count by elimination.

That is the upside, and it is a large one. But every engine has consequences that fall out of its design, and intellectual honesty requires asking the same question of this engine that the paper asked of the ranked one: what comes downstream of *this* design?

---

## What the Scored Engine Brings With It

Score voting's consequences are real, and the scored-voting community has never pretended otherwise. They cluster around one thing: how a voter decides what to write on the ballot.

**Bullet voting.** A voter who cares most about their favorite winning may give that candidate the top score and give everyone else a zero — even candidates they actually find acceptable — to avoid lifting a rival's total. The ballot allows nuance; the strategic incentive discourages using it.

**Burial.** A voter may give the strongest rival a zero rather than an honest middling score, deliberately sinking that rival's total to clear a path for their favorite. The honest score and the strategic score come apart.

**Min-maxing.** Generalizing both, a voter may abandon the middle of the scale entirely — every candidate gets either the maximum or the minimum, never a three or a four — because the extremes carry more strategic weight than honest gradations.

A careful reader should notice what kind of problem this is, because it is not the same kind the ranked engine had. Support backfiring, center squeeze, and ballot exhaustion are failures of the *count itself* — ways the engine can fail to reflect what voters actually marked on their ballots. Bullet voting, burial, and min-maxing are not failures of the count. The scored count reflects exactly what voters marked; the question is only whether voters mark their honest opinions or strategically distorted ones. One family of problems lives in the machine. The other lives in the incentive a voter faces while filling out an honest ballot.

These are different problems on different levels, and an honest reckoning sees that the levels are not equal. The ranked engine's consequences sit deeper — in the count — and they are not hypothetical. A ranked election in Burlington, Vermont produced a monotonicity failure in a real mayoral race, and a 2022 ranked congressional election in Alaska eliminated a broadly preferred candidate through center squeeze. These are not models. They happened, in public, and they became the material for repeal. Score voting's strategic incentives, by contrast, are real but a scale down: they pressure how a voter fills out a ballot, not whether the count honors what was filled out.

None of which means the strategic incentives should be waved away. The scored-voting community did not wave them away, any more than the ranked-choice community ignored exhaustion. Both developed mitigations. The difference — and it is the difference this paper has been building toward — is *where the mitigation lands.*

---

## Where the Mitigation Lands

Look again at how the ranked engine was mitigated. Every fix landed on the ballot and the voter: cap the rankings, expand the rankings, redesign the ballot, educate the voter to rank deeper. The counting rule stayed exactly as it was, and the burden of coping with it was distributed outward, onto ballot rules and onto voters asked to behave in the ways the engine needed.

The scored engine can be mitigated at the other end — on the counting rule itself. Add a second step to the count: after summing the scores, take the two highest-scoring candidates and hold an automatic runoff between them, where each ballot counts as a full vote for whichever of the two finalists it scored higher. The candidate preferred by more voters, head to head, wins.

That single change to the counting rule blunts the strategic incentives at their source. Burying an honest rival or min-maxing the scale loses much of its payoff, because the final decision is no longer the raw sum a voter was trying to game — it is a head-to-head majority comparison between the top two, where an honestly higher score and a strategically maximal score count the same. The incentive to distort is reduced not by a rule imposed on the voter, but by the structure of the count. No ballot caps. No mandatory ranking depth. No campaign to train voters out of voting the way the engine rewards. The mitigation is in the engine.

This is scoring with a built-in runoff, and it has a name: **STAR — Score Then Automatic Runoff.**

<iframe
  src="/assets/visualizations/star-voting.html"
  width="100%"
  height="440"
  frameborder="0"
  style="border: 1px solid #333; border-radius: 4px;">
</iframe>

STAR is the scored engine with its primary weakness addressed where the weakness lives. The voter still scores every candidate zero to five, exactly as in plain score voting — the ballot does not get harder. The counting rule does the additional work: sum the scores to find the two finalists, then decide between them by majority preference. The runoff step carries a second, modest virtue worth naming: because the final step is a head-to-head between two finalists, the count can be tallied locally, precinct by precinct.

None of this abolishes strategy from voting — no method does, and a paper that claimed otherwise would forfeit the honesty it has tried to keep. A voter still faces a question about how high to score a tolerable alternative to their favorite. But the pressure is reduced, and reduced from inside the count rather than patched from outside it. That is the case for the scored engine: not that it is perfect, but that its remaining weakness is the milder kind, and that the fix for it lands on the engine instead of on the voter.

---

## Where a Reasonable Person Might Still Choose Ranked Choice

A fair paper does not pretend the choice makes itself. Several good-faith positions can lead a thoughtful person to prefer ranked choice even after weighing everything above.

The first is the weight of experience over models. Ranked choice has a substantial real-world record in single-winner American elections; STAR's advantages, real as they are, are demonstrated heavily through analysis and simulation and a thinner record of live governmental use. A reformer who trusts what has been run at scale over what models predict can reasonably weight that record heavily.

The second is the ballot itself. Ranking candidates is an intuitive task — first, second, third — and some voters and election officials may find it more natural than scoring on a scale. A method's merits on paper matter less if voters find the ballot harder to use, and reasonable people can judge that tradeoff differently.

The third is momentum. Ranked choice has organizations, legislation, a body of administrative experience, and years of advocacy behind it. A reformer who believes the practical path to *any* better method runs through the movement already in motion can reasonably choose to build on that momentum rather than start a newer method's climb.

These are real arguments, honestly held. CEMA reaches a different conclusion, but not because the people who reach the opposite one have failed to think it through.

---

## Where CEMA Stands

CEMA shares the ranked choice movement's goal completely: a counting method that listens to more than a single name and produces winners who genuinely reflect what voters wanted. The disagreement is only about which engine does that best.

Between the engines this paper has set side by side, CEMA's judgment is that the scored engine, with its built-in runoff, is the better foundation. The reason is the difference in *kind* the paper kept returning to. The ranked engine's consequences live in the count itself — they are ways the elimination procedure can fail to carry a voter's marked preferences through to the result, and they have surfaced in real elections. The scored engine's weakness lives one level up, in the incentive a voter faces while marking the ballot, and STAR addresses it where it lives, inside the counting rule, rather than by pushing rules and burdens back onto the voter. Neither engine is perfect. But weighing the deeper problem against the milder one, and weighing a fix that lands on the engine against fixes that land on the voter, CEMA chose the scored engine. That is not a verdict on the ranked choice movement, whose achievement made this entire conversation possible. It is a judgment about engines — and an invitation to weigh the same parts CEMA weighed, and to keep building toward elections that listen to everything a voter has to say.

---

## Works Cited

*[To be completed.]*

---

<!--
## Revision History

**Revision 6.4** (Current)
- Initial publication of "Building On Ranked Choice Voting," second entry in the Building On series (after Building On Fusion Voting)
- Scope: single-winner IRV vs. single-winner STAR only. No proportional versions of either method, no Fair Representation Act framing, no two-engine scaffold. Single ranked engine against single scored engine, head to head
- Audience: the ranked choice voter with low-to-no voting-science background; every mechanic taught, not assumed
- Spine: credit the movement → shared diagnosis → ranked choice as a real improvement on plurality → teach three structural consequences neutrally (monotonicity failure / center squeeze / ballot exhaustion), all entering through sequential elimination, no CEMA verdict in the survey → grant the ranked-engine mitigations honestly (all operate on the ballot/input, not the counting rule) → the engine question (new engine or only patches?) → the scored engine in three beats: (a) plain score voting as its own engine, stating what changing the counting rule buys (the three elimination consequences are absent); (b) what the scored engine brings downstream — bullet voting, burial, min-maxing, taught as strategic incentives, with the careful-reader beat that these are a different and milder KIND of problem than the ranked pathologies (count-level vs. ballot-marking-level), glancing Burlington/Alaska cites as real-world evidence of the deeper kind; (c) where the mitigation lands — ranked fixes land on the voter/ballot, the scored fix lands on the counting rule itself, and that fix IS STAR, arriving as scoring-plus-runoff rather than introduced cold → honest concession (where a reasonable person might still choose RCV) → CEMA's judgment, landed once, at the close, turning on the difference in kind (deeper problem vs. milder, fix-on-engine vs. fix-on-voter)
- Even-handedness is now structural: the scored engine gets the SAME three-part treatment the ranked engine got — engine shown, downstream consequences named honestly, mitigation examined — so STAR is earned rather than presented. Plain score voting is introduced first and on its own; STAR appears only as the mitigation
- Burlington/Alaska boundary with "Why Not a Ranked Method?": glancing one-line factual cites permitted here as evidence that the ranked engine's problems are count-level and have detonated in real elections; the detailed blow-by-blow case studies remain exclusive to Why Not. This paper names them; Why Not prosecutes them
- Non-summability considered and dropped: an administrative/auditing consequence rather than a fidelity one (category mismatch with the other three), and CEMA's own Proportional STAR is non-summable, so deploying it as a defect here would contradict the later multi-winner case. STAR's single-winner summability retained only as a one-clause positive virtue in §7. Belongs in the exhaustive VME Structural Consequences treatment, not in this pointed paper
- "Candidate-centered" dropped from the strengths section: that virtue does work only as a contrast to party-list PR, which is out of scope here
- Terminology per the VME RCV language guide: "structural consequences" as the running term, "pathologies" tagged once with citation link; "monotonicity failure" not "non-monotonicity," with "support backfiring" as the recurring layperson handle; two-part engine framing (ballot + counting rule), with IRV as the counting rule and "RCV" pinned to the package, never drifting to the ballot-type category
- Posture boundary with the planned "Why Not a Ranked Method?" position paper: this paper STATES and TEACHES the consequences neutrally and reaches a single closing judgment; the prosecutorial treatment — explicit no-drops hierarchy, load-bearing weight on exhaustion, Burlington/Alaska case studies — is held exclusive to Why Not. CEMA's judgment appears only in the closing section
- Voice: primer-adjacent. Instructional second person, flat verdicts, no staged connectives, no self-narration. Warmth structural (living in credit and concession), not carried by prose rhythm
- Two inline engine diagrams replaced by three: RCV/IRV (§4), plain score voting (§7, "A Scored Engine"), and STAR (§9, "Where the Mitigation Lands"), all themed via the shared --diagram-* variables in stylesheets/extra.css. Marker IDs made unique per diagram (arrow / arrow-score / arrow-star) to avoid duplicate-ID collision across three SVGs on one page
- DPS 3.7 Building On series compliance: own-title H1; "in conversation with the [reform] movement" subtitle form; "the Act" convention suspended (CEMA used by name throughout); supporting-document footer (no attribution line); Works Cited required (Position Paper-adjacent; populated before publication)
- Aligned with Rev 6.4 of the CEMA legislative text
-->

*Revision history available in the raw file.*

> 📥 [Download this document](https://github.com/albertintech/apai/blob/main/docs/congress/cmf/cema/building-on-ranked-choice-voting.md) (opens on GitHub -- click the ⬇ download button)

---

*© 2026 Albert Ramos | American Policy Architecture Institute*
