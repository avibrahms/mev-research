---
id: <leave blank -- will be assigned by reviewers>
title: Classifying Sophisticated MEVs
team: avibrahms (main), fiiiu?, obadiaa?
created: 2022-02-28
---

## Background and Problem Statement
Some MEV opportunities involve multiple target addresses, accross multiple bundles, those aren't straightforward and are not easily identifiable by mev-explore. Whether for arbitrage, liquidation, sandwitch, front-running, back-running or more, there is a need to understand complex attacks.

## Plan and Deliverables
We propose to build a series of machine learning algorithms in order to unlock meaning from sophisticated MEV attacks. We propose to add this feature to mev-explore to enrich the knowledge of the community, prevent potential blind-spots in unforseen new kinds of attacks.
  
Machine learning will remove the bias introduced by human interpretation. (We simply provide the data to our models, insights are extracted, whether it makes or doesn't make sense to us.)
  
We describe below our methodology. And as per most machine learning approaches, it'll involve trial and error that we can't fully describe ahead of time.
  
1. Clustering algorithms: 
  sometimes, bundles are full blown attacks, other times they are part of a bigger attacks. The same way a person can act on its own or be part of a team. Because bundles are the basic unit in relays, we propose to use them as building blocks for more analysis. By running state-of-the-art clustering algorithms, we'll be able to group similar bundles and look at how they correlate in the bigger picture. 
  
2. Sequential analysis of transactions:
  We will also look at transations as words in a sentence, and get rid of the bundle structure, that way we 
  
## References

