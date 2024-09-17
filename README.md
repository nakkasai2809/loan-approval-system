# Loan Approval System

## Overview

This DAML project implements a comprehensive loan approval system with features for loan requests, approvals, token disbursements, and loan repayments. It also includes loan limit validation and repayment restrictions. The system is composed of several DAML templates and associated test scripts.

## Project Structure

- `daml/`
  - `Loan.daml`: Defines the `Loan` template and its operations, including token disbursement and repayment functionality.
  - `LoanApproval.daml`: Contains the `LoanRequest` template and the approval process.
  - `LoanLimit.daml`: Manages the loan limit for the bank.
  - `RepaymentRestriction.daml`: Specifies the minimum amount required for each repayment.
  - `Token.daml`: Represents tokens used for disbursement (if applicable).
  - `Main.daml`: Entry point for initializing the DAML scripts.

- `test/`
  - `LoanApprovalTest.daml`: Contains test scenarios to validate the loan request and approval workflow.
  - `LoanRepaymentTest.daml`: Contains test scenarios for loan repayment functionality and restrictions.

- `daml.yaml`: Configuration file for the DAML project.

## Setup

1. **Install DAML SDK**: Follow the instructions on the [DAML website](https://docs.daml.com/getting-started.html) to install the DAML SDK.

2. **Initialize the Project**:
   ```
   daml new loan-approval-system
   cd loan-approval-system
   ```

3. **Add DAML Files**: Replace the contents of the daml/ directory with the provided DAML files.

4. **Build the Project**:
   ```
   daml build
   ```
5. **Run the Tests**:
   ```
   daml test
   ```
