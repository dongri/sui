# Sui for Developer
https://docs.sui.io/build

# Sui install
```
$ cargo install --locked --git https://github.com/MystenLabs/sui.git --branch devnet sui

$ whereis sui
sui: /Users/dongri/.cargo/bin/sui
```

# Generate Address
```
$ sui client active-address
Config file ["/Users/dongri/.sui/sui_config/client.yaml"] doesn't exist, do you want to connect to a Sui full node server [yN]?Y
Sui full node server url (Default to Sui DevNet if not specified) : 
Select key scheme to generate keypair (0 for ed25519, 1 for secp256k1):
0
Generated new keypair for address with scheme "ed25519" [0x31a609d3cbe16abe1f91f036d00adcb80b773d8f]
Secret Recovery Phrase : [sport ability wish garlic shrug amazing police isolate able monitor candy crunch]
0x31a609d3cbe16abe1f91f036d00adcb80b773d8f

$ sui client addresses
Showing 1 results.
0x31a609d3cbe16abe1f91f036d00adcb80b773d8f
```

# Faucet
sui discord #devnet-faucet channel
```
!faucet 0x31a609d3cbe16abe1f91f036d00adcb80b773d8f

Brrrr... @dongri, 5 test Sui objects are heading to your wallet, check https://explorer.devnet.sui.io/addresses/0x31a609d3cbe16abe1f91f036d00adcb80b773d8f or with wallet cli sui client gas!
```

# console
```
$ sui console

sui>-$ env
```

# create nft
```
$ sui client create-example-nft
Successfully created an ExampleNFT:

----- Move Object (0xd2cafe101023a98ac0454ff800ec2da652bfd242[10843]) -----
Owner: Account Address ( 0x31a609d3cbe16abe1f91f036d00adcb80b773d8f )
Version: 10843
Storage Rebate: 25
Previous Transaction: Byin7UkyWMHx7CUeJawM758fDuP3i9qY5Va1iKtsShL1
----- Data -----
type: 0x2::devnet_nft::DevNetNFT
description: An NFT created by the Sui Command Line Tool
id: 0xd2cafe101023a98ac0454ff800ec2da652bfd242
name: Example NFT
url: ipfs://bafkreibngqhl3gaa7daob4i2vccziay2jjlp435cf66vhono7nrvww53ty
```