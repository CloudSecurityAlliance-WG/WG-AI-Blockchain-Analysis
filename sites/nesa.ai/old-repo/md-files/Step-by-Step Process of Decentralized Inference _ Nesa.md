3/25/24, 11:38 AM Step-by-Step Process of Decentralized Inference | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/decentralized-inference/step-by-step-process-of-decentralized-inference 1/6Step-by-Step Process of
Decentralized Inference
The following outlines the decentralized inference process, taking into account the
techniques and protocols established within the previous sections:
Users submit inference requests to the blockchain. Each request includes the user’s input
data for the AI model and the fee paid by the user, which determines the priority of the
request in the system.
Requests are registered in a smart contract that acts as a priority queue manager. The
smart contract organizes the requests based on the respective fees, ensuring those who
paid higher fees receive higher priority in the execution queue.
At the beginning of each slot, a committee of nodes is selected to perform the inference
task. The selection is based on the output of a VRF that each node executes using its
private key. Nodes generating qualifying random numbers are chosen for the committee.
The selected committee of nodes independently performs the requested AI infer- ence
task. Each node computes the result using the input data provided in the user’s request.Step 1: User Request Submission
Step 2: Priority Queue Management
Step 3: Inference Committee Selection
Step 4: Inference Execution
Step 5: Commitment to Inference Results
Nesa3/25/24, 11:38 AM Step-by-Step Process of Decentralized Inference | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/decentralized-inference/step-by-step-process-of-decentralized-inference 2/6To prevent free-riding, each node in the committee commits to its computed infer- ence
result using a cryptographic commitment scheme. This involves sending a hash of the
result and a nonce to the blockchain within a specific timeframe.
Within a subsequent timeframe, each node reveals its committed inference result by
submitting both the result and the nonce to the blockchain. If a node fails to reveal its
result, submits after the deadline, or reveals a result that does not match its commitment, it
faces a penalty.
Submitted inference results are collected by a smart contract that performs a majority vote
to determine the consensus result. The result most frequently reported by the committee is
considered the correct outcome.
The smart contract identifies and penalizes nodes that submitted incorrect results (not
aligning with the majority). Penalties may include slashing of stakes or reduction in
reputation. Nodes that contributed to the majority result receive rewards, as specified by
the system’s incentive structure, for their accurate and honest work.
The smart contract finalizes the consensus result of the inference task and records it on
the blockchain. The user is notified of the result, which concludes the inference process.
This step-by-step summary encapsulates the core sequence of operations within Nesa's
decentralized inference system. It details the journey from request submission to the final
delivery of the consensus inference result, highlighting the roles of smart contracts, priority
queues, committee selection, result commitment and reveal, and aggregation via majorityStep 6: Reveal of Inference Results
Step 7: Result Aggregation and Majority Vote
Step 8: Penalty Enforcement and Reward Distribution
Step 9: Finalization and User Notification3/25/24, 11:38 AM Step-by-Step Process of Decentralized Inference | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/decentralized-inference/step-by-step-process-of-decentralized-inference 3/6vote, all without any specific privacy-preserving or cryptographic enhancements from
Chapter 4.
The system ensures a transparent, fair, and secure process, motivating nodes to produce
accurate results and maintaining reliability across the network.
Nesa's default aggregation system by smart contract epitomizes an equilibrium between
democratic principles and technological enforcement, allowing us to mitigate risks
associated with node aberrance or malicious intents. By provision of penalties and
reputation diminution for deviant or deceitful submissions, we are engendering a self-
regulating ecosystem that encourages computational precision and integrity.
The process maintains detailed control over results set retrieval, an array of sophisticated
statistical methods for conclusive consensus, and reward allocation commensurate with the
predefined incentives ensuring adversarial resilience and motivation for continued honest
engagement by Nesa miners.3/25/24, 11:38 AM Step-by-Step Process of Decentralized Inference | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/decentralized-inference/step-by-step-process-of-decentralized-inference 4/6
3/25/24, 11:38 AM Step-by-Step Process of Decentralized Inference | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/decentralized-inference/step-by-step-process-of-decentralized-inference 5/6Previous
Aggregation of Inference ResultsOff-chain and on-chain algorithms for the Commit phase. The Commit phase is stage one of the two-
part subphase for Nesa's commit-reveal paradigm within the system’s decentralized inference protocol.
Off-chain and on-chain algorithms for the Reveal phase. The Reveal phase is stage two of the two-part
subphase for Nesa's commit-reveal paradigm within the system’s decentralized inference protocol. The
Reveal phase allows nodes to disclose their previously committed results. Each node must reveal both
the result m and the nonce r used in the commitment, allowing others to verify the hash against the
commitment made in the previous phase. This phase also has a timeout limit, and failure to reveal on
time, or revealing a different result from what was committed, will result in punitive measures against the
offending node. After the reveal, submitted inference results are collected by a smart contract that
performs a majority vote to determine the consensus result. The result most frequently reported by the
committee is considered the correct outcome.
3/25/24, 11:38 AM Step-by-Step Process of Decentralized Inference | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/decentralized-inference/step-by-step-process-of-decentralized-inference 6/6Next
Hybrid Design for Enhanced Privacy
Last updated 1 month ago