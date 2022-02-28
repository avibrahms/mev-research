---
id: <leave blank -- will be assigned by reviewers>
title: Classifying Sophisticated MEVs
team: avibrahms (main), fiiiu?, obadiaa?
created: 2022-02-28
---

## Background and Problem Statement
Some MEV opportunities involve multiple target addresses, accross multiple bundles, those aren't straightforward and are not easily identifiable by mev-explore. Whether for arbitrage, liquidation, sandwitch, front-running, back-running or more, there is a need to detect complex attacks.

## Plan and Deliverables
We propose to build a series of machine learning algorithms in order to discover and unlock meaning from sophisticated MEV attacks. We propose to add this feature to mev-explore, enrich the knowledge of the community, prevent potential blind-spots and unforseen new kinds of attacks.
  
Machine learning will remove the bias introduced by human interpretation. (We simply provide a ML-based feature map for our analysis)
  
We describe below our methodology. And as per most machine learning approaches, it'll involve trial and error that we can't fully describe ahead of time.
  
1. Clustering: 
  (Because bundles are the basic unit in relays, we propose to use them as building blocks for our analysis.)
  Problematic bundles are those that don't appear to be an MEV attack on their own. And might be part of something bigger. 
  By designing and running state-of-the-art clustering algorithms, we'll be able to group bundles, not only by internal structure, but also by how they relate to their surrounding bundles. And look at how they relate to their respective environment.
 
2. Separation:
  Problematic bundles are bundles that are part of a bigger attack, therefore they either make sense on their own, or they don't. If they do, we classify them. If they don't we'll assume they are part of a sequence. Before we go to the next point: sequential analysis, we need to separate bundles by the attack they belong to. Multiple searchers might launch complex attacks in the same block, we distinguish between them 
  
3. Sequential analysis:
  The bundles are part of a sequence inside the block. We
  
## References

