# ECVRF verifier

This is a simple verifier for the ECVRF proof provided by a game.

An ECVRF generates a proof and a hash (used as the random number) from an input value using a secret private key on the game server.

The input (α) is the game's input.
The input is used to generate the hash (β) and proof (π).
The hash (β) is used as the random number for the game.
The proof (π) is used to validate that the signature is correct.

In an ECVRF, the following must be true:
```
Verify(π, α) = β
```

## Usage

### 1: Install dependencies

```bash
pnpm i
```

### 2: Add the proof

Replace the values in the `index.cjs` file with the proof provided by the game.

### 3: Run the verifier

```bash
pnpm verify
```

## License

This project is licensed under the CC0 license.
