# Week 07 Report – offCKB Project  
**Name:** SENNARIA Imane
**Period:** August 24–28, 2025  


## What I Did
### Running the Devnet Environment
Successfully launched the offCKB devnet environment.

![Running Devnet](./W07-Running%20DEVNet.png)

Faced multiple build errors related to missing targets and crates.

-  `can't find crate for 'core'`  
-  `could not compile 'cfg-if'`  
-  Problem was resolved after installing missing Rust target and adjusting environment.

![Build Error – Missing Crate](./W07-PRBCantFindCrat.png)  
![Build Error – Client Issue](./W07-PRBCantFindClient.png)  
![Build Success](./W07-ProblemResolved.png)


###  Transfer & Deposit Commands

Successfully :
- Transfer CKB tokens between accounts
- Check balances before and after
- Deposit into devnet accounts

![Transfer Command](./W07-transfercommande.png)  
![Deposit Command](./W07-deposit.png)  
![Check Balance](./W07-balancecomande.png)



### Listing Accounts 

Listed available test accounts using `offckb accounts`.

![offCKB Accounts](./W07-offckbaccounts.png)



### Checked Devnet Configuration

Ran `offckb config list` to inspect RPC URLs, paths, and environment settings.

![Devnet Config](./W07-devlist.png)



## What I Learned

- How to troubleshoot make build issues (`core` crate missing, target not installed)
- How to run and interact with offCKB devnet
- Using the commandes for transfers, balance checks, and deposits
- Exploring the default test accounts and configuration settings



##  Challenges I Faced

### Build Errors
- Encountered issues related to the `riscv64` target not being installed.
- Had to run:  
  ```bash
  rustup target add riscv64imac-unknown-none-elf
