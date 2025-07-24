# Week 04 Report – SENNARIA Imane –July 21-22, 2025

## What I Did

-Complete the module: Construct and Send Your First CKB Transaction

### Generate Key Pair Execution Output  
![LGenerate Key Pair](./W04-Generate_Key_Pair.png)
### Create an Address Execution Output  
![Create an Address](./W04-Create_an_Address.png)

### Construct a transaction to send 100 CKBytes Execution Output
![Construct a transaction](./W04-Construct_a_Transaction.png)

### Sign a Transaction Execution Output
![Sign a Transaction](./W04-Sign_a_Transaction.png)

### Send a Transaction
![Send a Transaction](./W04-Sign_a_Transaction_result.png)

### Use the output that has already been spent in Input
![Use the output that has already been spent in Input](./W04-0outputAlreadySpent.png)
==> Because the transaction is trying to use an outpoint that has been already spent
### covert one cell to 3 live cells
![covert one cell to 3 live cells](./W04-1OnecellTo3livecells.png)
==> We had to include the transaction fees in our calculations
### Spend multiple outputs in Input
![Spend multiple outputs in Input](./W04-2MULpuloutputininput.png)
==>We had to group the signatures using fulfill(tx, 0, 1).
### Make the number of CKBytes in the output greater than that in the Input
![Make the number of CKBytes in the output greater than that in the Input](./W04-3oVERFLOWTRANSACTION.png)
==>Obvious error: malformed overflow transaction!
## What I Learned

I’ve learned how to create and send a basic transaction using Java.

## Challenges I Faced

- No challenges this week


