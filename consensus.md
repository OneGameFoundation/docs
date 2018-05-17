---
layout: single
sidebar:
  nav: "docs"
---

### Consensus 
-----------------------------

Decentralization relies on consensus, and One Game will use Popularity Rank (Rp) and Competitiveness Rank (Rc) as a consensus mechanism.   Rp and Rc measure the activeness of developers and players, and the platform will periodically re-compute PR and CR for each developer and player.
These two consensus mechanisms enable decentralized governance and a self-evolving platform based on voting:

***Popularity Rank, defines the popularity of the land created by developers.***

***Rp(l, i+1)= kp ∈ Pt(p,l)T(p)+(1-k)Rp(l, i)***

Here, Rp(l, i+1) and Rp(l, i) respectively represent a land l ’ s Popularity Rank in the current period (period  i+1), and the previous period (period i); k is a number between 0 and 1, and represents the weight of the current period; P is the set of all the players that visited land l in the current period, and p represents a single player; t(p,l) represents the time that a single player p spent in land l , and T(p) is the time that player p spent in all the land in the current period.
Rp(d, i)= l ∈ L(d)Rp(l, i)
A developer d’s Popularity Rank Rp(d, i) equals to the sum of all of his land’ Popularity Ranks Rp(l, i) , where l represents a single land, and L(d) is the set of all the land created by d. 

***Competitiveness Rank, defines players’ performance in different games created by developers.***

***Rc (p, i+1)= kl ∈ LRp(l, i)s(l, p)S(l)+(1-k)Rc(p, i)***

Here, Rc(p,i+1) and Rc(p, i) represent a single player, p ’s Competitiveness Rank in the current period and the previous period; k is a number between 0 and 1, and represents the weight of the current period; L is the set of land that player p visited in the current period, and l represents a single piece of land; s(l, p) represents a single player p ’s performance score in land l, and S(l) presents the sum of all the scores from different players in land l.
Please take note that the popularity rank Rp(l, i) of the previous period is used as a weight in the formula. In other words, players need to gain scores in more popular games in order to better increase their Competitiveness Rank. 
