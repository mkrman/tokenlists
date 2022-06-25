# Avalanche Tokenlists

Token Lists is a specification for lists of token metadata (e.g. address, decimals, etc.) that can be used by any dApp interfaces that needs one or more lists of tokens. Anyone can create and maintain a token list, as long as they follow the specification. The community invites you to add your token to our tokenlists!

## Adding Your Token to an Existing List
### General Requirements

Token should be verified on the Snowtrace Explorer.
Token must be added to a list that it qualifies for:

ZSwap Tokenlist: Token must be on the Avalanche network.
Fuji Tokenlist: Token must be on the Fuji network.

### Adding Your Token

Add an entry in the tokens field of the appropriate tokenlist. Please use the checksum address. Here is an example using ZWAP:

{
  "chainId": 43114,
  "address": "0xADDRESS",
  "decimals": 18,
  "name": "ZSwap",
  "symbol": "ZWAP",
  "logoURI": "https://raw.githubusercontent.com/mrkman/tokens/main/assets/0xADDRESS/logo.png"
}
Update the timestamp field to the current timestamp.

Update the version field to adhere to semantic versioning:

Increment major version when tokens are removed
Increment minor version when tokens are added
Increment patch version when tokens already on the list have minor details changed (name, symbol, logo URL, decimals)
Note: Changing a token address or chain ID is considered both a remove and an add, and should be a major version update.

### Adding Your Token Logo

Token logos are hosted here.
