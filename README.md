# Waifusion Contracts
Tracking & documenting on-chain contracts for the Waifusion NFT project. There are 3 contracts that make Waifusion work: Waifus, WaifuEnhancementToken (WET) and Dungeon.

## Waifus
This is the core waifu contract that extends the ERC721 (NFT) implementation. It contains the mappings of token owners, waifu names and more.

### Public Readable
`balanceOf(address)`
Returns how many waifus `address` owns

`isNameReserved(string)`
Returns if a name is applied to another waifu, therefore rendering it unavailable (case insensitive)

`ownerOf(uint256)`
Returns the owner address of the supplied waifu ID

`validateName(string)`
Returns if a name is valid; requirements:
- Has to be between 1 and 25 chars.
- Cannot have leading or trailing spaces
- Cannot contain continuous spaces
- Has to confirm to a-zA-Z0-9


## WaifuEnhancementToken
WaifuEnhancementToken, or WET is an extension of the standard ERC20 contract that is exclusive to the Waifusion world-wide harem. It serves two purposes:
- Allows waifu owners to give their waifus unique names
- Allows waifu owners to burn undesirable waifus in exchange for a new waifu from the dungeon

Every day, each waifu "drips" 10 WET. Name changes cost 1,830 WET and burning costs 5,490 WET

TODO: add contract code to repo

## Dungeon
TODO: dungeon documentation & contract code