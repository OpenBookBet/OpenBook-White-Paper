# Making a Bet

At a high level, OpenBook has two essential operations that are undertaken by its users: making a bet and becoming a bookie by providing liquidity. These two actions serve as the lifeblood of the OpenBook protocol. This section contains the discussion of the first of these two functions, making a bet. The other, becoming a bookie, will be covered in the mirror section 8.1. Here’s the simple five step process for placing a bet with OpenBook:

![](https://lh5.googleusercontent.com/IF0HWR5D\_xYP4kAVjYOXMX3aa3873jS6Q6MHaKPn5Pl5NFF5RyZIk59hf-qVzS9aPRf6F8-WjAeZ7PyYBljmgmgEMNX2dgPj5csSDw564jilH\_KahHHJslsem-jc1mwuvtN8noKUbIBH36qI)

## Step 1: Login to MetaMask

To utilize the services OpenBook provides, one needs to connect their MetaMask wallet to the site. By following this route over a traditional login approach, all Bettors and Bookies can remain anonymous to OpenBook. The only identification factor is the public wallet address one uses to make bets or provide liquidity.

## Step 2: Bet Selection

Once logged into MetaMask and connected to OpenBook, the Bettor must choose the bet or bets they’d like to make. For now, we offer only money line bets on all of our matches. The types of betting and their role in OpenBook are addressed in more detail in the following section. Choosing a bet and adding it to the Bettor’s bet slip is as easy as clicking on the box inside the correct match corresponding to the chosen side of the moneyline. Bets inside the bet slip have individual wager amount boxes to be filled out.

## Step 3: Place Bet(s)

As soon as the Bettor has filled their bet slip to satisfaction, placing a bet is a simple as clicking the “Place Bets” button. The bet or bets will need to be confirmed in the MetaMask pop ups, then an on-screen receipt will appear with the details of the transaction for the Bettor. As soon as the blockchain processes the transaction–blocktime on the Polygon network is roughly every 2 seconds, meaning this wait will hardly be noticeable under the worst conditions –the Bettor is sent their bet slip as an ERC-1155 token.

## Step 4: Wait and/or Watch the Game

Very little explanation is needed for this part; after confirming the transaction, the blockchain and our Providers take care of everything else on the back end. Until the outcome of the match is settled and confirmed by the Providers, all the Bettor needs to do is hope they won.

## Step 5: Collect Winnings

After the Providers have settled the final outcome of a match, that information is shared with OpenBook. When the Bettor checks to see if they’ve won, our interface will refer to the Bettor’s wallet for bet slips and determine by slip ID# and metadata if each slip has won. If there are any unclaimed winnings on any bet slips in the Bettor’s wallet, there will be a button on the page to claim all winnings. After confirming to claim winnings, the ERC-1155 token receipt for all winning bet slips are checked for validity and then systematically burnt. After validation, the original bet amount and winnings are disbursed to the Bettor’s wallet, completing the process.

