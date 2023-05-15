# Vault contract

- LOCK operation
  The user requesting bridging initiates the LOCK function and submits the Bridging Fee. As a result, a LOCK event is triggered in the fromChain Vault, which completes the Token Lock process. Subsequently, the backend system intercepts this event and initiates the MINT process of the toChain Minter.

- RELEASE operation
  It is the reverse case of toChain Minter's BURN process. Once the Backend obtains the signature for the transaction that has been agreed upon, the RELEASE function is executed. This function is performed within the fromChain Vault and results in the completion of the Token Release.
