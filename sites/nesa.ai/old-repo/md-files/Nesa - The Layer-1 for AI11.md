3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/trustless-ai-oracle 1/4
Trustless AI Oracle
ARTIFICIAL INTELLIGENCE
 Playground Technology Research Token Docs Developers DNA X3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/trustless-ai-oracle 2/4
As a trustless AI oracle network, a critical step in Nesa's decentralized inference system
revolves around the aggregation of results submitted by individual nodes in the inference
committee, to deliver the o cial outcome of the inference task. The system implements a
default majority vote strategy within a smart contract.
Oracle Aggregation of Inference
Results
Any submitted result that does not align with the majority is  agged as faulty. The node
responsible for a faulty result is subject to a penalty. This could manifest as a loss of a
security deposit (slashing), a reduction in reputation score, or both.
This majority vote strategy ensures that the aggregated result reflects
the consensus of the committee, thereby reducing the likelihood of
erroneous outcomes due to individual node failures or malicious
behavior.
Once the o cial result is determined and faulty nodes are penalized, the smart contract
 nalizes the result and triggers the appropriate reward distribution to the nodes that
contributed to the majority result. Rewards are allocated as per the pre-de ned incentive
structure as dictated in the smart contract, balancing the costs incurred by nodes and
incentivizing continued honest participation in the system. The oracle reports the decision
back to the network.
Customized aggregation strategies are also o ered by Nesa and can range from simple
methods like majority voting or averaging to more complex techniques such as averaging
with outlier removal. This is helpful when certain use cases may demand more tailored
approaches.
 Playground Technology Research Token Docs Developers DNA X3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/trustless-ai-oracle 3/4
The AIVM implements the following veri cation methods to ensure reporting is accurate
and true: a) Outlier Identi cation: This involves statistical analysis within the aggregation
code to detect and handle outputs that deviate signi cantly from the consensus or
expected range of results. b) Publicly Checkable Proof: Similar to approaches used in
academic works like TownCrier, the model owner can require nodes to produce zero-
knowledge proofs or leverage trusted hardware attestations to publicly verify the
correctness of their computations. c) Outlier Quota and Proof Submission: Each node is
assigned an outlier quota, limiting the number of times it can deviate from the consensus
results before it is required to submit a proof of computation. If a node exceeds its quota,
it must provide such proof to maintain its standing in the network and avoid penalties.
 Playground Technology Research Token Docs Developers DNA X3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/trustless-ai-oracle 4/4
COPYRIGHT 2024 NESA FOUNDATIONGITHUB CAREERS TEAM TERMS PRIVACY CONTACT
 Playground Technology Research Token Docs Developers DNA X