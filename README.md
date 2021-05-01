# PinataParty

Based on [tutorial](https://medium.com/pinata/how-to-create-nfts-like-nba-top-shot-with-flow-and-ipfs-701296944bf) by Justin Hunter

## Some commands

Deploy project:
```
flow project deploy
```

Mint NFT:
```
flow transactions send --code ./transactions/MintPinataParty.cdc --signer emulator-account
```

Fetch metadata:
```
flow scripts execute --code ./scripts/CheckTokenMetadata.cdc 
```