# Sky_Forged_Token_Sale
This Solidity smart contract, SkyForgedTokenSale, facilitates a token sale where users can purchase tokens with USDC in multiple stages, each having a set price and availability of tokens.

# Main Functions:
## buyTokens:
Allows users to buy tokens using USDC. The function checks if the sale has started, is not paused, and the current stage has enough tokens available.
It transfers USDC from the buyer to the fee wallet and decreases the available token count.
If a stage runs out of tokens, the sale automatically moves to the next stage.

## pauseSale and resumeSale:
These functions allow the owner to pause or resume the sale.

## setFeeWalletAddress:
The owner can change the fee wallet address where USDC payments are sent.

## withdrawUnsoldTokens:
After the sale is completed, the owner can withdraw any unsold tokens or remaining USDC from the contract.

## claimTokens:
After the sale is over, buyers can claim their purchased tokens. The function transfers tokens from the contract to the buyer.

# Events:
## Purchase: 
Triggered whenever a token purchase is made.

## TokensClaimed: 
Triggered when a buyer claims their tokens after the sale.
