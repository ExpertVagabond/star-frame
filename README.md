<div align="center">

# star_frame

**High-performance, trait-based Solana program framework**

[![Crates.io](https://img.shields.io/crates/v/star_frame?logo=rust)](https://crates.io/crates/star_frame)
[![docs.rs](https://img.shields.io/docsrs/star_frame?logo=docsdotrs)](https://docs.rs/star_frame)
[![Solana](https://img.shields.io/badge/Solana-14F195?logo=solana&logoColor=white)](https://solana.com)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)

*Revived fork of [staratlasmeta/star_frame](https://github.com/staratlasmeta/star_frame) for the Solana Graveyard Hackathon*

</div>

---

## Overview

Star Frame is a modern Solana program framework designed to make developing on-chain programs more ergonomic, safe, and performant. Built with a trait-based architecture, it provides compile-time validation, optimized compute unit usage via Pinocchio, and a modular design where everything is a trait or type.

> **Status: REVIVED** -- Framework compiles against Solana Rust 1.84.1, examples build and deploy.

## Key Advantages

- **Performance** -- optimized for Solana compute unit constraints using Pinocchio
- **Type Safety** -- comprehensive compile-time validation with traits all the way down
- **Modularity** -- everything is a trait or type; use only what you need
- **Developer Experience** -- intuitive APIs with derive macros for common patterns

## Quick Start

```bash
cargo install star_frame_cli
sf new my-program
```

## Framework Features

| Feature | Description |
|---------|-------------|
| `#[derive(StarFrameProgram)]` | Program entrypoint and instruction dispatch |
| `#[derive(InstructionSet)]` | Type-safe instruction enum |
| `#[derive(AccountSet)]` | Account validation with compile-time checks |
| `#[derive(ProgramAccount)]` | Zero-copy account data with bytemuck |
| `#[star_frame_instruction]` | Instruction handler with automatic deserialization |

## Resources

- [API Documentation](https://docs.rs/star_frame)
- [Example Programs](example_programs/)
- [Compute Unit Benchmarks](example_programs/bench/COMPUTE_UNITS.md) (vs Anchor)

## Original Project

Maintained fork of [staratlasmeta/star_frame](https://github.com/staratlasmeta/star_frame) by ATMTA, Inc.

## License

[Apache License 2.0](LICENSE)
