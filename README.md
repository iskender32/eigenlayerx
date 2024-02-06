# All the below fields are required for successful operator registration.

# To learn more about operator fields
# https://github.com/Layr-Labs/eigenlayer-contracts/blob/92ccacc868785350973afc15e90a18dcd39fbc0b/src/contracts/interfaces/IDelegationManager.sol#L21:
operator:
  # This is the standard Ethereum address format (ex: 0x6a8c0D554a694899041E52a91B4EC3Ff23d8aBD5) of your operator
  # which is the ecdsa key you created or imported using EigenLayer CLI
  address: 0x590E0E15B661fb0aCE72d6aa909d6c117cD4FcBF
  # This is the standard Ethereum address format (ex: 0x6a8c0D554a694899041E52a91B4EC3Ff23d8aBD5)
  # This is the address where your operator will receive earnings. This could be same as operator address
  earnings_receiver_address: 0x590E0E15B661fb0aCE72d6aa909d6c117cD4FcBF
  # This is the standard Ethereum address format (0x...)
  # This is the address which operator will use to approve delegation requests from stakers.
  # if set, this address must sign and approve new delegation from Stakers to this Operator
  # For now, you can leave it  with the default value for un-gated delegation requests
  # Once we enable gated delegation requests, you can update this field with the address of the approver
  delegation_approver_address: 0x0000000000000000000000000000000000000000
  # Please refer to this link for more details on this field https://github.com/Layr-Labs/eigenlayer-contracts/blob/92ccacc868785350973afc15e90a18dcd39fbc0b/src/contracts/interfaces/IDelegationManager.sol#L33:
  # Please keep this field to 0, and it can be updated later using EigenLayer CLI
  staker_opt_out_window_blocks: 0
  metadata_url: 

# EigenLayer Slasher contract address
# This will be provided by EigenLayer team
el_slasher_address: 

# Address of BLS Public Key Compendium contract
# This will be provided by EigenLayer team
bls_public_key_compendium_address:

# ETH RPC URL to the ethereum node you are using for on-chain operations
eth_rpc_url: 

# Signer Type to use
# Supported values: local_keystore
signer_type: local_keystore

# Full path to local ecdsa private key store file
private_key_store_path: <path-to>/test.ecdsa.key.json

# Full path to local bls private key store file
bls_private_key_store_path: <path-to>/test.bls.key.json

# Chain ID: 1 for mainnet, 5 for Goerli, 17000 for holesky, 31337 for local
chain_id: 5
