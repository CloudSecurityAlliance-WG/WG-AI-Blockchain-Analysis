3/25/24, 11:37 AM Model Consistency and Inference Reliability | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/aivm-the-artiﬁcial-intelligence-virtual-machine/model-consistency-and-inference-reliability 1/3Model Consistency and
Inference Reliability
The AIVM’s primary purpose is to guarantee that AI models execute consistently across
various nodes in the network. Model consistency and inference reliability are the linchpins
of our platform, ensuring that every node produces identical results given the same inputs
and model parameters.
This section delves into the measures and specifications that we have put in place within
the AIVM to uphold these principles.
To achieve uniform model execution, the AIVM configuration must encompass every aspect
that could influence the computational outcome. This includes specifying the operating
system and compiler versions, along with precise compilation options and flags.
By rigorously defining the execution environment, we eliminate variability that could
otherwise arise from different software stacks.
If a model demands particular hardware characteristics, such as GPU acceleration or
specialized processing units like TPUs, these requirements are explicitly stated in the AIVM
configurations.
Moreover, features provided by the hardware that could potentially lead to inconsistent
execution, such as non-deterministic hardware instructions, are either strictly enabled or
disabled as appropriate.Configuration Specificity
Hardware Specifications
Nesa3/25/24, 11:37 AM Model Consistency and Inference Reliability | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/aivm-the-artiﬁcial-intelligence-virtual-machine/model-consistency-and-inference-reliability 2/3This approach ensures that all participating nodes can adequately prepare and align their
computational capabilities with the model’s needs.
Many AI models introduce randomness during inference, which can pose a challenge for
achieving deterministic and reproducible results. To mitigate this, we have implemented the
strategy of fixing the random seed, which ensures that any pseudo-random number
generation during inference leads to the same sequence of numbers across all executions.
In scenarios where public randomness is necessary, we integrate the cryptographic method
of Verifiable Random Functions  VRFs) that produce randomness that is both unpredictable
and provably unbiased.
This use of VRF in our system not only lends credibility to the random number generation
process but also makes it possible to verify the randomness after the fact.
The execution protocol within the AIVM prescribes a series of steps that every node must
follow. This protocol includes initialization procedures, data input conventions, model
execution, and output handling.
By standardizing the execution flow, we can reliably predict and replicate the behavior of AI
models across the network.
Before an AIVM kernel is approved and stored on the blockchain, it undergoes rigorous
validation to ensure compliance with the specified configuration and to confirm that it
yields consistent results across diverse environments.
A suite of tests is run in simulated multi-node scenarios to affirm that the kernel’s execution
is deterministic and immune to variances in the underlying systems.
The measures above coalesce to create a robust framework for model consistency and
inference reliability within the AIVM.
These provisions are critical for maintaining the integrity of our decentralized inference
system, guaranteeing that any node, regardless of its individual hardware or software
configurations, can reliably participate in the network and contribute to collective AI tasks.
With this standard of uniformity, we enable a diverse ecosystem of nodes to work together
seamlessly and trustlessly.3/25/24, 11:37 AM Model Consistency and Inference Reliability | Nesa
https://nesaorg.gitbook.io/nesa/nesa-gitbook/aivm-the-artiﬁcial-intelligence-virtual-machine/model-consistency-and-inference-reliability 3/3Previous
AIVM Architecture and Design
Next
On-Chain Model and AIVM Repository
Last updated 1 month ago