# Federal Elections Modernization Act

## STAR Voting and Allocated Score: A Technical Explainer

### Published February 2026

Based on Rev 5.0 of the Federal Elections Modernization Act

---

## Purpose

This document explains how votes are counted under the Federal Elections Modernization Act (FEMA), hereafter referred to as "the Act." It covers both voting methods used in federal elections:

1. **STAR Voting** -- used when one person is being elected (President, Senate, and some House races).
2. **Allocated Score** -- used when multiple people are being elected from the same district (most House races).

**This document is written for voters.** It assumes no background in math, political science, or election administration. Every step of both counting methods is explained in plain language with worked examples you can follow and verify yourself. A glossary of technical terms is included at the end.

Both methods use the same ballot. You score candidates from 0 to 5 stars. What changes between single-winner and multi-winner elections is how those scores are added up to determine who wins. This document shows you exactly how that works, with nothing hidden.

---

## Part I: STAR Voting

STAR stands for **Score Then Automatic Runoff**. It is used whenever an election is choosing one winner -- for President, for Senate, or for House districts that elect fewer than three Representatives.

### How You Vote

You receive a ballot listing all the candidates. Next to each name is a rating scale from 0 to 5 stars.

- **5 stars** means you strongly support this candidate.
- **0 stars** means you do not support this candidate at all.
- **1 through 4 stars** lets you show different levels of support in between.

You can score as many or as few candidates as you want. You can give the same score to more than one candidate. If you leave a candidate blank, they receive 0 stars from your ballot.

There are no rankings, no party lists, and no requirement to rate every candidate. Your only task is: score each candidate based on how much you support them.

### How Votes Are Counted

STAR voting counts your ballot in two steps. Each step answers a different question.

**Step 1: The Scoring Round**

Every score from every voter is added up. Each candidate gets a total score -- the sum of all the ratings they received from all voters. The two candidates with the highest total scores move on to the next step. They become the **finalists**.

This step answers the question: *Which two candidates have the most overall support?*

**Step 2: The Automatic Runoff**

Now every ballot is looked at one more time. For each voter, the system checks: which of the two finalists did you give a higher score? Your full vote goes to that finalist. The finalist who is preferred by more voters wins the election.

This step answers the question: *Between the top two, which one do more voters actually prefer?*

### Why Two Steps?

Each step catches something the other one would miss.

The scoring round makes sure that the finalists are candidates with broad support. A candidate who is loved by a small group but unknown or disliked by everyone else will not score high enough overall to become a finalist.

The automatic runoff makes sure the winner is preferred by a majority. It is possible for one candidate to have a higher total score but still lose the head-to-head comparison. The runoff catches this and ensures the winner is the one more voters prefer when it comes down to two.

Together, the two steps identify the candidate who has both wide support and majority preference.

### Worked Example: A Senate Election

Imagine a Senate election with five candidates and 100 voters.

**The Candidates:**

- Rivera
- Okafor
- Walsh
- Tanaka
- Fischer

**Step 1: The Scoring Round**

After all 100 voters have turned in their ballots, election officials count how many voters gave each candidate each score. The results are shown in the table below.

**Table 1: How Voters Scored Each Candidate**

| Candidate | 0 Stars | 1 Star | 2 Stars | 3 Stars | 4 Stars | 5 Stars | Total Voters |
|-----------|:-------:|:------:|:-------:|:-------:|:-------:|:-------:|:------------:|
| Rivera    | 20      | 20     | 0       | 25      | 0       | 35      | 100          |
| Okafor    | 30      | 20     | 10      | 5       | 20      | 15      | 100          |
| Walsh     | 0       | 35     | 20      | 20      | 0       | 25      | 100          |
| Tanaka    | 40      | 10     | 10      | 5       | 15      | 20      | 100          |
| Fischer   | 40      | 20     | 5       | 10      | 5       | 20      | 100          |

**How to read this table:** Each row is one candidate. Each column shows how many voters gave that candidate that score. Take Rivera's row: 20 voters gave Rivera 0 stars, 20 voters gave Rivera 1 star, 0 voters gave Rivera 2 stars, 25 voters gave Rivera 3 stars, 0 voters gave Rivera 4 stars, and 35 voters gave Rivera 5 stars. Since every voter scored every candidate, each row adds up to 100.

Now we calculate each candidate's total score. This is pure addition -- we are adding up every score every voter gave. The table below uses multiplication as a shorthand to make this manageable. Instead of writing out "1 + 1 + 1 + 1..." twenty times, we write "20 times 1 equals 20." The result is the same.

**Table 2: Score Calculation**

| Candidate | x0 | x1 | x2 | x3 | x4 | x5 | Total Score |
|-----------|:--:|:--:|:--:|:--:|:--:|:--:|:-----------:|
| Rivera    | 0  | 20 | 0  | 75 | 0  | 175 | **270**    |
| Okafor    | 0  | 20 | 20 | 15 | 80 | 75  | **210**    |
| Walsh     | 0  | 35 | 40 | 60 | 0  | 125 | **260**    |
| Tanaka    | 0  | 10 | 20 | 15 | 60 | 100 | **205**    |
| Fischer   | 0  | 20 | 10 | 30 | 20 | 100 | **180**    |

**How to read this table:** This table takes the voter counts from Table 1 and turns them into scores. Take Rivera's row again:

- Rivera received 20 scores of 0. That is 20 times 0, which equals a subtotal of **0**.
- Rivera received 20 scores of 1. That is 20 times 1, which equals a subtotal of **20**.
- Rivera received 0 scores of 2. Subtotal: **0**.
- Rivera received 25 scores of 3. That is 25 times 3, which equals a subtotal of **75**.
- Rivera received 0 scores of 4. Subtotal: **0**.
- Rivera received 35 scores of 5. That is 35 times 5, which equals a subtotal of **175**.

Adding up all of Rivera's subtotals: 0 + 20 + 0 + 75 + 0 + 175 = **270**. That is Rivera's total score.

The same calculation applies to every candidate. The two candidates with the highest total scores -- **Rivera (270)** and **Walsh (260)** -- become the finalists and advance to the automatic runoff.

**Step 2: The Automatic Runoff**

Now every ballot is looked at one more time. For each voter, the system asks a simple question: which finalist did you score higher, Rivera or Walsh? Your full vote goes to that finalist.

| Preference | Voters |
|------------|:------:|
| Scored Rivera higher than Walsh | 35 |
| Scored Walsh higher than Rivera | 65 |

**Walsh wins, 65 to 35.**

**What does this tell us?**

Look back at Table 1. Rivera had the most 5-star ratings of any candidate (35 voters gave Rivera the top score). But Rivera also had 20 voters at 0 stars -- one in five voters gave Rivera the lowest possible rating. Rivera had passionate supporters but also real opposition.

Walsh, on the other hand, had zero voters at 0 stars. Nobody strongly opposed Walsh. Walsh's support was spread across the upper score levels -- 25 voters at 5 stars, 20 at 3 stars, 20 at 2 stars, and 35 at 1 star. That broad, cross-cutting support produced the second-highest total score in the scoring round and a decisive majority in the runoff.

The scoring round identified the two candidates with the most overall support. The runoff then determined which of those two the majority of voters actually preferred. Rivera's passionate base was not enough to overcome Walsh's wider appeal.

Under the old system where you pick just one candidate, five candidates would split the vote badly -- someone could win with as little as 21% support while 79% of voters preferred someone else. STAR voting lets you honestly score all five candidates, and the two-step process makes sure the winner has both broad support and majority preference.

---

## Part II: Allocated Score

Allocated Score is used when a district is electing more than one Representative at the same time. Under the Act, most House districts elect between 3 and 7 Representatives. Allocated Score is how those multiple seats get filled fairly.

You may also see this method called **STAR-PR** (STAR Proportional Representation). Both names refer to the same thing.

### Why Elect More Than One Representative?

When a district elects only one person, the winner takes the whole seat and everyone who voted for someone else gets nothing. If a district is 60% one party and 40% the other, the 40% will likely never win that seat. Their votes are effectively wasted, election after election.

Multi-member districts fix this. A district that elects 5 Representatives can give roughly 3 seats to the 60% and 2 seats to the 40%. Voters across the political spectrum get representation in proportion to their numbers. That is what "proportional representation" means: your share of the seats reflects your share of the voters.

Allocated Score is the method that makes this proportional allocation happen.

### How You Vote

Exactly the same as STAR voting. You score each candidate from 0 to 5 stars. The ballot looks the same. Your task is the same. The only difference is that the district is electing multiple winners instead of one.

### The Big Idea: Ballot Weight

To understand Allocated Score, you need one new concept: **ballot weight**.

Think of your ballot as having a battery. When the election starts, your battery is fully charged -- your ballot has a weight of 1, meaning it counts at full strength.

When a candidate you supported wins a seat, some of your battery gets used up. Your ballot weight goes down, because you have already gotten some of what you wanted -- one of your preferred candidates is now elected. This means your ballot has less influence on the remaining seats.

Meanwhile, voters whose preferred candidates have not won yet still have full batteries. Their ballots now carry more weight in deciding who fills the next seat.

This is what makes the outcome fair and proportional. Once a group of voters has elected their preferred candidate, they step back and make room for other voters' preferences to be heard. No single group can sweep all the seats, because their ballot weight gets spent as their candidates win.

### How Votes Are Counted

Allocated Score fills one seat at a time through a series of rounds. Here is what happens in each round:

**1. Add up the scores.** For each candidate who has not already won a seat, add up all the scores they received -- but now each score is multiplied by that ballot's current weight. In the first round, all ballot weights are 1, so this is just simple addition like in STAR voting. In later rounds, some ballots will weigh less because those voters already helped elect someone.

**2. The highest-scoring candidate wins the next seat.**

**3. Reduce ballot weights.** Every ballot that gave the winning candidate a score above 0 has its weight reduced. The more you supported the winner, the more your weight goes down. Ballots that gave the winner 0 stars are not affected at all.

**4. Repeat** until all seats are filled.

### How Much Weight Gets Spent?

Before the first round, a number called the **quota** is calculated. The quota is the total number of voters divided by the number of seats. In an election with 30 voters filling 3 seats, the quota is 30 divided by 3, which equals 10.

The quota represents the "cost" of one seat. In each round, a total of exactly 10 units of ballot weight (in our example) gets spent across all the ballots that supported the winning candidate. How much each individual ballot pays depends on how strongly that ballot supported the winner compared to everyone else who supported the winner.

If you gave the winner 5 stars and most other supporters gave 3 stars, you pay a bigger share of the cost. If you only gave the winner 1 star, you pay a smaller share. This is fair: voters who got more of what they wanted give up more of their remaining influence.

### Worked Example: A Three-Seat House District

Let's walk through a full example. This district has 30 voters electing 3 Representatives from a field of 6 candidates.

**The quota is 30 voters / 3 seats = 10.**

**The Candidates:**

- Lin
- Garcia
- Kim
- Murphy
- Patel
- Brooks

**The Voters:**

The 30 voters fall into three groups based on their scoring patterns. In real elections, voter preferences are far more varied and complex -- we use groups here only to keep the example small enough to follow by hand. The math works the same regardless of whether voters fall into neat groups or each voter scores differently.

| Voter Group | Number of Voters | Lin | Garcia | Kim | Murphy | Patel | Brooks |
|-------------|:----------------:|:---:|:------:|:---:|:------:|:-----:|:------:|
| Group 1     | 15               | 5   | 4      | 2   | 0      | 0     | 1      |
| Group 2     | 10               | 0   | 0      | 1   | 5      | 4     | 0      |
| Group 3     | 5                | 1   | 2      | 5   | 1      | 0     | 3      |

**How to read this table:** Each row is a group of voters who scored the candidates the same way. The 15 voters in Group 1 each gave Lin 5 stars, Garcia 4 stars, Kim 2 stars, Murphy 0 stars, Patel 0 stars, and Brooks 1 star. The 10 voters in Group 2 each gave Lin 0 stars, Garcia 0 stars, Kim 1 star, Murphy 5 stars, Patel 4 stars, and Brooks 0 stars. And so on for Group 3.

Now let's fill the three seats.

#### Round 1: Filling the First Seat

All 30 ballots start with a weight of 1 (full strength). We add up each candidate's scores across all ballots.

**Table 3: Round 1 Score Calculation**

| Candidate | From Group 1 (15 voters) | From Group 2 (10 voters) | From Group 3 (5 voters) | Total Score |
|-----------|:------------------------:|:------------------------:|:-----------------------:|:-----------:|
| Lin       | 15 x 5 = 75             | 10 x 0 = 0              | 5 x 1 = 5              | **80**      |
| Garcia    | 15 x 4 = 60             | 10 x 0 = 0              | 5 x 2 = 10             | **70**      |
| Kim       | 15 x 2 = 30             | 10 x 1 = 10             | 5 x 5 = 25             | **65**      |
| Murphy    | 15 x 0 = 0              | 10 x 5 = 50             | 5 x 1 = 5              | **55**      |
| Patel     | 15 x 0 = 0              | 10 x 4 = 40             | 5 x 0 = 0              | **40**      |
| Brooks    | 15 x 1 = 15             | 10 x 0 = 0              | 5 x 3 = 15             | **30**      |

**How to read this table:** Take Lin's row. The 15 voters in Group 1 each gave Lin 5 stars, so their contribution is 15 times 5, which equals 75. The 10 voters in Group 2 each gave Lin 0 stars, so their contribution is 0. The 5 voters in Group 3 each gave Lin 1 star, so their contribution is 5 times 1, which equals 5. Add those up: 75 + 0 + 5 = 80. That is Lin's total score.

**Lin wins the first seat** with a total score of 80.

**Now we reduce ballot weights.** Lin's total score was 80, and the quota is 10. Every ballot that gave Lin a score above 0 will have its weight reduced. The reduction depends on how much each ballot contributed to Lin's total compared to the full total of 80.

Here is how the weight reduction works for each group:

**Group 1 voters** (15 voters, each gave Lin 5 stars):

- Each ballot's contribution to Lin: weight (1.0) times score (5) = 5.0
- Share of Lin's total: 5.0 out of 80 = 0.0625 per ballot
- Weight spent per ballot: quota (10) times 0.0625 = 0.625
- New ballot weight: 1.0 minus 0.625 = **0.375**

These voters gave Lin their strongest support, so they pay the most. Their ballots now count at about a third of full strength.

**Group 2 voters** (10 voters, each gave Lin 0 stars):

- These voters gave Lin nothing, so they contributed nothing to Lin's election.
- Weight spent: 0
- New ballot weight: **1.000** (unchanged)

These voters did not help elect Lin, so their ballots stay at full strength. This is the key to proportionality -- they still have their full voice for the next seat.

**Group 3 voters** (5 voters, each gave Lin 1 star):

- Each ballot's contribution to Lin: weight (1.0) times score (1) = 1.0
- Share of Lin's total: 1.0 out of 80 = 0.0125 per ballot
- Weight spent per ballot: quota (10) times 0.0125 = 0.125
- New ballot weight: 1.0 minus 0.125 = **0.875**

These voters gave Lin only mild support, so they pay only a small amount. Their ballots are still nearly full strength.

**Summary after Round 1:**

| Voter Group | Voters | New Ballot Weight | Why |
|-------------|:------:|:-----------------:|-----|
| Group 1     | 15     | 0.375             | Gave Lin 5 stars -- paid the most |
| Group 2     | 10     | 1.000             | Gave Lin 0 stars -- unaffected |
| Group 3     | 5      | 0.875             | Gave Lin 1 star -- paid a little |

#### Round 2: Filling the Second Seat

Now we recalculate scores, but this time each ballot's score is multiplied by its current weight. Lin is removed from the candidate list since Lin already has a seat.

**Table 4: Round 2 Weighted Score Calculation**

| Candidate | Group 1 (15 voters x 0.375) | Group 2 (10 voters x 1.0) | Group 3 (5 voters x 0.875) | Weighted Total |
|-----------|:---------------------------:|:--------------------------:|:---------------------------:|:--------------:|
| Garcia    | 15 x 0.375 x 4 = 22.5     | 10 x 1.0 x 0 = 0          | 5 x 0.875 x 2 = 8.8       | **31.3**       |
| Kim       | 15 x 0.375 x 2 = 11.3     | 10 x 1.0 x 1 = 10.0       | 5 x 0.875 x 5 = 21.9      | **43.1**       |
| Murphy    | 15 x 0.375 x 0 = 0        | 10 x 1.0 x 5 = 50.0       | 5 x 0.875 x 1 = 4.4       | **54.4**       |
| Patel     | 15 x 0.375 x 0 = 0        | 10 x 1.0 x 4 = 40.0       | 5 x 0.875 x 0 = 0         | **40.0**       |
| Brooks    | 15 x 0.375 x 1 = 5.6      | 10 x 1.0 x 0 = 0          | 5 x 0.875 x 3 = 13.1      | **18.8**       |

**How to read this table:** The calculation now has three parts multiplied together: the number of voters, their current ballot weight, and their score for the candidate. Take Murphy's row. Group 1 (15 voters, weight 0.375) gave Murphy 0 stars: 15 times 0.375 times 0 equals 0. Group 2 (10 voters, weight 1.0) gave Murphy 5 stars: 10 times 1.0 times 5 equals 50. Group 3 (5 voters, weight 0.875) gave Murphy 1 star: 5 times 0.875 times 1 equals 4.4. Add those up: 0 + 50 + 4.4 = 54.4.

**Murphy wins the second seat** with a weighted total of 54.4.

Notice what happened: Group 2's voters still had full ballot weight (1.0) because they gave Lin 0 stars in Round 1. That full-strength weight, combined with their strong support for Murphy (5 stars), made Murphy the clear winner this round. The system worked as designed -- voters who had not yet been represented got to drive this decision.

**Reducing ballot weights again:** Murphy's weighted total was 54.4, and the quota is still 10.

| Voter Group | Murphy Score | Previous Weight | Weight Spent | New Weight |
|-------------|:-----------:|:---------------:|:------------:|:----------:|
| Group 1     | 0           | 0.375           | 0            | **0.375**  |
| Group 2     | 5           | 1.000           | 0.919        | **0.081**  |
| Group 3     | 1           | 0.875           | 0.161        | **0.714**  |

Group 2 voters gave Murphy 5 stars and have now spent almost all their ballot weight (down to 0.081). They have elected their candidate and have very little influence remaining -- which is fair, because they have already been represented.

#### Round 3: Filling the Third Seat

Recalculate scores one more time with the latest ballot weights. Both Lin and Murphy are removed.

**Table 5: Round 3 Weighted Score Calculation**

| Candidate | Group 1 (15 x 0.375) | Group 2 (10 x 0.081) | Group 3 (5 x 0.714) | Weighted Total |
|-----------|:---------------------:|:---------------------:|:--------------------:|:--------------:|
| Garcia    | 15 x 0.375 x 4 = 22.5 | 10 x 0.081 x 0 = 0  | 5 x 0.714 x 2 = 7.1 | **29.6**      |
| Kim       | 15 x 0.375 x 2 = 11.3 | 10 x 0.081 x 1 = 0.8 | 5 x 0.714 x 5 = 17.9 | **29.9**     |
| Patel     | 15 x 0.375 x 0 = 0    | 10 x 0.081 x 4 = 3.2 | 5 x 0.714 x 0 = 0   | **3.2**       |
| Brooks    | 15 x 0.375 x 1 = 5.6  | 10 x 0.081 x 0 = 0   | 5 x 0.714 x 3 = 10.7 | **16.3**     |

**Kim wins the third and final seat** with a weighted total of 29.9.

This was close -- Garcia finished at 29.6, just behind Kim. What made the difference? Kim had support from all three voter groups. Group 1 contributed 11.3, Group 2 contributed 0.8, and Group 3 contributed 17.9. Garcia had more from Group 1 (22.5) and Group 3 (7.1) but nothing from Group 2. Kim's broader appeal, drawing from every part of the electorate, was enough to edge out Garcia's stronger but narrower support.

#### What the Final Result Tells Us

| Seat | Winner | Elected By |
|------|--------|------------|
| 1    | Lin    | Primarily Group 1 voters (who gave Lin 5 stars) |
| 2    | Murphy | Primarily Group 2 voters (who gave Murphy 5 stars) |
| 3    | Kim    | A mix of all three groups |

Now compare each group's share of voters to their share of representation:

| Voter Group | Voters | Share of Electorate | Seats Won | Share of Seats |
|-------------|:------:|:-------------------:|:---------:|:--------------:|
| Group 1     | 15     | 50%                 | 1 (Lin)   | 33%            |
| Group 2     | 10     | 33%                 | 1 (Murphy) | 33%           |
| Group 3     | 5      | 17%                 | 1 (Kim)   | 33%            |

With only three seats to fill, perfect proportionality is not possible -- you cannot divide three seats into exact 50/33/17 portions. Group 1 is somewhat underrepresented and Group 3 somewhat overrepresented. This is a mathematical limitation of small numbers, not a flaw in the method. As district size increases (the Act allows up to 7 seats per district), proportional accuracy improves.

The important point is that every group of voters received representation. In a traditional single-winner election, only one group would win and the other two would get nothing. Here, all three groups elected someone who reflects their preferences.

And nobody had to vote strategically. Every voter simply scored each candidate honestly. The ballot weight mechanism handled the rest.

---

## Part III: How STAR and Allocated Score Fit Together

### Same Ballot, Different Counting

The Act's voting methods are designed so that you do the same thing on every federal race: score each candidate from 0 to 5 stars. Whether you are voting for President, Senator, or Representative, the ballot looks the same and your task is the same.

What changes is behind the scenes. For single-winner races, your scores are counted using STAR voting's two-step process (scoring round, then automatic runoff). For multi-winner House races, your scores are counted using Allocated Score's round-by-round allocation with ballot weight.

This consistency is intentional. There is only one skill to learn. If you know how to rate things on a 5-star scale -- and most people already do, from restaurant and product reviews -- you know how to vote under the Act.

### What Stays the Same, What Changes

| Feature | STAR (One Winner) | Allocated Score (Multiple Winners) |
|---------|-------------------|------------------------------------|
| What you do | Score candidates 0-5 stars | Score candidates 0-5 stars |
| Number of winners | 1 | 3 to 7 |
| How winners are determined | Highest scores, then head-to-head runoff | Highest weighted scores, round by round |
| Ballot weight | Not applicable | Reduced as your preferred candidates win |
| Proportionality | Not applicable (one winner) | Seat shares reflect voter shares |

### Who Manages the System?

The Act creates the **Electoral Science Office (ESO)**, a permanent technical agency responsible for maintaining and improving the voting methods over time. The ESO operates within a three-tier protection framework that matches each element's level of protection to its significance.

Some things are **statutory principles** -- the democratic commitments that define how the voting system must work: the 0-5 star scoring scale, the requirement that all voters are treated equally, and the proportional outcome requirement for multi-winner elections. These can only be changed by an Act of Congress.

Other things are **protected design elements** -- core design choices like the specific scoring range and the structure of the automatic runoff. The ESO can study these and propose improvements, but changes require Congress to affirmatively approve them.

Finally, there are **adjustable technical parameters** -- implementation details like the exact formula used to calculate the quota, or the precise rules for breaking ties. The ESO can adjust these through a structured public process that includes supermajority Commission approval, public comment, and Congressional review. This allows the system to benefit from new research without requiring a new law every time a small improvement is identified.

The key point for voters: the parts of the system you interact with directly -- the ballot, the scoring scale, and the fundamental rules of how winners are determined -- receive the highest levels of protection. Technical details that operate behind the scenes can be refined by experts, but only through transparent processes with Congressional oversight.

---

## Part IV: Common Questions

**Why not ranked-choice voting?**

Ranked-choice voting asks you to rank candidates in order: 1st, 2nd, 3rd, and so on. STAR voting asks you to score candidates on a scale. The key differences: STAR lets you give equal scores to candidates you support equally, which ranking does not. STAR's counting process is simpler and more transparent -- there are no complicated multi-round elimination sequences where candidates are knocked out one at a time. And STAR guarantees that giving a candidate a higher score always helps that candidate, which some ranked-choice systems do not.

**Why not party lists?**

Some countries use a system where you vote for a political party, and the party decides which specific people fill the seats they win. The Act does not use this approach. Under Allocated Score, you score individual candidates by name. Representatives win seats because voters rated them highly -- not because a party put them on a list. You always know exactly who you are voting for.

**What if there is a tie?**

In STAR voting, if two candidates tie for the second finalist spot, the tie is broken by comparing those two candidates head-to-head (which one did more voters prefer). If the tie persists in the runoff, state law determines how to break it -- typically by a public random drawing.

In Allocated Score, ties in weighted score totals are resolved through procedures set by state law, following guidance from the Electoral Science Office. All tie-breaking methods must be neutral and publicly verifiable.

**Can I vote if I only know a few candidates?**

Yes. Score the candidates you know. Any candidate you leave blank receives 0 stars from your ballot. You do not need to research every candidate to participate.

**Does scoring other candidates hurt my favorite?**

No. Every candidate's score is added up independently. Giving your second-favorite candidate 4 stars does not take anything away from the 5 stars you gave your favorite. In the STAR runoff, only your preference between the two finalists matters. In Allocated Score, the ballot weight system ensures that your influence is spent proportionally, not taken away arbitrarily.

**Will this be confusing?**

Most voters find scoring easier than ranking. You already rate restaurants, movies, products, and apps on star scales. This works the same way. The counting process is more complex than "most votes wins," but the counting is done by election officials and computers -- your only job is to score the candidates honestly.

---

## Appendix A: Mathematical Specification

This appendix provides formal definitions for readers who want the precise mathematics. These specifications represent the reference implementation; specific parameters are subject to ESO modification within the graduated protection framework established by the Act.

### A.1 STAR Voting (Single-Winner)

**Inputs:** A set of ballots B, where each ballot b assigns a score s(b, c) in {0, 1, 2, 3, 4, 5} to each candidate c.

**Scoring Round:**

For each candidate c, compute the total score:

> S(c) = sum of s(b, c) for all ballots b in B

The two candidates with the highest total scores, c1 and c2, advance as finalists. If more than two candidates tie for the highest total score, tie-breaking procedures apply.

**Automatic Runoff:**

For each ballot b, compare s(b, c1) and s(b, c2):

- If s(b, c1) > s(b, c2), ballot b votes for c1.
- If s(b, c2) > s(b, c1), ballot b votes for c2.
- If s(b, c1) = s(b, c2), ballot b is exhausted (no runoff preference expressed).

The finalist with more runoff votes wins. If tied, tie-breaking procedures apply.

### A.2 Allocated Score (Multi-Winner)

**Inputs:** A set of ballots B, each with initial weight w(b) = 1. A set of candidates C. A number of seats to fill, k.

**Quota Calculation:**

> Q = |B| / k

where |B| is the number of valid ballots. (The specific quota formula -- Hare, Droop, or other -- is an adjustable technical parameter maintained by the ESO within the graduated protection framework.)

**Allocation Round (repeated k times):**

**Step 1.** For each remaining candidate c, compute the weighted score:

> WS(c) = sum of w(b) x s(b, c) for all ballots b in B

**Step 2.** Elect the candidate c* with the highest WS(c*).

**Step 3.** For each ballot b where s(b, c*) > 0, reduce the ballot weight:

> spend(b) = Q x [w(b) x s(b, c*)] / WS(c*)

> w(b) = w(b) - spend(b)

Ballots that gave the elected candidate a score of 0 are unaffected.

**Step 4.** Remove c* from the set of remaining candidates. Repeat from Step 1.

**Properties:**

The total weight spent in each round equals Q (the quota), ensuring that each elected candidate "costs" an equal share of the electorate's total voting power. Ballot weight reductions are proportional to each ballot's contribution to the elected candidate's total, ensuring that voters who gave stronger support to an elected candidate have more weight spent than those who gave weaker support.

### A.3 Notation Summary

| Symbol | Meaning |
|--------|---------|
| B | Set of all valid ballots |
| b | A single ballot |
| C | Set of all candidates |
| c | A single candidate |
| k | Number of seats to fill |
| s(b, c) | Score assigned by ballot b to candidate c (0-5) |
| w(b) | Current weight of ballot b (starts at 1) |
| Q | Quota (ballots per seat) |
| S(c) | Total score for candidate c (unweighted) |
| WS(c) | Weighted score for candidate c |

---

## Glossary

**Allocated Score.** The method used to count votes in multi-winner elections under the Act. Voters score candidates 0-5 stars, and seats are filled one at a time with ballot weights adjusted after each round. Also called STAR-PR.

**Automatic runoff.** The second step of STAR voting. After the two highest-scoring candidates are identified, every ballot is checked to see which of the two the voter preferred. The one preferred by more voters wins. No separate runoff election is held -- it happens automatically using the scores already on your ballot.

**Ballot weight.** A number that represents how much influence your ballot still has. It starts at 1 (full influence). As candidates you supported win seats, your ballot weight decreases, reflecting that you have already received some representation.

**Deterministic.** Means the same ballots always produce the same result. There is no randomness in the counting process (except for tie-breaking in rare cases). Anyone can recount the ballots and get the identical outcome.

**District magnitude.** The number of seats elected from a single district. A single-member district has a magnitude of 1. Under the Act, multi-member House districts have a magnitude between 3 and 7.

**Electoral Science Office (ESO).** A permanent federal agency created by the Act to maintain, evaluate, and refine the technical details of the voting methods. The ESO operates within a three-tier graduated protection framework: statutory principles require an Act of Congress to change, protected design elements require affirmative Congressional approval, and adjustable technical parameters can be refined by the ESO through a structured public process with Congressional oversight.

**Finalist.** In STAR voting, one of the two candidates who received the highest total scores and advance to the automatic runoff.

**Monotonicity.** A property meaning that giving a candidate a higher score can never hurt that candidate. If you increase your score for a candidate, it can only help them or make no difference -- it can never backfire and cause them to lose.

**Multi-member district.** A district that elects more than one Representative. Under the Act, most House districts elect between 3 and 7 Representatives.

**Proportional representation.** A system where the share of seats won by different groups of voters roughly matches those groups' share of the electorate. If 40% of voters prefer one set of candidates, they win roughly 40% of the seats.

**Quota.** The amount of ballot weight needed to fill one seat. Calculated by dividing the total number of voters by the number of seats. In an election with 100 voters and 5 seats, the quota is 20.

**Scoring round.** The first step of STAR voting. Every score from every voter is added up. The two candidates with the highest total scores become the finalists.

**Single-member district.** A district that elects one Representative.

**STAR voting.** Score Then Automatic Runoff. The method used for single-winner elections under the Act. Voters score candidates 0-5, the two highest-scoring candidates become finalists, and the finalist preferred by more voters wins.

**STAR-PR.** Another name for Allocated Score. The "PR" stands for Proportional Representation.

**Weighted score.** A candidate's score after ballot weights are applied. Calculated by multiplying each ballot's score for that candidate by that ballot's current weight, then adding up the results.

---

## Revision History

**Revision 2.0** (Current)

- Updated from CMA Rev 4.2 to FEMA Rev 5.0
- Rebranded all references from "Congressional Modernization Act (CMA)" to "Federal Elections Modernization Act (FEMA)"
- Applied APAI self-reference conventions: full name established once in Purpose section, "the Act" used for all subsequent references
- Updated "Who Manages the System?" section to reflect three-tier graduated protection framework (statutory principles, protected design elements, adjustable technical parameters), replacing prior binary framing
- Updated ESO glossary entry to reflect three-tier framework
- Updated Appendix A quota description to reference graduated protection framework
- No changes to voting method descriptions, worked examples, or mathematical specifications

**Revision 1.0**

- Initial publication
- Unified explainer covering STAR voting and Allocated Score
- Written for a general voter audience
- Includes worked examples for both single-winner and multi-winner elections
- Glossary of technical terms
- Mathematical specification appendix

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
