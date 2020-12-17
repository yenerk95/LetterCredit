# LetterCredit

The aim of our project is to first digitalize and then to boldy innovate the letter of credit process. In order to do this, we prototyped three different implementations with increasing complexity.

## Repository Structure
The **Smart Contracts** folder contains three sub-folders. Each of them contain a Solidity prototype, which builds up on the previous one, and a .md file briefly describing  most relevant aspects and the main differences with regard to the previous prototype. 


The **General Documents** folder contains: `Log.md`, illustrating our general workflow, `General Idea.txt`, briefly describing some theoretical aspects of the ideas, `Pitfalls and Safety checks.txt`, describing some security considerations and checks we performed, as well as some aspects that can be improved.

## General rules for contract deployment

In the following image we describe the pipeline and workflow of our most basic prototype, the **Central Fintech** one. While the other prototypes add complexity, the general framework remains the same. <br/>
More detailed instructions and information are specified in each relevant folder, highlighting the differences among implementations.


![plot](https://github.com/CaterinaFabbri/LetterCredit/blob/main/Documents%20and%20Images/Basic%20Structure.jpg)


## How to use the front-end
The v1 implementation, we created a [website](https://eth-app-final.yenerk95.vercel.app/) which allows to use the contract functionalities outside of Remix, through a Metamask integration. <br/>

In order to use the website, one needs to first deploy the contract in Remix, using Injected Web3 and a Metamask Testnet. Then, the contract address shall be copypasted into the form on the initial webpage.  <br/>
The website makes use of **conditional rendering**, so each user has access to a different page. To actually visualize the page of the current metamask account, it suffices to press again the set smart contract button.  <br/>
The workflow is pretty much as in Remix. To upload a document, click on the logo and an IPFS hash will automatically be created. To actually upload the hash into the smart contract, it suffices to click `Buyer Upload` (specifying as argument only the number of days the seller will have in order to upload the documents) or `Seller Upload`.


[Here](https://github.com/yenerk95/eth-app-final) is the Github repo relative to the website
