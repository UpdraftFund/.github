# 🪁Updraft
![updraft-512](https://github.com/UpdraftFund/.github/raw/main/profile/updraft-512.png)

* [Test Website](https://www.updraft.fund)
* [Updraft Discord](https://discord.gg/mQJ58MY6Nz)
* [Updraft Guide](https://guide.updraft.fund)
* [Updraft for orgs deck](https://docs.google.com/presentation/d/19Yz_sKd_6erlpmpTcYp-VpZvQBPd8HBOPfANqiEubeY)
* [Updraft overview deck](https://docs.google.com/presentation/d/1opRgIcf7iH_aiQzKpeVr110kt5L8bA6mtbjl2YGPXAU)

Get paid to find ideas, crowdfund and work on what you love.

## How it works

### Support ideas

Post an idea that would make your community or the world better. Support other people's ideas. If your idea or an idea you supported receives more support, you earn money.

Ideas with the most support rise to the top and receive more views from the public and people who can solve them.

### Fund solutions

Drafters propose solutions to ideas and optionally stake their own funds that their solutions will reach their funding goals.

If a solution doesn't reach its funding goal, funders receive a refund from the solution fund plus a portion of the drafter's stake. If the solution reaches its goal, congratulations!--you helped build something that will make the world better.

You also earn money from any funding that comes after yours. A drafter can continue to receive funding and add more goals while early funders continue to earn.

Funding flow diagram ([Link to larger version with explanations](https://hackmd.io/VAIblnwwRwCUA1bkUEli8A))
![updraft-funding-flow](https://github.com/UpdraftFund/.github/raw/main/profile/updraft-funding-flow.png)

## Vision

Public goods will be as easy to fund as for-profit ventures. DAOs, grant-makers and philanthropists will route their ideas and proposals through Updraft to engage a larger community for support, feedback and solutions.

## Why it works

Funding public goods suffers from three problems:

1. Preference revelation. Public goods are free; without a market it's hard to know the value of a public good and which people will benefit from it.
2. Free-riding. If someone expects a public good to be fully funded, they could try to save their money and let others pay for it. This loophole can result in an important public good never being provided or its providers being underpaid.
3. Assurance. Even if someone is willing to pay for a public good, they may be reluctant to support a solution that might fail if others don't also support it. These doubts compound in a negative feedback loop.

Updraft gets closer than other systems to solving the preference revelation problem by attracting attention through the possibility of a reward. This is a superior system than polling or voting in which the value of a single vote is negligible and rarely worth the effort to research different options.

The possibility of a reward also means that more people that would free ride are impelled to instead add their own support at a level they can afford. Even those that overpay (compared to the per-person value of the public good, but still within their personal budget) can feel good knowing that their favored solution was fully funded and the public good they care about will be available to more people.

Updraft is a [dominant assurance contract](https://en.wikipedia.org/wiki/Assurance_contract#Dominant_assurance_contracts), meaning that the *dominant* strategy for potential funders is to always fund the public good. This in turn encourages more funders, bringing down the per-person cost of funding. The dual prospects of winning a drafter's stake or contributing early and earning from follow-on supporters are a powerful motivation to fund underfunded goods.

## Decentralization

Updraft must be completely open-source and easy to fork. Some members of the global community might not like a dev's decisions, or they may prefer a different front-end. Anyone should be allowed to create their own version and manage it as they please.

## Bounties

Any project can make themselves more like a public good by using Updraft to create ideas as bounties. Drafters can start working on bounties even before they reach their funding goal, posting updates on their progress. Staking is always optional for solutions and may not be useful for bounties.

## Details

Updraft is built using [Attention Streams](https://docs.google.com/document/d/1TKA-K8YadRdgz-Qek01TUcCkRaI9CKCXGtJ31AbVWIU/edit?tab=t.0#heading=h.c8wdt9uwyj7r).

Support for ideas are paid in Updraft tokens(UPD). Idea creators set the *funder reward* for their idea as a percentage. This goes to previous funders of the idea. The idea creator doesn't need to pay the funder reward. Both idea creators and contributors pay an anti-spam fee[^1](in UPD). The rest of a contribution is stored and used to determine future earnings as follow-on support comes in. The contribution and earnings can be withdrawn at any time; this encourages funders to reduce support for stale ideas. Ideas with the highest *interest* (total shares generated; called "relative support" in the Attention Streams doc) are sorted at the top of the default ordering and searches in Updraft.

A solution drafter pays an anti-spam fee[^1] (in UPD), sets a funding deadline, a stake amount (also in UPD), a funding goal (in a token they choose), and a funder reward. Solution funders pay the funder reward to previous funders. What remains goes to a locked solution fund. If the goal isn't reached by the deadline, the stake is paid to solution funders (split in proportion to shares, just like funder rewards) and all contributions to the solution fund are refunded.

Funders can also add any amount to the drafter's stake to attract follow-on supporters; they will get their full stake back if the solution reaches its goal and part of it back (since it's split among funders) if it doesn't.

After a goal is reached, funders can still make contributions (from which they still pay funder rewards). A drafter can extend their solution with a new goal, stake, and deadline to continue to fund their efforts or new related efforts.

When creating a solution, the drafter sets the following parameters:
* funder reward % to solution funders. (This isn't paid or earned by the drafter.)
* funding deadline
* stake amount
* funding goal
* funding token

## Features

Many of these features may not be available at launch, but could be proposed as ideas for improving Updraft.

### Search, sort and filter

Updraft is launching with views for ideas with high interest, new ideas, solutions nearing their deadline, ideas from followed accounts, ideas with watched tags, and full-text searches on idea names and descriptions.

#### Future views
* Solutions
  * Solutions using a specific token
  * Solution funding > X

### Ideas for you

Recommendation engine to show ideas similar to ones a user supported in the past, or suggest ideas based on cohort analysis (e.g. you supported idea X; people who supported X also supported Y).

### Anti-spam fee set by community

Set the anti-spam fee amount using a continuous median vote. Anyone who is Aura verified as a unique human is eligible to vote.

### Comments

Allow anyone to comment on ideas and solutions. This will require moderation.

### Aura scorecards

[Aura](https://brightid.gitbook.io/aura) players in the Updraft domain create score cards rating drafters on how well they implemented their solution and how effective it was in achieving the parent idea.

#### Benefits

* People will trust solutions more and be more willing to add follow-on support if they see positive score cards for drafters and funders.
* Drafters and funders could be exempt from anti-spam fees if they have a (revokable or expirable) badge from Aura.

#### For solutions

[Aura](https://brightid.gitbook.io/aura) scorecards for the solutions, where experts evaluate the validity and impact of solutions, idea-solution fit, the track record of drafters, and sniff out scams.

They can also report on the quality and impact of a funded solution's implementation.

#### For drafters

Drafters that create multiple solutions can request their own score cards.

#### For funders

Frequent funders (DAOs, philanthropists, grant-makers) can also request to have their own score cards.

### Streaming, splitting, vesting, and clawback

A solution can set their solution fund to stream, vest or split (to multiple recipients or milestones) which takes effect once the goal is reached. These settings can help contributors feel safer about funding the solution.

A solution can configure Aura (see above) as a judge to provide funder clawback. If Aura finds the solution to be poorly implemented, any tokens left in the solution fund will be returned to funders proportional to their contributions.

## UPD Tokens

There is a fixed supply of 100B UPD minted on Ethereum mainnet and available from liquidity pools on various networks.

### How UPD tokens are used

* Anti-spam fees are paid in UPD (creating and supporting ideas, creating solutions, updating solutions, editing your profile).
* Supporting an idea always uses UPD.
* Staking on a solution always uses UPD.

Solution funding can use UPD or any token the solution drafter chooses. There are no fees for funding a solution.

### Liquidity pools and voting

90B+ UPD will go into liquidity pools so anyone can buy UPD. The LP tokens will be burned to provide permanent liquidity.

Initially, 100B UPD will be added to a UPD-USDC pool on Arbitrum, but final sizes, networks, and token pairs of liquidity pools will be based on the outcome of [votes described in the user guide](https://guide.updraft.fund/updraft/voting/voting).

### Founder's fund

A maximum of 10B UPD will go to the *founder's fund*: a grant-making body that funds ideas and solutions on Updraft.

### UPD Faucet

Anti-spam fees will go to [Unitap](https://unitap.app) to be distributed to anyone interested in using Updraft. This ensures no one is excluded from using Updraft because they can't pay the fees.

[^1]: The anti-spam fee for an idea is the greater of a % fee (e.g. 1%) and a low, fixed fee (e.g. 1 UPD). The % fee discourages someone from contributing to their own idea just to boost it in the sort order. Drafters pay the low, fixed anti-spam fee.
