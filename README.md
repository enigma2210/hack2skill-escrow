
# Escrow Payment Smart Contract

This repository contains an Anchor-based Solana smart contract designed to facilitate secure and transparent escrow payments between freelancers and clients. The program ensures funds are locked until predefined conditions are met, promoting trust in transactions.

---

## Features

- **Secure Payments**: Funds are locked in escrow until both parties meet agreed-upon conditions.
- **Decentralized**: Built on Solana's blockchain, ensuring transparency and immutability.
- **Configurable**: Flexible parameters for customizing transaction terms.
- **Automated Workflows**: Releases payment upon approval from both parties or a mediator.

---

## Project Structure

- **`programs/`**: Contains the Rust source code for the escrow smart contract.
- **`tests/`**: Test scripts for verifying the escrow program's functionality.
- **`migrations/`**: Deployment and upgrade scripts for the program.
- **`target/`**: Build artifacts and compiled binaries.
- **`Anchor.toml`**: Configuration file for the Anchor framework.
- **`Cargo.toml` & `Cargo.lock`**: Rust project and dependency configuration files.
- **`package.json`**: Frontend and interfacing scripts configuration.
- **`.gitignore`**: Files and directories excluded from version control.
- **`.prettierignore`**: Files ignored by Prettier code formatting.

---

## Prerequisites

To work with this repository, ensure you have the following installed:

- **Rust**: For compiling Solana programs ([Install Rust](https://www.rust-lang.org/tools/install)).
- **Anchor Framework**: For Solana smart contract development ([Anchor Docs](https://www.anchor-lang.com/docs)).
- **Node.js & Yarn**: For frontend and testing scripts ([Download Node.js](https://nodejs.org/)).
- **Solana CLI**: For interacting with the Solana blockchain ([Install Solana CLI](https://docs.solana.com/cli/install-solana-cli-tools)).

---

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/anchor_escrow.git
   cd anchor_escrow
   ```

2. **Install Dependencies**:
   - Rust:
     ```bash
     rustup update
     ```
   - Node.js packages:
     ```bash
     yarn install
     ```

3. **Build the Program**:
   ```bash
   anchor build
   ```

4. **Deploy to Solana**:
   Update the `Anchor.toml` file with your Solana wallet and cluster configuration, then deploy the program:
   ```bash
   anchor deploy
   ```

5. **Run Tests**:
   ```bash
   anchor test
   ```

---

## Usage

1. **Initialize Escrow**:
   - Freelancer and client agree on terms.
   - Client deposits funds into the escrow account.

2. **Release Funds**:
   - Freelancer submits proof of work.
   - Client approves the release of funds.
   - If disputes arise, a mediator can intervene.

---

## Development

### Key Contracts

- **Escrow Initialization**:
  Handles the setup of the escrow account and parameters (e.g., payment amount, participants).
- **Fund Release**:
  Facilitates the release of funds upon mutual agreement or mediation.

### Testing
- All tests are located in the `tests/` directory. Use the Anchor testing framework to run simulations.

```bash
anchor test
```

---

## Contributing

1. Fork the repository.
2. Create a feature branch.
3. Commit changes and open a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

For any questions or support, contact [Your Name/Team Name] at [Your Email Address].
