# Liquidity

![](https://lh6.googleusercontent.com/sutg7d54UQ4slklXrurNPCqSrsybqiuxryDvTLFmeMtNXGVDZvMm2i\_WYK9pvN6U8z-XMS5wzLI3ZAs55Nx\_kLzuAkvc6EgSnkxQjUf4FI7S00mlBuCxKfkodiBtS8Qi5B4hoQvuaTtMZa1J)

Liquidity contract is inherited from ERC1155. ERC1155 standard has multiple tokens. Each address can have any amount of token for a given id. Item 0 in our contract represents the liquidity token.

In the frontend, UI calls addLiquidity contract after approving Liquidity contract to spend DAI on their behalf. The method moves DAI from the user’s wallet to the contract wallet, and if the transaction is successful, mints Item 0 of the same size as DAI transferred. This represents their stake in the liquidity pool. Furthermore, the date of the deposit is also logged.

When a user wants to remove liquidity, UI calls _**removeLiquidity**_ function with the appropriate amount. UI does an initial check to see if the user has that amount of withdrawable balance. This function gets the balance of token0 and checks the locked liquidity to check if the user has that amount. If they do, the contract sends DAI to the address and burns the proportional amount of token 0.
