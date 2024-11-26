# ETH is Money - Config Files
This is the main repository where anyone can find all the underlying datapoints that are used to aggregate metrics for ethismoney.xyz
The scripts for data aggregation can be found in the growthepie backend repository: https://github.com/growthepie/gtp/tree/main/backend/eim

---
## How to participate
Anyone can help by keeping our data as up-to-date and as complete as possible. In order to aggregate the datasets for our metrics we need certain underlying information which we'll explain more below.

---
## 1 - ETH Exported
The amount of ETH exported to other ETHconomies is calculated by checking the balances of the corresponding bridge contracts on Ethereum. We check for native ETH balances as well as for all derivatives balances (which can be found in eth_derivatives.yml).

If you noticed that certain ETHconomies (chains that use ETH in their ecosystem) are missing you can add them to the eth_exported_entities.yml file.
If you think that not all necessary ETH derivatives are being tracked you can add the missing ones in eth_derivatives.yml

---
## 2 - ETH Holders
Prominent entities or personalities that hold ETH. This list aims to be a transparent register of publicly known ETH holdings.

If we are missing holders or amounts, please add missing holders / addresses / transactions to eth_holders.yml

---

## 3 - ETH Supply
The ETH supply is retrieved from ultrasound.money API. The events are defined in ethereum_events.yml