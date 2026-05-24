# Deployments

Date: 2026-05-22

## X Layer Testnet (chain ID 1952)

| Item | Value |
|---|---|
| Network | X Layer Testnet (Terigon) |
| Chain ID | `1952` |
| RPC | `https://testrpc.xlayer.tech/terigon` |
| Explorer | `https://www.okx.com/web3/explorer/xlayer-test` |
| Deployer | `0xBc25F65EC030f2A889556c92d2A2D91612Dd1F66` |

### Deployed Contracts

| Contract | Address | Notes |
|---|---|---|
| `StandoffGateway` | `0xCD6Cf4834e7FAB52c6ab4b60290cB36681E4963b` | Initialized with `[deployer, deployer]` as cosigners and `requiredApprovals=2`. For multi-party demos add a second signer via the gateway owner. |
| `ReceiptRegistry` | `0x8200236B2738AD04A0c844Be952Bf8aC2d2655b8` | Stand-alone receipt anchor. |

### Verification

`eth_getCode` returned 9,240 bytes for `StandoffGateway` and 2,904 bytes for `ReceiptRegistry`. Both contracts are live and queryable via the explorer above.

## Reproduce Deployment

```bash
export XLAYER_TESTNET_RPC_URL=https://testrpc.xlayer.tech/terigon
export DEPLOYER_PRIVATE_KEY=<funded testnet private key>

npx hardhat run scripts/deploy-xlayer.ts --network xlayer-testnet
```

Hardhat config exposes both networks:

- `xlayer` — chainId 196 (mainnet, not used in this submission)
- `xlayer-testnet` — chainId 1952 (this submission target)

## X Layer Mainnet

Status: not attempted. Hackathon submission is testnet-only.
