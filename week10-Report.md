# Week 10 Report – SENNARIA IMANE  
**November 17 – December 1, 2025**

##  What I Did

### 1. Built my JavaScript smart contract (`testCCC`)
I successfully bundled and compiled my TypeScript/JavaScript contract using **esbuild**, generating the `.bc` bytecode file.

![Build](./Week10-buildContract.png)

---

### 2. Installed and configured all required CKB tools
The installation of **ckb-debugger** was challenging due to missing dependencies (`protoc`) and PATH issues. Multiple errors occurred before the installation succeeded.

![Error1](./Week10-Error1CkbDebugger.png)  
![Error2](./Week10-Error2CkbDebugger.png)  
![Error3](./Week10-Error3CkbDebugger.png)  
![Error4](./Week10-Error4CkbDebugger.png)  
![Error5](./Week10-Error5CkbDebugger.png)

---

### 3. Attempted to run tests on Devnet – Failed
Running tests on Devnet caused this error because **ckb-js-vm is NOT deployed on Devnet**.

![Devnet Error](./Week10-ckbjsvmNot%20Deployed%20in%20devnet.png)

---

### 4. Successfully deployed the contract on Testnet
Since ckb JS VM  is not deployed in Devnet, I deployed the smart contract on **Testnet** instead.

**Command used:**

offckb deploy --network testnet --target dist/testCCC.bc
### 5. Executed tests on Testnet

The test successfully sent a transaction: 

TX Hash: 0x3b7720df175b7b2b21336041a7659d23cd0d5f781d9f2d9b483a6e84ef93704e

![Testnet Data](./Week10-DeployContract.png)

![Testnet testPass](./Week10-testnet-pass.png)
### 6. Transaction detail on CKB explorer
-  Data section

The data stored in the output cell 0:

0x6d79

![Testnet Data](./Week10-TestNetExplorer.png)
-  Type Script section 

Displays:
![Testnet Data](./Week10-TestNetExplorerTypeScript.png)



## Challenges I Faced

    - Missing protoc

    - SSL timeout during installation

    - ckb-debugger: command not found

    -The ckb-js-vm is not deployed on Devnet. We could have used Devnet we only needed to retrieve the binary file ckbfile.bc, but since the contract is already deployed on Testnet, we proceeded to deploy our construct directly on Testnet.

    - Some dependencies required Node 20+




## Results

    - Contract built successfully
    - Successful deployment on Testnet
    - Testnet transaction sent successfully
    - transaction detail visible on explorer
    - Identified async test issues

## Goals for Next Week
-Build a more advanced test scenario
-Begin developing a more complex JavaScript smart contract


