# Core Concept

The fundamental idea behind the Equito Bridge is to have a separation of concerns between the Frontend and Backend, which are responsible for sending requests and monitoring the status of the bridge-related blockchain. The implementation approach of this concept involves deploying two distinct instances, with no direct communication or knowledge of each other.

In the Frontend, requests are sent to each side of the bridge-related blockchain, while the status finalization on the other side is monitored by either listening for smart-contract program updates or checking the local state of the associated wallet, depending on the chain mechanism and functionalities.

On the Backend, services listen to smart contracts on each chain and wait for new approvals, which are then update the status of smart contracts.

The bridge process fulfillment is followed through listening to smart contract transactions finalization with specific signatures associated with the exact bridging process started by the same Frontend instance, which is controlled by the Smart Contract.

The token mechanisms in place vary depending on the chains. For Algorand, LOCK/RELEASE is used, while on Ethereum, MINT/BURN is used.
