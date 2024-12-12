# How Governance Module

The **Governance Module** in the Ubiquity ecosystem is central to enabling decentralized decision-making and managing the lifecycle of proposals.&#x20;

The governance system allows token holders to propose, **discuss**, **vote**, and **implement changes** within the Ubiquity ecosystem. This ensures community-driven development and prioritizes ecosystem health and stability.

Governance within the Ubiquity ecosystem operates across **four distinct phases**, designed to progressively transition from centralized decision-making to full community-driven governance. Each phase serves a specific purpose in **refining**, **implementing**, and **executing proposals** that benefit the ecosystem.

## **Four key phases**:

## **1, Rapid Prototyping Period:**

At the very beginning of each product, the Ubiquity team will have full access to **deploy changes** and **hotfixes** to the product as needed.  this will facilitate agile development and rapid iteration at the inception of a product. Furthermore, the core development team will have mint access to [uCR](https://github.com/ubiquity/ubiquity-dollar-development/wiki/11.-uCR) tokens to finance these changes.

This stage lasts approximately one month, but this may vary based on the project.

## **2, Cool Off Period**

The **Cool Off Period** is to introduce community feedback into the decision-making process. During this period, the Ubiquity team will maintain exclusive deployment privileges, ensuring that all proposed changes are subject to a transparent community discussion on the project’s forums. This approach allows for thorough vetting and ensures that the community plays an active role in discussions, providing feedback, and engaging with the initial stages of governance processes.&#x20;

The duration of the Cool Off Period is estimated to be around **three months**, although there is flexibility to adjust this timeframe based on the project's needs.

## **3, Fully Decentralized Governance**

**Fully Decentralized Governance** is to transition to a governance model that is entirely driven by the community. Under this model, control lies in the hands of the community, as proposals are created, debated, and executed based on the outcomes of community voting.&#x20;

Voting power within this framework is determined by the staking of **UBQ** tokens, where staked governance tokens dictate the weight of each vote. Additionally, a duration multiplier is applied, which means that longer staking periods result in greater voting power, following a predefined multiplier curve.&#x20;

<figure><img src="../../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

**Voting power** is determined by:

<figure><img src="../../../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

**Where**

* UBQ is the number of governance tokens staked in the governance module
* D is a duration multiplier, based on how long the tokens are staked for

The staking duration can range from a minimum of 1 week to a maximum of 208 weeks, allowing participants to have increased influence based on their level of commitment to the governance process.

The process for suggesting and implementing a proposal will closely follow UniSwap’s governance process, with tweaked parameters and an additional **Tender** step.

### **1, Temperature Check**:&#x20;

**T**he purpose of the Temperature Check is to determine if there is sufficient will to make changes to the status quo.

**Create a Temperature Check:**

1. Community member (A) asks a general, non-biased question to the community forum about a potential change (example: “Should uAD rewards for coupon holders be increased by 10%?”).
2. Voters vote on-chain to indicate their interest in bringing it forward to the next stage. Voting lasts 5 days, or until 5% of the voting pool backs the proposal.

If the proposal gains 5% of the pool backing, then it moves to the next stage - consensus check.

### **2, Consensus Check**:&#x20;

The **Consensus Check** stage ensures that a proposed idea, refined by community feedback, is thoroughly discussed and formally voted upon to determine whether it proceeds to the **Tender Process**.

This stage serves to establish formal discussions, creating a structured environment for stakeholders to engage in in-depth conversations about the proposed idea, allowing them to express concerns, share insights, and explore the implications. It also emphasizes the importance of refining proposal details, leveraging feedback from the community to strengthen the proposal, address potential challenges, enhance feasibility, and ensure that key considerations are not overlooked.

### To create a Consensus Check:

**Community member (A)** uses feedback from the Temperature Check post and creates a new poll that covers the options which have gained support. This poll can either be binary or multiple-choice but should include the option “Make no change” or its equivalent.

**Community member (A)** creates a new topic in the forum titled “Consensus Check — \[Your Title Here].” This will alert the community that this topic has already passed Temperature Check. Any topics beginning with Consensus Check that have not passed Temperature Check should be immediately removed by community moderators. Community member (A) makes sure that the discussion thread links to the:

* Original Temperature check thread
* Original Temperature check poll
* The new poll for the Consensus check

**Community member (A):**

* Reaches out to their network to build support for the proposal.
* Discusses the proposal and solicit delegates to vote on it.
* Responds to questions on the Consensus Check topic.
* Shares their viewpoint, although tries to remain as impartial as possible.

**The proposal should also include an implementation standard for the suggestion:**

* What companies/individuals are eligible for the implementation process
* Is a POC required
  * Is the POC partially or fully funded by the treasury?
* What is the maximum budget for the implementation?
* What are the deadlines?
  * For submitting a tender proposal
  * For the final deliverables
* What is the penalty for not delivering the project:
  * Within the deadlines
  * With a sufficiently good scope

Voting lasts 5 days. Whichever option has the majority of votes wins, and can be included in a Tender for Stage 3. A 67% pool quorum of the voting pool is required for the vote to be considered valid.

If the option “**Make no change**” wins, the Consensus Check topic should be closed by community moderators

### **3, Tender Process**:&#x20;

The **Tender Process** is designed to identify the most capable entity to implement a proposed initiative effectively. To achieve this objective, a mechanism is established wherein a public bidding process is opened, allowing applicants to submit detailed proposals. These proposals are required to outline essential components, including timelines, success criteria, requested subsidies, and penalty terms. Once the bids are submitted, the community engages in a voting process to rank the proposals based on merit, with the top-ranked applicant ultimately selected as the Implementation Party.&#x20;

The tender begins after the Consensus check, and applicants can submit their proposals for implementation. Those parameters include (but are not limited to):

* **Bit for the implementation**
* **Deadline**
* **Success criteria**
* **Request for penalty amount subsidy**
* **Request for audit subsidy**

This party is then required to stake a penalty deposit or secure subsidies from their supporters to ensure commitment to the project. If the selected Implementation Party fails to meet the agreed-upon conditions, the opportunity does not end there; instead, it cascades to the next-ranked bid, or the process restarts if necessary. The outcome of this process is that the winning bid progresses to the Governance Proposal stage, where it can be formally approved and set in motion. Through this structured approach, the Tender Process ensures that the most qualified entities are chosen to carry out community-backed initiatives while promoting transparency and accountability.

### **4, Governance Proposal**:&#x20;

The **Governance Proposa**l stage is crucial for finalizing and executing proposals following community approval. The primary objective of this stage is to ensure that the implementation party develops the proposal code thoroughly and undergoes an audit to verify its integrity and functionality; audit costs can be subsidized by the treasury to alleviate financial burdens.&#x20;

Once the code is audited and ready, a final voting period of five days is initiated, during which the community can cast their votes to determine whether the proposal will be approved.  Should the proposal receive the necessary backing, it enters a mandatory two-day time lock period, allowing for any final concerns to be addressed before execution. In instances where proposals are not approved, the implementation party has the opportunity to recalibrate and refine the proposal for another attempt, or the proposal can be outright rejected.&#x20;

**Ultimately**, when a proposal is approved, it proceeds to execution, marking the completion of the governance cycle. This structured approach emphasizes community involvement and accountability, ensuring that only well-vetted proposals move forward to implementation, thereby enhancing overall trust in the governance process.

#### **To create a Governance Proposal:**

The implementation party writes the code for the proposal. All proposed code should be audited by a professional auditor. This auditing process could be paid or reimbursed by the community treasury (audit subsidy)

Once the proposal is active, a **5 day voting period** is started. Ongoing discussions can take place in the community forum. If the proposal passes successfully, a two-day timelock will follow before the proposed code is executed. If the proposal does not pass, one of two things happen:

* The community can vote on a time extension in order for the implementation party to re-calibrate its proposal
* The community rejects the proposal, any penalties defined are slashed from the implementation party’s deposit and the Tender process begins anew

## **4, Governance Proposal Execution**

The **Governance Proposal Execution** stage is designed to implement the winning proposals that have emerged from the decentralized governance phase. The primary purpose of this stage is to ensure that these approved proposals are executed efficiently and effectively, guiding the community's initiatives toward realization. The process begins with Proposal Creation, which involves defining detailed parameters such as the implementation plan, budget, success criteria, and any penalties that may apply for non-compliance. This clarity helps all stakeholders understand the scope and expectations of the proposal.

Once the proposal is created, it moves to the **Voting phase**, which requires a quorum of **67%** of delegated tokens to pass. This threshold ensures that a significant portion of the community supports the decision, fostering democratic participation. After securing approval, approved proposals undergo a Time lock period lasting two days, designed to provide a buffer for any last-minute concerns before execution.

In terms of Accountability, if a proposal ultimately fails to meet its objectives, any defined penalties may be enforced, reinforcing the importance of adherence to the agreed-upon terms. Furthermore, the process allows for the initiative to revert to earlier stages, enabling the implementation party to recalibrate the proposal or resubmit it for another round of consideration.&#x20;

This structured execution framework ensures that governance proposals are not only carried out with community support but also maintains accountability and provides opportunities for improvement when necessary.

