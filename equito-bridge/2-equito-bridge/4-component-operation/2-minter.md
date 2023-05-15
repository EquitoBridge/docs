# Minter contract

- MINT operation
  It is the reverse case of fromChain Vault 's LOCK process.
  After the Backend collects the signature for the agreed transaction, MINT function is executed.
  MINT function is executed in toChain Minter and Token Minted.

- BURN operation
  User requesting bridging executes BURN function with Bridging Fee.
  BURN event occurs in toChain Minter and Token Burn is completed.
  Backend catches the event, and run fromChain Vault's RELEASE Process
