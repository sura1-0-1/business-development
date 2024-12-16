# Tokenomics

## **Ubiquity Tokenomics Overview**

Ubiquity's **Dollar (UUSD)** is a decentralized stablecoin designed to maintain its peg through a combination of **monetary and fiscal policies**. Recognizing the challenges faced by purely algorithmic stablecoins, Ubiquity adopts a hybrid approach, beginning with full collateralization and evolving towards partial collateralization.

***

## **Key Features of** UUSD **Tokenomics**

### **1. Collateralization Approach**

The collateralization approach begins with a strategy that is fully collateralized to establish a robust and stable foundation during the initial launch phase. As the platform matures, there is a gradual reduction in reliance on collateral, which aims to maintain stability while optimizing capital efficiency.&#x20;

### **What is Collateralization in UUSD?**

Collateralization is the practice of backing UUSD with real, tangible assets held in the protocol’s treasury. This ensures that the value of UUSD is stable and maintains its peg to the dollar. Ubiquity adopts a **hybrid collateralization approach** that evolves over time, starting with full collateralization and transitioning to partial collateralization.

***

### **What Collateral Does UUSD Currently Use?**

The **collateral backing UUSD** is composed of a diversified portfolio of dollar-pegged stable assets, ensuring stability and liquidity. The primary collateral types include:

1. **3CRV Tokens (Core Collateral):**
   *   **What are 3CRV Tokens?**

       3CRV tokens represent liquidity provider shares in Curve Finance’s **3pool**, which contains three leading stablecoins: **DAI, USDC, and USDT**.
   *   **Why 3CRV?**

       3CRV tokens are highly liquid and offer exposure to a basket of stablecoins, mitigating the risk of depegging from any single stablecoin. They allow the treasury to benefit from transaction fees and liquidity rewards on Curve.
2. **Direct Stablecoin Reserves:**
   * The treasury holds reputable stablecoins such as:
     * **USDC (USD Coin):** A highly regulated, fiat-backed stablecoin issued by Circle.
     * **DAI (MakerDAO’s Stablecoin):** A decentralized, overcollateralized stablecoin.
     * **USDT (Tether):** The most widely used stablecoin globally.
   * These stablecoins are kept in reserve to provide immediate liquidity and protect the peg.
3.  **Yield-Generating Collateral (via Yield Aggregator):**

    Stablecoins deposited into the **Yield Aggregator** are deployed into low-risk DeFi protocols,&#x20;

Such as:

* **AAVE and Compound:** Lending platforms providing interest on deposits.
* **Curve Finance:** Liquidity pools that generate trading fees.
* **Yearn Finance or Rari Capital:** Low-risk yield optimizers.
* Yield from these deployments flows back into the treasury to replenish collateral reserves.

### **2. Collateral Management**

The initial phase of the manual collateral buyback process is managed through the treasury wallet, providing an opportunity to test and refine various aspects of the system. This includes selecting suitable types of collateral, sourcing collateral through the Yield Aggregator, and determining the level of aggressiveness needed for buybacks.&#x20;

Once these processes have been thoroughly validated, buybacks will transition to automation via Transfer Hooks. This shift will occur during Ubiquity Dollar transactions, thereby enhancing both the efficiency and scalability of the buyback mechanism.

**How is Collateral Managed?**

The management of collateral involves two key phases:

1. **Initial Manual Buybacks (Current Phase):**
   * During the early stages, buybacks are performed manually through the treasury wallet.
   * **Manual Collateral Operations Include:**
     * Deciding the type of collateral to acquire.
     * Allocating stablecoins sourced from yield farming.
     * Adjusting the collateral ratio based on market conditions.
2. **Automated Buybacks (Future Phase):**
   * Buybacks will transition to automated mechanisms via **Transfer Hooks**, executed during UUSD transactions.
   * Automation improves efficiency, scalability, and response time to market fluctuations.

***

## **Ubiquity Ecosystem**

The Ubiquity ecosystem is designed with a modular approach, enabling individual products to function independently while benefiting from **synergies across products**. This ensures that the ecosystem's value grows as more products are integrated.

### **Current Components**

1. **Ubiquity Dollar Protocol**: The foundation of the ecosystem, built around the stability and utility of the UUSD stablecoin.
2. **Yield Aggregator**: A tool to optimize returns, which also plays a key role in collateral sourcing for the Ubiquity Dollar.

### **Shared Ecosystem Elements**

*   **🏦 Treasury**:

    Acts as the financial backbone, supporting collateral buybacks and funding ecosystem development. Enables sustainable growth and facilitates the transition to partial collateralization.
*   **👨‍⚖️ Governance**:

    Oversees decision-making across the ecosystem, transitioning from centralized to community-driven governance in structured phases.

### **Future Products**

The ecosystem is designed to support multiple products, each operating autonomously but benefitting from shared resources such as governance and treasury, creating synergies across the ecosystem.

***

The **Ubiquity Dollar Protocol** and its supporting ecosystem components are the first steps in building a scalable and resilient platform, demonstrating the potential of hybrid stablecoins in a decentralized financial ecosystem.
