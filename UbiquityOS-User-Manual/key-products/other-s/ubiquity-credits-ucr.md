# Ubiquity Credits(uCR)

**uCR tokens** are a key component of the Ubiquity Dollar (uAD) protocol, designed to manage the debt cycle and stabilize the uAD token's price around its $1 peg. These tokens incentivize participants to burn uAD tokens during a debt cycle by providing a mechanism to convert them into a form of perpetual credit.

uCR is issued at a premium that depreciates over time through a debt cycle.

**For example,**&#x20;

The credits may be issued at a 30% premium at the very beginning of the debt cycle, and this premium shall depreciate over the course of the debt cycle. These credits are 'perpetual' since they never expire like **uCR NFT** coupons. However, the credit to uAD redemption ratio shall become lower over time, unlike **uCR NFTs**, which can be redeemed for uAD at a guaranteed ratio of 1:1 as long as they are unexpired.



The purpose of these credits is to incentivize the purchase of debt right from the beginning of the debt cycle when the premium for uCR NFT isn't high enough for uAD holders to make a substantial profit. This may be especially handy when the price of uAD attains substantial stability around the $1 peg, and the possible arbitrage return on buying uCR NFTs at a low premium decreases.



<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

To effectively ensure the contraction of uAD supply during a debt cycle, it's critical to design incentives that align with the desired outcomes: encouraging participants to burn uAD early, consistently, and until the TWAP (Time-Weighted Average Price) reaches 1.&#x20;

Here are some potential strategies to achieve these goals:

1. **Early Burn Incentives:**

Offer additional rewards (e.g., in the form of tokens or other assets) for those who burn uAD early in the debt cycle. These rewards could decrease over time to encourage prompt action. Implement a tiered reward system where early burners receive higher rewards than those who burn later. This creates a sense of urgency.

2. **Continuous Burn Incentives:**

Ensure that the rewards for burning uAD decrease gradually as the TWAP approaches its minima and increases back towards 1, encouraging burning throughout the cycle.

Offer rewards at specific milestones of the uAD price decrease, incentivizing participants to continue burning even as the price drops.

3. **Sustained Burn Incentives until TWAP = 1:**

Provide an additional incentive for participants who continue burning until the TWAP equals 1, ensuring the complete contraction of uAD supply. Create a mechanism where the last few participants to burn enough uAD to help reach TWAP = 1 receive a unique bonus, encouraging participation until the end of the cycle.

