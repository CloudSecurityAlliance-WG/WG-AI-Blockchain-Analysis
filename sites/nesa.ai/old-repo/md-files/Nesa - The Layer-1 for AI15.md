3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/commit-and-reveal-subphases 1/3
Commit and Reveal
Subphases
 Playground Technology Research Token Docs Developers DNA X3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/commit-and-reveal-subphases 2/3
CRYPTOGRAPHY
Nesa's decentralized inference framework is composed of several core components:
users who submit inference requests, chain contracts responsible for veri cation and
aggregation of results, and nodes that process these requests.
Two Distinct Subphases: Commit
and Reveal
In the  rst phase, Inference Request Queueing, a user submits an inference request
transaction, which includes the necessary details for the inference task but does not
trigger the execution immediately. Instead, this transaction is registered into a queue
within the blockchain, prioritized based on fee paid.
The second phase, Inference Execution and Response, is initiated once the inference
request reaches the front of the queue. Separate transactions are created by the
designated inference committee, which is tasked with actually performing the inference
task. Upon completion, the results are recorded and disclosed.
This framework leverages a two-phase transaction structure,
utilizing the commit-reveal paradigm, to safeguard against dishonest
behavior and free-riding.
The separation of request and execution transactions o ers several advantages. Firstly, it
avoids the congestion that can occur when the blockchain waits for computationally
intensive inferences to complete. Secondly, it provides  exibility in resource allocation, as
the inference task can be processed in parallel with other blockchain operations. Finally, it
ensures that the blockchain maintains a consistent and fast block generation time,
regardless of the complexity or size of the AI models being inferred.
 Playground Technology Research Token Docs Developers DNA X3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/commit-and-reveal-subphases 3/3
COPYRIGHT 2024 NESA FOUNDATIONGITHUB CAREERS TEAM TERMS PRIVACY CONTACT
 Playground Technology Research Token Docs Developers DNA X