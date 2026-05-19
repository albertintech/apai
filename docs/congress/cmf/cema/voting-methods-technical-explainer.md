# Congressional Elections Modernization Act

## STAR Voting and Allocated Score: A Technical Explainer

---

## Purpose

This document explains how votes are counted under the Congressional Elections Modernization Act (CEMA), hereafter referred to as "the Act." It covers both voting methods used in congressional elections:

1. **STAR Voting** -- used when one person is being elected (Senate and some House races).
2. **Allocated Score** -- used when multiple people are being elected from the same district (most House races).

**This document is written for voters.** It assumes no background in math, political science, or election administration. Every step of both counting methods is explained in plain language with worked examples you can follow and verify yourself. A glossary of technical terms is included at the end.

Both methods use the same ballot. You score candidates from 0 to 5 stars. What changes between single-winner and multi-winner elections is how those scores are added up to determine who wins. This document shows you exactly how that works, with nothing hidden.

---

## Part I: STAR Voting

STAR stands for **Score Then Automatic Runoff**. It is used whenever an election is choosing one winner -- for Senate, or for House districts that elect fewer than three Representatives.

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

You may also see this method referred to under the umbrella term **STAR-PR** (STAR Proportional Representation). STAR-PR is the general concept -- a 0-5 star ballot counted with a proportional algorithm. Allocated Score is the specific counting algorithm recommended for STAR-PR by the Equal Vote Coalition's research committee after a two-year comparative evaluation. The Act uses Allocated Score as its proportional method.

### Why Elect More Than One Representative?

When a district elects only one person, the winner takes the whole seat and everyone who voted for someone else gets nothing. If a district is 60% one party and 40% the other, the 40% will likely never win that seat. Their votes are effectively wasted, election after election.

Multi-member districts fix this. A district that elects 5 Representatives can give roughly 3 seats to the 60% and 2 seats to the 40%. Voters across the political spectrum get representation in proportion to their numbers. That is what "proportional representation" means: your share of the seats reflects your share of the voters.

Allocated Score is the method that makes this proportional allocation happen.

### How You Vote

Exactly the same as STAR voting. You score each candidate from 0 to 5 stars. The ballot looks the same. Your task is the same. The only difference is that the district is electing multiple winners instead of one.

### The Big Idea: Ballot Weight

To understand Allocated Score, you need one new concept: **ballot weight**.

Think of your ballot as having a battery. When the election starts, your battery is fully charged -- your ballot has a weight of 1, meaning it counts at full strength.

When a candidate wins a seat, the system identifies that candidate's strongest supporters and removes them from the count. Their ballot weight goes to zero -- they have been fully represented by the winning candidate and step aside so that other voters can drive the next seat. If the quota boundary falls in the middle of a group of voters who all gave the winner the same score, those voters split the remaining cost equally, each losing a fraction of their weight rather than being fully removed.

Voters who gave the winner a lower score -- below the boundary where the quota was filled -- keep their full ballot weight. They were not needed to fill the winner's quota, so they retain their full voice for the remaining seats.

This is what makes the outcome fair and proportional. Each winner is "paid for" by a specific quota of voters drawn from that winner's strongest supporters. Once those supporters have been allocated, everyone else continues at full strength. No single group can sweep all the seats, because each seat consumes a quota of that group's voters.

### How Votes Are Counted

Allocated Score fills one seat at a time through a series of rounds. Here is what happens in each round:

**1. Add up the scores.** For each candidate who has not already won a seat, add up all the scores they received -- but now each score is multiplied by that ballot's current weight. In the first round, all ballot weights are 1, so this is just simple addition like in STAR voting. In later rounds, some ballots will weigh less because those voters already helped elect someone.

**2. The highest-scoring candidate wins the next seat.**

**3. Allocate ballot weight from the winner's strongest supporters.** After the winner is determined, voters are sorted by the score they gave the winner, from highest to lowest. Starting from the top of this sorted list, ballot weights are set to zero -- one voter at a time -- until one quota's worth of ballot weight has been consumed. The winner's strongest supporters are fully allocated first. If the quota boundary falls in the middle of a group of voters who all gave the same score, those voters share the remaining cost equally (each loses the same fraction of their weight). Voters below this boundary are not affected at all -- their ballot weight stays exactly where it was.

**4. Repeat** until all seats are filled.

### How Much Weight Gets Spent?

Before the first round, a number called the **quota** is calculated. The quota is the total number of voters divided by the number of seats. In an election with 30 voters filling 3 seats, the quota is 30 divided by 3, which equals 10.

The quota represents the "cost" of one seat. Each time a candidate wins, exactly one quota's worth of ballot weight is consumed from that candidate's supporters. The allocation starts at the top -- voters who gave the winner the highest scores are consumed first. If 10 units of weight are needed and the winner's 5-star supporters account for 15 units, only a fraction of each supporter's weight is taken (enough to total exactly 10), and everyone who gave a lower score is left completely untouched.

Think of it like paying for pizza with a group. The people who wanted the pizza the most pay first. If they have more than enough money between them, they each chip in an equal fraction and nobody else has to pay at all. The people who barely wanted the pizza keep their full wallet for next time.

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

**Now we allocate ballot weight.** The quota is 10, so we need to consume 10 units of ballot weight from Lin's supporters, starting with the strongest supporters first.

First, sort all voters by the score they gave Lin, from highest to lowest:

| Score Given to Lin | Voter Group | Number of Voters | Weight per Voter | Total Weight in Tier |
|:-------------------:|:-----------:|:----------------:|:----------------:|:--------------------:|
| 5 stars             | Group 1     | 15               | 1.0              | 15.0                 |
| 1 star              | Group 3     | 5                | 1.0              | 5.0                  |
| 0 stars             | Group 2     | 10               | 1.0              | 10.0                 |

Now allocate from the top. The 5-star tier has 15 units of ballot weight. The quota is 10. Since 15 exceeds 10, the quota is filled entirely within this tier -- we do not need to touch anyone below it.

**Fractional surplus handling:** We need 10 units out of the 15 available. Each of the 15 voters in this tier loses the same fraction: 10 divided by 15 equals two-thirds. Each Group 1 voter's weight drops from 1.0 to one-third (approximately 0.333).

The 1-star tier (Group 3) and the 0-star tier (Group 2) are below the allocation boundary. They are not touched at all. Their ballot weight stays at 1.0.

**Summary after Round 1:**

| Voter Group | Voters | New Ballot Weight | Why |
|-------------|:------:|:-----------------:|-----|
| Group 1     | 15     | 0.333             | Gave Lin 5 stars -- allocated as Lin's quota (fractional) |
| Group 2     | 10     | 1.000             | Gave Lin 0 stars -- below the allocation boundary |
| Group 3     | 5      | 1.000             | Gave Lin 1 star -- below the allocation boundary |

Notice that Group 3 gave Lin 1 star but kept their full ballot weight. Under Allocated Score, the quota was completely filled by the 5-star supporters before reaching anyone else. Group 3's mild support for Lin cost them nothing.

#### Round 2: Filling the Second Seat

Now we recalculate scores, but this time each ballot's score is multiplied by its current weight. Lin is removed from the candidate list since Lin already has a seat.

**Table 4: Round 2 Weighted Score Calculation**

| Candidate | Group 1 (15 voters x 0.333) | Group 2 (10 voters x 1.0) | Group 3 (5 voters x 1.0) | Weighted Total |
|-----------|:---------------------------:|:--------------------------:|:--------------------------:|:--------------:|
| Garcia    | 15 x 0.333 x 4 = 20.0     | 10 x 1.0 x 0 = 0          | 5 x 1.0 x 2 = 10.0        | **30.0**       |
| Kim       | 15 x 0.333 x 2 = 10.0     | 10 x 1.0 x 1 = 10.0       | 5 x 1.0 x 5 = 25.0        | **45.0**       |
| Murphy    | 15 x 0.333 x 0 = 0        | 10 x 1.0 x 5 = 50.0       | 5 x 1.0 x 1 = 5.0         | **55.0**       |
| Patel     | 15 x 0.333 x 0 = 0        | 10 x 1.0 x 4 = 40.0       | 5 x 1.0 x 0 = 0           | **40.0**       |
| Brooks    | 15 x 0.333 x 1 = 5.0      | 10 x 1.0 x 0 = 0          | 5 x 1.0 x 3 = 15.0        | **20.0**       |

**How to read this table:** The calculation now has three parts multiplied together: the number of voters, their current ballot weight, and their score for the candidate. Take Murphy's row. Group 1 (15 voters, weight 0.333) gave Murphy 0 stars: 15 times 0.333 times 0 equals 0. Group 2 (10 voters, weight 1.0) gave Murphy 5 stars: 10 times 1.0 times 5 equals 50. Group 3 (5 voters, weight 1.0) gave Murphy 1 star: 5 times 1.0 times 1 equals 5. Add those up: 0 + 50 + 5 = 55.

**Murphy wins the second seat** with a weighted total of 55.0.

Notice what happened: Both Group 2 and Group 3 still had full ballot weight (1.0) because neither was allocated after Round 1. Group 2 gave Murphy 5 stars. Group 3 gave Murphy only 1 star. Together with Group 2's full-strength support, Murphy was the clear winner this round. The system worked as designed -- voters who had not yet been represented got to drive this decision.

**Allocating ballot weight again:** Sort voters by weighted score given to Murphy, from highest to lowest:

| Weighted Score for Murphy | Voter Group | Voters | Current Weight | Total Weight in Tier |
|:-------------------------:|:-----------:|:------:|:--------------:|:--------------------:|
| 5.0 (weight 1.0 x score 5) | Group 2   | 10     | 1.0            | 10.0                 |
| 1.0 (weight 1.0 x score 1) | Group 3   | 5      | 1.0            | 5.0                  |
| 0 (weight 0.333 x score 0) | Group 1   | 15     | 0.333          | 5.0                  |

The quota is 10. The top tier (Group 2, weighted score 5.0) has exactly 10 units of ballot weight -- precisely one quota. All 10 voters in this tier are fully allocated: their weight goes to zero.

The 1.0 tier (Group 3) and the 0 tier (Group 1) are below the allocation boundary. They are untouched.

**Summary after Round 2:**

| Voter Group | Voters | New Ballot Weight | Why |
|-------------|:------:|:-----------------:|-----|
| Group 1     | 15     | 0.333             | Gave Murphy 0 stars -- below the allocation boundary |
| Group 2     | 10     | 0.000             | Gave Murphy 5 stars -- fully allocated as Murphy's quota |
| Group 3     | 5      | 1.000             | Gave Murphy 1 star -- below the allocation boundary |

Group 2 voters gave Murphy 5 stars and have now been fully allocated -- their weight is zero. They elected their candidate and are completely represented. Group 3, despite giving Murphy 1 star, retains full ballot weight because the quota was consumed entirely by Group 2 before reaching them.

#### Round 3: Filling the Third Seat

Recalculate scores one more time with the latest ballot weights. Both Lin and Murphy are removed.

**Table 5: Round 3 Weighted Score Calculation**

| Candidate | Group 1 (15 x 0.333) | Group 2 (10 x 0.000) | Group 3 (5 x 1.000) | Weighted Total |
|-----------|:---------------------:|:---------------------:|:--------------------:|:--------------:|
| Garcia    | 15 x 0.333 x 4 = 20.0 | 10 x 0 x 0 = 0      | 5 x 1.0 x 2 = 10.0  | **30.0**       |
| Kim       | 15 x 0.333 x 2 = 10.0 | 10 x 0 x 1 = 0      | 5 x 1.0 x 5 = 25.0  | **35.0**       |
| Patel     | 15 x 0.333 x 0 = 0    | 10 x 0 x 4 = 0      | 5 x 1.0 x 0 = 0     | **0.0**        |
| Brooks    | 15 x 0.333 x 1 = 5.0  | 10 x 0 x 0 = 0      | 5 x 1.0 x 3 = 15.0  | **20.0**       |

**Kim wins the third and final seat** with a weighted total of 35.0.

What drove this result? Group 3 had retained full ballot weight throughout the entire election -- they were never above the allocation boundary in either previous round. Their 5 voters at full strength, each giving Kim 5 stars, contributed 25.0 to Kim's total. Group 1 contributed 10.0 at their reduced weight. Garcia, by contrast, drew 20.0 from Group 1 and 10.0 from Group 3 -- more from Group 1 but less from Group 3. Kim's advantage came from Group 3's strong preference (5 stars for Kim versus 2 stars for Garcia), and Group 3's full ballot weight gave that preference its full effect.

Group 2 contributed nothing to any candidate in Round 3. Their ballot weight was zero -- they were fully allocated after Murphy's election. This is exactly the point of the allocation mechanism: voters who have been represented step aside entirely, making room for underrepresented voters to drive the remaining decisions.

#### What the Final Result Tells Us

| Seat | Winner | Elected By |
|------|--------|------------|
| 1    | Lin    | Group 1 voters (who gave Lin 5 stars) -- allocated as Lin's quota |
| 2    | Murphy | Group 2 voters (who gave Murphy 5 stars) -- fully allocated as Murphy's quota |
| 3    | Kim    | Primarily Group 3 voters (who retained full weight throughout and gave Kim 5 stars) |

Now compare each group's share of voters to their share of representation:

| Voter Group | Voters | Share of Electorate | Seats Won | Share of Seats |
|-------------|:------:|:-------------------:|:---------:|:--------------:|
| Group 1     | 15     | 50%                 | 1 (Lin)   | 33%            |
| Group 2     | 10     | 33%                 | 1 (Murphy) | 33%           |
| Group 3     | 5      | 17%                 | 1 (Kim)   | 33%            |

With only three seats to fill, perfect proportionality is not possible -- you cannot divide three seats into exact 50/33/17 portions. Group 1 is somewhat underrepresented and Group 3 somewhat overrepresented. This is a mathematical limitation of small numbers, not a flaw in the method. As district size increases (the Act allows up to 7 seats per district), proportional accuracy improves.

The important point is that every group of voters received representation. In a traditional single-winner election, only one group would win and the other two would get nothing. Here, all three groups elected someone who reflects their preferences.

The allocation mechanism created clean constituency boundaries. Group 1's strongest supporters were allocated to Lin. Group 2's supporters were fully allocated to Murphy. Group 3, whose preferred candidates had not yet won, retained full ballot weight throughout and used that weight to elect Kim in the final round. Each group's influence was spent on candidates they actually supported, and nobody had to vote strategically to make this happen.

---

## Part III: How STAR and Allocated Score Fit Together

### Same Ballot, Different Counting

The Act's voting methods are designed so that you do the same thing on every congressional race: score each candidate from 0 to 5 stars. Whether you are voting for Senator or Representative, the ballot looks the same and your task is the same.

What changes is behind the scenes. For single-winner races, your scores are counted using STAR voting's two-step process (scoring round, then automatic runoff). For multi-winner House races, your scores are counted using Allocated Score's round-by-round allocation with ballot weight.

This consistency is intentional. There is only one skill to learn. If you know how to rate things on a 5-star scale -- and most people already do, from restaurant and product reviews -- you know how to vote under the Act.

### What Stays the Same, What Changes

| Feature | STAR (One Winner) | Allocated Score (Multiple Winners) |
|---------|-------------------|------------------------------------|
| What you do | Score candidates 0-5 stars | Score candidates 0-5 stars |
| Number of winners | 1 | 3 to 7 |
| How winners are determined | Highest scores, then head-to-head runoff | Highest weighted scores, round by round |
| Ballot weight | Not applicable | Allocated from strongest supporters as candidates win |
| Proportionality | Not applicable (one winner) | Seat shares reflect voter shares |

### Who Manages the System?

The Act creates the **Electoral Science Office (ESO)**, a permanent technical agency responsible for maintaining and improving the voting methods over time. The ESO operates within a three-tier protection framework that matches each element's level of protection to its significance.

Some things are **statutory principles** -- the democratic commitments that define how the voting system must work: the requirement that all voters can score all candidates, the requirement that all voters are treated equally, and the proportional outcome requirement for multi-winner elections. These can only be changed by an Act of Congress.

Other things are **protected design elements** -- core design choices like the 0-5 star scoring range, the treatment of unscored candidates, and the structure of the automatic runoff. The ESO can study these and propose improvements, but changes require Congress to affirmatively approve them.

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

No. Every candidate's score is added up independently. Giving your second-favorite candidate 4 stars does not take anything away from the 5 stars you gave your favorite. In the STAR runoff, only your preference between the two finalists matters. In Allocated Score, ballot weight is allocated starting from the winner's strongest supporters. If a quota's worth of ballot weight is consumed before reaching voters who gave lower scores, those lower-scoring voters are completely unaffected -- their influence is fully preserved for the remaining seats.

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

**Step 3.** Sort all ballots by their weighted score for the elected candidate, ws(b) = w(b) x s(b, c*), in descending order.

**Step 4.** Working from the top of the sorted list, identify the **split point** -- the highest weighted score value v such that the total weight of all ballots with ws(b) strictly greater than v is less than Q. This identifies the cusp tier: the score tier containing the quota boundary.

Let spent_above = sum of w(b) for all ballots where ws(b) > split_point.

- For all ballots where ws(b) > split_point: set w(b) = 0 (fully allocated).
- For all ballots where ws(b) = split_point (the cusp tier): compute the fraction f = (Q - spent_above) / (sum of w(b) for ballots where ws(b) = split_point). Set w(b) = w(b) x (1 - f) for each ballot in this tier.
- For all ballots where ws(b) < split_point: w(b) is unchanged.

**Step 5.** Remove c* from the set of remaining candidates. Repeat from Step 1.

**Properties:**

The total weight spent in each round equals Q (the quota), ensuring that each elected candidate "costs" an equal share of the electorate's total voting power. Allocation proceeds from the top of the sorted list: voters who contributed the most to the winner's election are fully consumed first. Voters at the cusp of the quota boundary share the remaining cost equally through fractional surplus handling, preserving equal treatment of voters who scored the winner identically. Voters below the cusp are completely unaffected -- their ballot weight is preserved in full for subsequent rounds. This sort-and-allocate mechanism creates hard constituency boundaries between voters who have been represented and those who have not, which is the structural property that produces proportional outcomes.

### A.3 Notation Summary

| Symbol | Meaning |
|--------|---------|
| B | Set of all valid ballots |
| b | A single ballot |
| C | Set of all candidates |
| c | A single candidate |
| c* | The elected candidate in a given round |
| k | Number of seats to fill |
| s(b, c) | Score assigned by ballot b to candidate c (0-5) |
| w(b) | Current weight of ballot b (starts at 1) |
| ws(b) | Weighted score of ballot b for a given candidate: w(b) x s(b, c) |
| Q | Quota (ballots per seat) |
| S(c) | Total score for candidate c (unweighted) |
| WS(c) | Weighted score for candidate c |
| f | Fractional surplus handling factor for cusp-tier ballots |

---

## Glossary

**Allocated Score.** The counting algorithm used for multi-winner elections under the Act. Voters score candidates 0-5 stars. Seats are filled one at a time: the highest-scoring candidate wins each round, and a quota's worth of that candidate's strongest supporters are allocated (their ballot weight is set to zero), with fractional surplus handling at the cusp. Allocated Score is the specific algorithm recommended for STAR-PR by the Equal Vote Coalition's research committee.

**Automatic runoff.** The second step of STAR voting. After the two highest-scoring candidates are identified, every ballot is checked to see which of the two the voter preferred. The one preferred by more voters wins. No separate runoff election is held -- it happens automatically using the scores already on your ballot.

**Ballot weight.** A number that represents how much influence your ballot still has. It starts at 1 (full influence). When a candidate you supported wins a seat, the system allocates weight from that candidate's strongest supporters first. If you are among the voters whose weight is consumed to fill the winner's quota, your weight goes to zero (fully allocated) or is fractionally reduced (if you are at the cusp). If you are below the allocation boundary, your weight is unaffected.

**Deterministic.** Means the same ballots always produce the same result. There is no randomness in the counting process (except for tie-breaking in rare cases). Anyone can recount the ballots and get the identical outcome.

**District magnitude.** The number of seats elected from a single district. A single-member district has a magnitude of 1. Under the Act, multi-member House districts have a magnitude between 3 and 7.

**Electoral Science Office (ESO).** A permanent federal agency created by the Act to maintain, evaluate, and refine the technical details of the voting methods, and to certify, evaluate, and maintain the algorithmically neutral districting algorithm used to draw congressional district boundaries. The ESO operates within a three-tier graduated protection framework: statutory principles require an Act of Congress to change, protected design elements require affirmative Congressional approval, and adjustable technical parameters can be refined by the ESO through a structured public process with Congressional oversight.

**Finalist.** In STAR voting, one of the two candidates who received the highest total scores and advance to the automatic runoff.

**Monotonicity.** A property meaning that giving a candidate a higher score can never hurt that candidate. If you increase your score for a candidate, it can only help them or make no difference -- it can never backfire and cause them to lose.

**Multi-member district.** A district that elects more than one Representative. Under the Act, most House districts elect between 3 and 7 Representatives.

**Proportional representation.** A system where the share of seats won by different groups of voters roughly matches those groups' share of the electorate. If 40% of voters prefer one set of candidates, they win roughly 40% of the seats.

**Quota.** The amount of ballot weight needed to fill one seat. Calculated by dividing the total number of voters by the number of seats. In an election with 100 voters and 5 seats, the quota is 20.

**Scoring round.** The first step of STAR voting. Every score from every voter is added up. The two candidates with the highest total scores become the finalists.

**Single-member district.** A district that elects one Representative.

**STAR voting.** Score Then Automatic Runoff. The method used for single-winner elections under the Act. Voters score candidates 0-5, the two highest-scoring candidates become finalists, and the finalist preferred by more voters wins.

**STAR-PR.** STAR Proportional Representation. The umbrella concept for a 0-5 star ballot counted with a proportional algorithm. Allocated Score is the specific counting algorithm recommended for STAR-PR. Other algorithms (such as Sequentially Spent Score and Sequential Monroe) were evaluated as alternative tabulation methods for STAR-PR during the Equal Vote Coalition's research process.

**Weighted score.** A candidate's score after ballot weights are applied. Calculated by multiplying each ballot's score for that candidate by that ballot's current weight, then adding up the results.

---

<!--
## Revision History

**Revision 5.7** (Current)
- Aligned with Rev 5.7 of the legislative text
- Corrected Allocated Score algorithm specification throughout: replaced incorrect proportional-spending formula with correct Monroe-type sort-and-allocate mechanism (sort voters by weighted score given to winner, allocate from the top, fractional surplus handling at the cusp, full weight preserved below the cusp)
- Recalculated all ballot weights and round results in the three-seat House district worked example using the corrected algorithm; winners unchanged (Lin, Murphy, Kim)
- Rewrote prose descriptions of the weight-reduction mechanism ("The Big Idea: Ballot Weight," "How Much Weight Gets Spent?," "How Votes Are Counted" step 3) to reflect sort-and-remove rather than proportional-spending
- Corrected STAR-PR / Allocated Score terminology: STAR-PR is the umbrella concept (star ballot + proportional algorithm); Allocated Score is the specific recommended counting algorithm. Revised Part II introduction, glossary entries for "Allocated Score," "Ballot weight," and "STAR-PR," and Part III comparison table
- Corrected Appendix A.2 split point definition: replaced "cumulative weight first meets or exceeds Q" with "highest weighted score value such that total weight strictly above is less than Q" to correctly identify the cusp tier
- Fixed residual proportional-spending language in Part IV FAQ ("Does scoring other candidates hurt my favorite?")

**Revision 5.6**
- Renamed from "Federal Elections Modernization Act (FEMA)" to "Congressional Elections Modernization Act (CEMA)"; all references, defined terms, and download paths updated throughout
- Presidential scope removal: removed presidential election references from Purpose section, STAR voting introduction, and Part III overview; the Act governs congressional elections only
- DPS 3.1 header compliance: removed "Published March 2026" and "Based on Rev 5.2" metadata lines per DPS Rev 3.1 Section 1.2
- Download link updated: path migrated to congress/cmf/cema/; added emoji prefix and parenthetical per DPS Rev 2.8 Section 1.9
- No changes to voting method descriptions, worked examples, or mathematical specifications

**Revision 3.0**
- Updated reference line from Rev 5.0 to Rev 5.2
- Corrected tier classification in "Who Manages the System?" section: moved 0-5 star scoring range from statutory principles (Tier 1) to protected design elements (Tier 2); replaced with "requirement that all voters can score all candidates" as the Tier 1 principle per Section 409(c)(1) and 409(d)(1)
- Added "treatment of unscored candidates" to protected design elements description
- Updated ESO glossary entry to include districting algorithm certification, evaluation, and maintenance responsibilities added in Rev 5.1
- Wrapped revision history in HTML comment block per DPS Rev 2.3, Section 1.4
- Added "Revision history available in the raw file." note per DPS Section 1.3
- Added download link per DPS Section 1.9
- No changes to voting method descriptions, worked examples, or mathematical specifications

**Revision 2.0**
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
-->

*Revision history available in the raw file.*

> 📥 [Download this document](https://github.com/albertintech/apai/blob/main/docs/congress/cmf/cema/voting-methods-technical-explainer.md) (opens on GitHub -- click the ⬇ download button)

---

*Prepared by Albert Ramos for The American Policy Architecture Institute*
