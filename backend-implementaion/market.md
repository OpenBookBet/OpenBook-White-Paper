# Market

![](https://lh3.googleusercontent.com/AKMPvGJ2KfB82-7Trwm5UPPPm7L0RrTg3DBOuDuSDM42YtuURp8mdt7mdoUT114iIvBCEGNyXrW7wyxz8vp0qdzsovID6JiaIpvvpqpIqGKbZ6p1VDe39sWvGQvMH-4D\_5qpwctKMu16YP9v)

New Matches are created and settled from the Market contract. Only the provider address can call must of functions in the market contract. A market is started when provider calls _**startMarket**_ function with appropriate details like start time, match name, match details, series of bets available for the match, and the starting odds. This data is sent in an array, and multiple matches can be sent at the same time. The data is stored inside a map with an index that increases with every new call serving as the match id and the key in the map.

Before the match settles, providers can call the _**updateOdds**_ function to update the odds for the game.

![](https://lh3.googleusercontent.com/uCGj6UMuiOHs29VMeFXnuVv56pEr1FMbB5e-Pp-j6OfptrRjLcIhnf63Mt\_HbZOogxw1hVDAqBTJu5p9rBV3vvlBq8aLH-zcBhUtskYzNVWWZlcGjW\_NpCFYvN6Tt-RVS3K9fP6v6J9D0ApI)

The match is settled when the provider calls settleMarkets method with the index of the winning team. When a match is settled, this contract unlocks the liquidity the bet contract locked for this match.

Market contract also has many read-only functions that frontend calls to get details of a match. It returns all matches, match details by given id, and so on.
