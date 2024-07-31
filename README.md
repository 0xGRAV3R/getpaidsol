# GetPaid App
GetPaid is a Solana-based application that simplifies the process of receiving payments by utilizing secure and efficient payment links. Users can generate unique payment links, which can be shared with customers or clients to facilitate instant and transparent transactions on the Solana blockchain. The app ensures low transaction fees, fast processing times, and robust security, making it an ideal solution for businesses and individuals looking to streamline their payment processes.

By leveraging Solana's high-performance capabilities, GetPaid offers a seamless and user-friendly experience for both senders and receivers, supporting various use cases such as e-commerce, freelance services, and peer-to-peer payments.

## Getting Started

### Prerequisites

- Node v18.18.0 or higher
- Rust v1.70.0 or higher
- Anchor CLI 0.29.0 or higher
- Solana CLI 1.17.0 or higher

### Installation

#### Clone repo

```shell
git clone <repo-url>
cd <repo-name>
```

#### Install dependencies

```shell
npm install
```

#### Start the web app

```
npm run dev
```

## Apps

### Anchor

This is a Solana program written in Rust using the Anchor framework.

Note: The solana program code for the journal dapp can be found in `anchor/programs/src/lib.rs`

#### Commands

You can use any normal anchor commands. Either move to the `anchor` directory and run the `anchor` command or prefix the command with `npm run`, eg: `npm run anchor`.

#### Sync the program id:

Running this command will create a new keypair in the `anchor/target/deploy` directory and save the address to the Anchor config file and update the `declare_id!` macro in the `./src/lib.rs` file of the program.

You will manually need to update the constant in `anchor/lib/counter-exports.ts` to match the new program id.

```shell
npm run anchor keys sync
```

#### Build the program:

```shell
npm run anchor-build
```

#### Start the test validator with the program deployed:

```shell
npm run anchor-localnet
```

#### Run the tests

```shell
npm run anchor-test
```

#### Deploy to Devnet

```shell
npm run anchor deploy --provider.cluster devnet
```

### Web

This is a React app that uses the Anchor generated client to interact with the Solana program.

#### Commands

Start the web app

```shell
npm run dev
```

Build the web app

```shell
npm run build
```
