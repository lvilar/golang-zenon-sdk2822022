# golang-zenon-sdk

# Description

BIP39 is the use of a mnemonic phrase to serve as a backup to recover your wallet and coins. 

BIP44 defines the standard derivation path for wallets that generate Pay-to-Public-Key-Hash (P2PKH) addresses.

Also has model where you can check Process,Os,Reward,Reward,RewardHistory,Plasma,Pillar,Token,etc. - Info and Response

# Example

```go
import "github.com/andrews-avanexa/go-zenon"
```

```go
mnemonic := "route become dream access impulse price inform obtain engage ski believe awful absent pig thing vibrant possible exotic flee pepper marble rural fire fancy"
keyPairAccount := 0
key_store := zenon.FromMnemonic(mnemonic, keyPairAccount)
var ks zenon.KeyStore
bs := []byte(key_store)
json.Unmarshal(bs, &ks)
```

# Output

```go
Mnemonic: route become dream access impulse price inform obtain engage ski believe awful absent pig thing vibrant possible exotic flee pepper marble rural fire fancy
Entropy: bc827d0a00a72354dce4c44a59485288500b49382f9ba88a016351787b7b15ca
Seed: 19f1d107d49f42ebc14d46b51001c731569f142590fdd20167ddeedbb201516731ad5ac9b58d3a1c9c09debfe62538379461e4ea9f038124c428784fecc645b7
Private Key: d6b01f96b566d7df9b5b53b1971e4baeb74cc64167a9843f82d04b2194ca4863
Public Key: 3e13d7238d0e768a567dce84b54915f2323f2dcd0ef9a716d9c61abed631ba10
Address: z1qqjnwjjpnue8xmmpanz6csze6tcmtzzdtfsww7
Core Byte: 0025374a419f32736f61ecc5ac4059d2f1b5884d
```
