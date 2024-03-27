# State Machine Contract

## Description

The State Machine contract is designed to manage the lifecycle of a loan, transitioning between different states such as PENDING, ACTIVE, and CLOSED. Key functionalities include:

1. Funding the loan: Lenders can fund the loan amount.
2. Reimbursing the loan: Borrowers can reimburse the loan amount along with interest.
3. Transitioning between states: The contract automatically transitions between states based on predefined conditions.

## Contract Details

- **Solidity Version:** ^0.8.0
- **States:**
  - PENDING: Initial state before the loan is funded.
  - ACTIVE: State when the loan is funded and active.
  - CLOSED: State when the loan is reimbursed and closed.
- **Variables:**
  - `amount`: Loan amount.
  - `interest`: Interest amount.
  - `end`: Timestamp indicating the end of the loan duration.
  - `duration`: Duration of the loan.
  - `borrower`: Address of the borrower.
  - `lender`: Address of the lender.

## Usage

### Lender Functions

- **Fund Loan:** Lenders can fund the loan amount, transitioning it to the ACTIVE state.

### Borrower Functions

- **Reimburse Loan:** Borrowers can reimburse the loan amount along with interest, transitioning it to the CLOSED state.

## Smart Contract Integration

To integrate the State Machine contract into your DApp, follow these steps:

1. Deploy the State Machine contract on the Ethereum blockchain.
2. Connect your frontend application to the deployed contract using Web3.js or similar libraries.
3. Implement user interfaces for lenders to fund the loan and for borrowers to reimburse the loan.
4. Monitor contract events and states to keep users informed about the loan status.

## Sample Application

The provided `App.js` file demonstrates a React-based frontend application that interacts with the State Machine contract. It includes functionalities for lenders to fund the loan and for borrowers to reimburse the loan. The application dynamically updates the loan state and relevant information.

For more details on contract methods and events, refer to the contract's ABI (Application Binary Interface) and the Web3 documentation.

## License

This Solidity contract is licensed under the [MIT License](https://opensource.org/licenses/MIT).



