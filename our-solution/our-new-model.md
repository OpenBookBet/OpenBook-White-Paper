# Our New Model

OpenBook operates on a new hybrid prototype that takes the elements necessary from both centralized and decentralized design ideals and meshes them to solve problems with both. As mentioned previously, this is accomplished by two groups of users, the Bettors and the Bookies. The Bookies here can be likened to the “house” in a traditional casino or sports book, and the Bettors place their bets against the single liquidity pool filled by the Bookies. More details on the individual processes of making a bet and providing liquidity to the pool can be found in sections 7 and 8. The diagram below depicts the simple operation scheme of our platform.

![](https://lh6.googleusercontent.com/k1Y9cvWMLUh590OiAqcBhb0z1bKXCJsTvMb3\_yCiwuVf58p4\_62NiHqyhn1kPLerd953pvZI4rm6GRVtlmTvI1Q4CpB3SBK82wgOCxTDqDpHsMuiDCZnxbZGbkj06Xu3rznBf4sSr13TyTsK)

The dual nature of our design echoes the peer-to-peer betting ideal put forth by the Web3 native sports betting platforms with the key difference being that all Bookies contribute to the same pool instead of individual markets for individual matches. With this simple change, we solve the low limits challenges of current decentralized betting services.

Current decentralized models use oracles from Chainlink to create matches and settle the outcomes. The calls these oracles make to Chainlink rack up expensive fees when tracking many matches. Also, most current oracles come with limits.

We didn’t want to follow this style at OpenBook, so we reinvent the wheel and create a different approach focused on incentives. We create an entity called Providers who will stake their OpenBook DAO tokens and run a script to get odds and outcomes from a third-party source. Providers communicate off-chain to create matches, settle outcomes, and update the odds when there is a big enough deviation. OpenBook DAO token holders can decide by vote at any time if they think the current Providers are acting with honesty.

When the DAO is small, however, there is no economic sense in acting honestly. To solve this, the OpenBook founders will act as Providers in the beginning stages. Over time as the ecosystem grows, the DAO will be launched and the task will be delegated to the Providers voted on by the DAO.
