# Week 08 Report – SENNARIA IMANE – November 03–09, 2025

## What I Did

- Until now, we had only modified the TypeScript files. This week, for the first time, we directly modified `entry.rs` and `test.rs`.
- Installed Capsule and set up the development environment.
- Created a new smart contract project using Capsule.
- Implemented the contract by editing the following Rust source files:
  - `entry.rs`
  - `main.rs`
  - `lib.rs`
  - `tests/` (test files)

## What I Learned

- Gained a clearer understanding of the role of each Rust file (`entry.rs`, `main.rs`, `lib.rs`) in structuring a smart contract.
- Learned how to run and interpret test results in Rust using Capsule.

## Challenges I Faced

-  **Error 1:** Forgot to rename the project name in one of the files, which caused build issues. 
![Error1](./w8-Error1.png)
-  **Error 2:** Faced a compatibility issue due to an outdated Cargo version.  
![Error2](./w8-Error2.png)
  **Solution:** Resolved it by copying the correct configuration from an older, working project.


## Important Files

- [`entry.rs`](./entry.rs)
- `[`test.rs`](./tests.rs)

## Results
![TestResults](./w8-TestRunning.png)

## Goals for Next Week

- Learn the basics of JavaScript, as it's important for smart contract interactions and tooling in the suite.
-  Build and test a new contract and a contract off-chain (Off-CKB).
-  Start working on a more complex contract .
