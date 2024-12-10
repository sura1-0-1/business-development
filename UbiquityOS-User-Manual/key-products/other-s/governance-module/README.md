# Governance Module



The Ubiquity Governance System is the core structure that empowers UBQ token holders to actively engage in decision-making processes and influence the development of the protocol. Through a decentralized and transparent system, governance participants can propose, vote on, and implement changes to the protocol, ensuring that the ecosystem evolves in a way that aligns with the interests of its community.&#x20;

The UBQ token plays a pivotal role in enabling this governance, allowing token holders to have a direct impact on key decisions, such as upgrades, parameter changes, and integrations, fostering a collaborative and decentralized environment.

The UBQ token is a key component of the Ubiquity ecosystem, representing the governance power of the community and enabling participants to influence the direction and evolution of the DAO. Initially, the UBQ token had a supply of zero, with new tokens being minted as users engage with Ubiquity's products.

UBQ is a perpetually inflationary ERC20 token, created to serve two primary objectives:

1. **To drive adoption by e**ncouraging wider use and integration of Ubiquity's products.
2. **To enhance product functionality by s**trengthening the overall ecosystem and its offerings.

The **UBQ token** has no predefined mint schedule but is released when circumstances require it (some cases will be shown in this document for uAD). To avoid hyperinflation of the UBQ token, each product in the Ubiquity system that is allowed to mint governance tokens will be subject to a product-wide penalty depending on the total amount of UBQ tokens minted by the protocol.&#x20;

This penalty is defined by the following curve:

<figure><img src="../../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

The minting of UBQ tokens does not follow a predetermined schedule. Instead, new tokens are generated when necessary based on product requirements. However, to prevent hyperinflation, the system introduces a product-wide penalty for excessive UBQ minting, which is determined by a specific curve. Early stages of a product may see no penalty, but as the total minted tokens increase (e.g., surpassing 47 million), the penalty rate will rise, discouraging excessive inflation.

**Example Scenario**:

* **Product P2** rewards users with UBQ tokens for completing actions with no initial penalty.
* **Product P1** has already minted 50 million UBQ tokens. For actions in P1, users will receive rewards that are subject to a penalty—51% in this case—reducing the effective amount of UBQ tokens awarded.

In the case of **uAD**, the protocol generates revenue through various mechanisms such as LP fees, seigniorage, and other sources. A portion of the proceeds is allocated to the **UBQ Fund**, which is used to **buy back** UBQ tokens from the market and provide liquidity (LP) on platforms like SushiSwap. These tokens are then burned, enhancing the liquidity of the UBQ token while maintaining a similar price impact to a buyback and burn mechanism.

Overall, the UBQ token is integral to Ubiquity's decentralized governance system, incentivizing participation and ensuring the health and stability of the ecosystem.
