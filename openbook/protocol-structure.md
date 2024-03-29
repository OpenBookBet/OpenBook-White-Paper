# Protocol Structure

For users to interact with our protocol, we designed the Web user interface to be sleek and easy to navigate. We also want it to feel familiar as well as fresh to regular sports bettors and crypto natives alike. The entire user interface puts an emphasis on understandability, ease of navigation, good visuals, and functionality. The initial pages will look like a sportsbook to welcome the Bettors, while the Bookie pages are catered to the liquidity providing Web3 natives. That said, the entire website is accommodating for all user experience levels and types and aims not to overcomplicate wherever possible. OpenBook will be deployed on the Polygon Network, a layer two solution built on top of the Ethereum blockchain.

![](https://lh4.googleusercontent.com/GOVdGUnnqBB0I9d4RyXMjIacuTzZrqkFCzVDhVIlBOGUstzwlCyOrUFPXSsj9UTol5l\_UzhPZWoPAsPANL\_cL2b3wutfajucSj4IC8AOV0ch-DQ3ZwGnBQg41OKGEMZAhFu09X5dyUkwvhbc)

## **Odds and Updaters**

Odds Providers will run a script that will get odds from a single or multiple centralized providers. Centralized providers use AI-generated odds and the success of such centralized bookies reveals that these odds provide profit over the long term. Providers will get odds from here and modify them for the selected commission spread. If the received odds are different than the current ones at a spread bigger than some percentage they decide is resonable, they will create an on-chain transaction and update the odds. This approach is taken because updating the odds only occurs a few times before a match goes live, so occasional updating is all that’s required. In return for running the script, Providers will get the winnings of their Vault.

## **Pooled Liquidity**

Each Vault will have a single pool of liquidity. Anyone who wants to be a Bookie and get low-risk, stable returns will add their money to the liquidity pool. This is similar to a traditional bookie’s bank account. Winnings will be paid from this liquidity pool and losses will be incurred from paying out those winnings. Odds will initially have a2% commission or “vig.” This 2% will be given to Bookies as their profit to ensure the growth of the liquidity pool in long run, as not all matches will be profitable. The DAO can later vote to adjust the vig percentage numbers.

## **Outcome**

OpenBook will use a proprietary Oracle to create and settle matches.
