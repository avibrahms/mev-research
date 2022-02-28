---
id: <leave blank -- will be assigned by reviewers>
title: Classifying Sophisticated MEVs
team: avibrahms (main), fiiiu?, obadiaa?
created: 2022-02-28
---

## Background and Problem Statement
Lots of MEV opportunities involve multiple target addresses, accross multiple bundles, those aren't straightforward attacks and they are not easily identifiable by mev-explore. Weather it is for arbitrage, liquidation or more sophisticated attacks, there is a need to understand complex attacks better.

## Plan and Deliverables
We propose to build a series of machine learning algorithms, classifiers and clustering algorithms in order to unlock meaning from sophisticated MEV attacks. This feature will be added to mev-explore to enrich the knowledge of the community and prevent potential unforseen blind-spots, new attacks (some of which probably already using machine learning).
  
Machine learning is a great approach here as it removes the bias introduced by human interpretation. We simply provide the data to our models, and insights are extracted, weather it makes or doesn't make sense to us.
As per most machine learning approaches, our research will be based on trial and error. But we have a basic methodology that we describe here:
  
1. Clustering the bundlesBundle classifier (is it a fully contained attack, part of a bigger attack, 
Because bundles are the basic unit in relays, we propose to use them 
  
## References

