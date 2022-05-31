ERC 20 Standards
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### NOTE: This document is better viewed at https://docs.openzeppelin.com/contracts/api/token/erc20
#### This set of interfaces, contracts, and utilities are all related to the ERC20 Token Standard at https://eips.ethereum.org/EIPS/eip-20.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

#### There are a few core contracts that implement the behavior specified in the EIP:

```{IERC20}:``` the interface all ERC20 implementations should conform to.

```{IERC20Metadata}```: the extended ERC20 interface including the name, symbol and decimals functions.

```{ERC20}:``` the implementation of the ERC20 interface, including the name, symbol and decimals optional standard extension to the base interface.

#### Additionally there are multiple custom extensions, including:

```{ERC20Burnable}: ``` destruction of own tokens.

```{ERC20Capped}:``` enforcement of a cap to the total supply when minting tokens.

```{ERC20Pausable}:``` ability to pause token transfers.

```{ERC20Snapshot}:``` efficient storage of past token balances to be later queried at any point in time.

```{ERC20Permit}:``` gasless approval of tokens (standardized as ERC2612).

``{ERC20FlashMint}:`` token level support for flash loans through the minting and burning of ephemeral tokens (standardized as ERC3156).

`{ERC20Votes}:`support for voting and vote delegation.

`{ERC20VotesComp}:` support for voting and vote delegation (compatible with Compound’s token, with uint96 restrictions).

`{ERC20Wrapper}:` wrapper to create an ERC20 backed by another ERC20, with deposit and withdraw methods. Useful in conjunction with {ERC20Votes}.

#### Finally, there are some utilities to interact with ERC20 contracts in various ways.

`{SafeERC20}:` a wrapper around the interface that eliminates the need to handle boolean return values.

`{TokenTimelock}:` hold tokens for a beneficiary until a specified time.

The following related EIPs are in draft status.

`{ERC20Permit}`
