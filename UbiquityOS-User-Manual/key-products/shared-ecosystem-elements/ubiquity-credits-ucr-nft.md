# Ubiquity Credits(uCR)NFT

The **Ubiquity Credit NFT (uCR NFT)** is a critical component of the Ubiquity protocol, designed to maintain the stability of the **Ubiquity Dollar (UUSD)** by incentivizing supply contraction during periods of downward price pressure. This mechanism ensures the system's adaptability during volatile debt cycles and sustained stability once the peg to $1.00 is achieved.

## Why Choose uCR NFT Over uCR?

* CR NFT issuance includes a premium, allowing users to receive more value for burning **UUSD**.
* Users can trade uCR NFTs if they need liquidity before redemption.
* &#x20;For bot traders or those closely monitoring inflation cycles, uCR NFTs offer a strategic edge.

## Features of uCR NFT

**Premium Mechanics**

UUSD holders receive uCR NFTs at a premium rate to incentivize burning during times of instability.\
Example:

* For a 15% premium, burning 100 uAD yields 115 uCR NFT.

uCR NFTs have an expiration period (currently 180 days) after issuance and expired uCR NFTs lose their redeemability.

uCR NFTs are tokenized to enable secondary markets, fostering liquidity during debt cycles. Initial trading occurs on Open Sea via wrapped uCR NFTs (grouped by expiry dates). Future plans include a dedicated uCR NFT marketplace with automated pricing and transaction tools.

## **Role of uCR NFT in Stabilization**

uCR NFTs are ERC-1155 tokens redeemable for UUSD during **Inflation cycles** (when the price of UUSD > $1.00). The primary purpose is to encourage UUSD holders to burn their uAD during **Debt cycles** (when TWAP < $1.00), reducing the token supply and applying upward price pressure.

### **1, Debt Cycle**

Occurs when the Time-Weighted Average Price (TWAP) of UUSD falls below $1.00 due to excess supply. Holders of UUSD can burn their tokens in exchange for uCR NFT at a premium rate,&#x20;

Calculated using the formula:&#x20;

&#x20;**Premium Rate = Base Amount + (Debt Ratio × Factor)**

**Debt Ratio (R) = Total uCR NFT Supply / Total UUSD Supply.**

The greater the debt ratio, the higher the premium, incentivizing further burning.

### **2, Inflation Cycle**

Occurs when the TWAP of **UUSD** exceeds $1.00. uCR NFTs can then be redeemed for **UUSD** at a 1:1 ratio, applying downward price pressure and maintaining the peg.

