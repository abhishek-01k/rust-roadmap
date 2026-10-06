# Rust From Zero Roadmap

A 12-week, six-phase roadmap for learning Rust, using only the resources worth your time. Almost everything is free and official.

- **Time:** ~12 weeks at 1–2 hrs/day
- **Assumes:** you can already code in one other language
- **Cost:** ₹0 for everything core

The full checklist with tasks and milestones is in [Rust From Zero Roadmap.md](./Rust%20From%20Zero%20Roadmap.md).

## Phases

| Phase | When | Focus | Milestone |
|---|---|---|---|
| 0 | Day 1 | Toolchain: rustup, rust-analyzer, cargo | `cargo new hello && cargo run` |
| 1 | Weeks 1–2 | Foundations, ownership and borrowing | Guessing game with score + replay |
| 2 | Weeks 3–4 | Modules, errors, generics, traits, lifetimes, tests | `minigrep` with a `--count` flag |
| 3 | Weeks 5–6 | Closures, iterators, smart pointers, threads | Multi-threaded word counter |
| 4 | Weeks 7–8 | Async with Tokio and core crates | Concurrent URL checker CLI |
| 5 | Weeks 9–12 | Pick one track and ship a project | A real project on GitHub |
| 6 | Ongoing | Go deeper | A "good first issue" fix in a crate you use |

## Key resources

**Start here**
- [The Rust Book, interactive edition](https://rust-book.cs.brown.edu/) (or the [official book](https://doc.rust-lang.org/book/))
- [Rustlings](https://rustlings.rust-lang.org/): small exercises to do alongside the book
- [Rust Playground](https://play.rust-lang.org/)

**Practice**
- [Rust by Example](https://doc.rust-lang.org/rust-by-example/)
- [100 Exercises to Learn Rust](https://rust-exercises.com/100-exercises/)
- [Exercism Rust track](https://exercism.org/tracks/rust)
- [Standard library docs](https://doc.rust-lang.org/std/)

**Async and ecosystem**
- [Tokio tutorial](https://tokio.rs/tokio/tutorial)
- [Async Book](https://rust-lang.github.io/async-book/)
- [docs.rs](https://docs.rs/) and [crates.io](https://crates.io/)

**Tracks (pick one)**
- Web backend: [axum](https://docs.rs/axum/latest/axum/), [Zero To Production](https://www.zero2prod.com/) (paid)
- CLI tools: [Command Line Applications in Rust](https://rust-cli.github.io/book/index.html)
- Embedded: [The Embedded Rust Book](https://doc.rust-lang.org/embedded-book)
- Python interop: [Rust-Python Interoperability (PyO3)](https://rust-exercises.com/rust-python-interop/)

**Go deeper**
- [Rust for Rustaceans](https://nostarch.com/rust-rustaceans) (paid)
- [The Rustonomicon](https://doc.rust-lang.org/nomicon/index.html)
- [The Rust Reference](https://doc.rust-lang.org/reference/index.html)
- [Rust Users Forum](https://users.rust-lang.org/)

**Short on time?** Experienced developers can swap Phases 1–3 for Google's [Comprehensive Rust](https://google.github.io/comprehensive-rust/), then jump to Phase 4.

## Tip

When the borrow checker complains, read the whole error, then run `rustc --explain <code>` (for example, `rustc --explain E0382`). Clone freely while learning and optimize later.

---

Put together by **Abhishek** · [abhish3k.xyz](https://abhish3k.xyz)
