# Bet Contract

![](https://lh3.googleusercontent.com/yGfTSYv8z5BJgXS5X81v6b22xaSzRrZ4AqBHE8PxqUyzKHDlYhJKetK8JXGV5Ft47QhMJ0R7A-MUhkViqHwMF6\_YH5O98MnThXhKIeLgYp9m8u4piVlGQ5vZUw3ezSS85gfrFd0rDG\_oYYzL)

Bet contract covers most of the stuffs that happen on the platform. Like Liquidity contract, bet contract is also inherited from ERC1155. However, unlike liquidity contract, it issues different ERC1155 token for each bet. Each token represents a unique id incremented from 1. This id denotes a key inside a map that denotes the details for that bet. This idea was derived from Uniswap V3’s code.

UI calls createBets after approving DAI to be spent by the _createBets_ function on behalf of the user. This function takes arrays of gameId, the index of bets and the amount gambled for that bet. Then contracts first checks the risk parameters to see if less than 10% of bookie’s balance has been used for this match. If it has, it gets the odds internally, calculates the toWin amount and appends it to the map. Then it also updates the liquidity parameters. Finally a unique ERC1155 representing the bet is minted to the user.

Once user makes a bet they can see their bet. To show this, an array called active bets is stored. Then whenever someone wants to see theirs bets, the frontend loops through the active bets and find the users’s bets and shows that. Once an outcome is settled, UI sends the list of user’s outcome that was settled to the _**withdrawBets**_ functions. This function verifies that user owns the NFT and if the outcome is the winner, calls Liquidity contract to send the required DAI. Then the token is burned and the bet is moved to history.
