# PinataParty
Tutorial: How to Create NFTs Like NBA Top Shot With Flow and IPFS 

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

Link Pinnie token:
```
flow transactions send --code ./transactions/LinkPinnie.cdc
```

Mint Pinnie
```
flow transactions send --code ./transactions/MintPinnie.cdc --signer emulator-account
```

Check balance
```
flow scripts execute --code ./scripts/CheckPinnieBalance.cdc
```

Transfer Pinnie
```
flow transactions send --code transactions/TransferPinnieTokens.cdc --signer emulator-account
```

List Token for Sale
```
flow transactions execute --code transactions/ListTokenForSale.cdc
```

### Generate account

flow keys generate

flow accounts create --key YourNewPublicKey

To get AccountId:
```flow transactions status YourTransactionId```

Add 
```
"accounts": {
  "emulator-account": {
    "address": "f8d6e0586b0a20c7",
    "keys": "e5ca2b0946358223f0555206144fe4d74e65cbd58b0933c5232ce195b9058cdd"
  },
  "second-account": {
    "address": "<AccountID>",
    "keys": "<AccountPrivateKey>"
  }
},
```