# Governance Module

The **Ubiquity Governance System** is the core structure that empowers **UBQ token** holders to actively engage in decision-making processes and influence the development of the protocol. Through a decentralized and transparent system, governance participants can propose, vote on, and implement changes to the protocol, ensuring that the ecosystem evolves in a way that aligns with the interests of its community.

The UBQ token plays a pivotal role in enabling this governance, allowing token holders to have a direct impact on key decisions, such as upgrades, parameter changes, and integrations, fostering a collaborative and decentralized environment.

UBQ is a perpetually inflationary ERC20 token, created to serve two primary objectives:

1. **To drive adoption by e**ncouraging wider use and integration of Ubiquity's products.
2. **To enhance product functionality by s**trengthening the overall ecosystem and its offerings.

The **UBQ token** has no predefined mint schedule but is released when circumstances require it (some cases will be shown in this document for UUSD). To avoid hyperinflation of the UBQ token, each product in the Ubiquity system that is allowed to mint governance tokens will be subject to a product-wide penalty depending on the total amount of UBQ tokens minted by the protocol.

This penalty is defined by the following curve

<figure><img src="../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

### UBQ Tokens Emissions Curve

The emissions curve for UBQ tokens is designed to manage inflation and incentivize sustainable growth within Ubiquity’s ecosystem. Initially, products may distribute newly minted governance tokens without a penalty. However, once token emissions exceed 47 million, penalties of over 50% are applied to discourage further inflationary pressures.

#### Example

* **Product P2:** Initially rewards users with X governance tokens per action A, without any penalty due to minimal token emissions.
* **Product P1:** With a total emission of 50 million UBQ tokens over time, rewards for action B are subject to a 51% penalty. Thus, users receive Y x (1-51%) UBQ tokens per action.

#### UBQ Fund Allocation

Each of Ubiquity's products contributes a portion of their proceeds to the UBQ fund, sourced from:

* Treasury-controlled LP fees
* A percentage of seigniorage earnings

Funds in the **UBQ** fund are utilized for buyback and **liquidity provision (LP)** on platforms like **SushiSwap**. The strategy involves purchasing UBQ tokens from the market and using them as liquidity, burning the corresponding LP tokens. This method enhances liquidity while maintaining a similar market impact as a buyback and burn.

In the case of **UUSD**, the protocol generates revenue through various mechanisms such as LP fees, seigniorage, and other sources. A portion of the proceeds is allocated to the **UBQ Fund**, which is used to **buy back** UBQ tokens from the market and provide liquidity (LP) on platforms like **SushiSwap**. These tokens are then burned, enhancing the liquidity of the UBQ token while maintaining a similar price impact to a buyback and burn mechanism.

Overall, the **UBQ token** is integral to Ubiquity's decentralized governance system, incentivizing participation and ensuring the health and stability of the ecosystem.
