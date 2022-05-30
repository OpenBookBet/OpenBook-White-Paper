# Betting Page

![](https://lh6.googleusercontent.com/lmstC4PJvX05G2OcxyAGiqD5kWdBgh6Nd5y9QlkvPPICZsd1tJEwu\_pHJNiDb\_wVQ2qFsrppNU\_i1tlq2mTs0EFsRs37MEfPqLSig-I\_wgu4oQC3pbK9HuQYF00Ch8-3lQtea3H36zdVwHej)

Betting page is divided into multiple small pages, feature page and specific sport betting pages. When a user enters the betting page, the Market contract function _**getAllMarkets()** _ is called (represented by line ①),and the games are stored in the form of a JavaScript dictionary. The games are shown as card components, and if the data is loading, then card skeletons are displayed until the games are loaded.

Clicking on an odds button will put a game into the betslip, the bettor can manually type in the bet amount for that game and click on one of the four buttons in the bottom of the betslip to quickly set a bet amount.

Before the bet can be placed, the Bet contract function _**getLiquidityLimit(uint256\[] gameIds)**_ is called (represented by line ②), which returns the bet limit for the specified games in the betslip. If the current total bet amount is larger than the bet limit, the bet button would be disabled and the bettor can no longer place their bet.

If there are no errors detected, then a bettor can place the bet by clicking on orange Place a Bet button. The click event triggers the Bet contract function _**createBets(uint256\[] calldata gameIds, uint8\[] betIndexes, uint128\[] bet\_amounts)**_ (represented by line ③), the function returns either true or false which represents the outcome of the bet being placed. Either way, a popup is generated to inform the user about the result.
