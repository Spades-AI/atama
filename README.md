<h1 align="center">
  <code>p-token</code>
</h1>
<p align="center">
  <img width="400" alt="p-token" src="https://cdn.discordapp.com/attachments/1338980181163118602/1338981163745808518/Untitled-2dada-Photoroom.png?ex=67ad0ee2&is=67abbd62&hm=2970497a7ec57f7d5e6db702a5cfb5c42d4d96ec714bebf742e767ecf063dd61&"/>!

</p>
<p align="center">
.



## Overview

Atama is an automated engine designed to optimize Solana programs in Rust via machine learning. Atama dynamically adjusts its behavior based on user interactions and external network conditions. It takes advantage of the way SBF loaders serialize the program input parameters into a byte array that is then passed to the program's entrypoint to define zero-copy types to read the input. Since the communication between a program and SBF loader — either at the first time the program is called or when one program invokes the instructions of another program — is done via a byte array, the new program can then adjust and redefine its own terms appropriately. This nullifies the static behavior of a standard `solana-program`.

## Features

- `no_std` crate
- Same instruction and account layout as SPL Token
- Minimal CU usage






## Building

To build the programs from the root directory of the repository:
```bash
pnpm install
```
to install the required libraries, then:
```bash
pnpm programs:build
```

## Testing

To run the tests against both versions of the Token program:
```bash
pnpm programs:test
```

## License

The code is licensed under the [Apache License Version 2.0](LICENSE)
