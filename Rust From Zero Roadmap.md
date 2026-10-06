You commented "rust" · here's what I promised

# Rust from zero, the exact roadmap

Twelve weeks, six phases, only the resources worth your time. Most of it is free and official. Tick things off as you go; your progress stays saved in this browser.

**\~12 weeks** at 1–2 hrs/day **Assumes** you can code in one other language **Cost** ₹0 for everything core

0 / 0 done

**Already a working developer and short on time?** Swap Phases 1–3 for [Comprehensive Rust](https://google.github.io/comprehensive-rust/), the free course Google's Android team uses internally. Its first four days cover the fundamentals, then jump to Phase 4.

0Day 1

## Set up your toolchain

Get Rust installed properly and learn the four cargo commands you'll type every day.

### Do this

- [ ] Install Rust with [rustup](https://www.rust-lang.org/tools/install), the official installer. Avoid your OS package manager.
- [ ] Install VS Code with the **rust-analyzer** extension (inline types and errors as you type).
- [ ] Create a project and run it: `cargo new hello`, then `cargo run`.
- [ ] Learn the daily four: `cargo check` (fast compile check), `cargo run`, `cargo fmt`, `cargo clippy` (linter that teaches idioms).
- [ ] Bookmark the [Rust Playground](https://play.rust-lang.org/) for trying snippets without a project.

### Keep updated

`rustup update`

1Weeks 1–2

## Foundations and ownership

Syntax, types, structs, enums, and the one idea that makes Rust different: ownership and borrowing. Read and practise side by side, every day.

### Do this

- [ ] Read the Rust Book through the chapters on common concepts, ownership, structs, enums and `match`.
- [ ] Spend extra time on the ownership chapter. Read it twice if needed. Everything later depends on it.
- [ ] Start Rustlings and solve the exercises matching each chapter you finish.

### Resources

- [The Rust Book, interactive edition](https://rust-book.cs.brown.edu/)Free

  Brown University's version of the official book, with quizzes and visual diagrams of ownership. Start here over the plain version.
- [The Rust Programming Language ("the book")](https://doc.rust-lang.org/book/)Free

  The official original. Also available offline with `rustup doc --book`.
- [Rustlings](https://rustlings.rust-lang.org/)Free

  Official small exercises you fix in your own editor until they compile and pass. Built to run alongside the book.

### Install Rustlings

`cargo install rustlings`

`rustlings init && cd rustlings && rustlings`

**Milestone**Build the guessing game from Chapter 2 without looking, then add a score counter and a "play again" prompt.

2Weeks 3–4

## The core language

Modules, collections, error handling with `Result` and `?`, generics, traits, lifetimes and tests. This is where Rust starts to feel productive.

### Do this

- [ ] Continue the book: packages and modules, common collections, error handling.
- [ ] Generics, traits and lifetimes. Don't aim to master lifetimes yet; aim to read them.
- [ ] Writing automated tests with `#[test]` and `cargo test`.
- [ ] Keep Rustlings in sync with each chapter.
- [ ] When a concept doesn't click, look it up in Rust by Example for a code-first explanation.

### Resources

- [Rust by Example](https://doc.rust-lang.org/rust-by-example/)Free

  Official. Short runnable examples for every concept, light on prose. Great as a lookup next to the book.
- [Standard library docs](https://doc.rust-lang.org/std/)Free

  Get comfortable reading these early. `Vec`, `HashMap`, `String`, `Option` and `Result` pages are worth a full read.

**Milestone**Build `minigrep`, the command-line search tool from the book's I/O project chapter. Then add a `--count` flag on your own.

3Weeks 5–6

## Write idiomatic Rust

Closures, iterators, smart pointers (`Box`, `Rc`, `RefCell`) and threads. Then lots of reps with feedback so your code starts looking like real Rust.

### Do this

- [ ] Finish the book's chapters on iterators and closures, Cargo and crates.io, smart pointers, and fearless concurrency.
- [ ] Work through 100 Exercises to Learn Rust. It ties every concept to a single growing project.
- [ ] Solve at least 20 Exercism problems and request mentor feedback on a few.
- [ ] Run `cargo clippy` on everything and fix every warning. It's free code review.

### Resources

- [100 Exercises to Learn Rust](https://rust-exercises.com/100-exercises/)Free

  By Mainmatter, a Rust consultancy. Theory plus about 100 hands-on exercises, from syntax to the standard library and ecosystem.
- [Exercism Rust track](https://exercism.org/tracks/rust)Free

  99 exercises with automated analysis and free human mentoring from volunteers who show you the idiomatic way.

**Milestone**A multi-threaded word counter: read a folder of text files in parallel threads and print the top 10 words. Use channels or `Arc<Mutex<_>>`.

4Weeks 7–8

## Async and the ecosystem

Real-world Rust runs on a handful of crates. Learn async with Tokio and the libraries nearly every project uses.

### Do this

- [ ] Complete the official Tokio tutorial end to end.
- [ ] Read part one of the Async Book for the concepts behind `async`/`.await`.
- [ ] Get familiar with the essentials: `serde` (JSON), `clap` (CLI args), `reqwest` (HTTP client), `anyhow`/`thiserror` (errors), `tracing` (logs).
- [ ] Look up any crate's docs on [docs.rs](https://docs.rs/) and find new ones on [crates.io](https://crates.io/).

### Resources

- [Tokio tutorial](https://tokio.rs/tokio/tutorial)Free

  Official guide to the most widely used async runtime: spawning tasks, shared state, channels, I/O, framing and `select!`.
- [Asynchronous Programming in Rust](https://rust-lang.github.io/async-book/)Free

  The official async book. It's currently being rewritten, so treat it as a concept reference and lean on Tokio for practice.

**Milestone**An async CLI that takes a list of URLs, fetches them all concurrently, and prints status code and response time for each.

5Weeks 9–12

## Pick a track and ship something

Tutorials stop teaching you around here. Choose one direction, build one real project in it, and put it on GitHub.

#### Web backend

APIs and services with axum, built by the Tokio team.

- [axum docs](https://docs.rs/axum/latest/axum/) + its examples folder
- [Zero To Production in Rust](https://www.zero2prod.com/) Paid. Free sample; the author offers help to students who can't afford it.

#### CLI tools

The easiest place to ship something people actually use.

- [Command Line Applications in Rust](https://rust-cli.github.io/book/index.html)
- Build: a todo CLI, a file renamer, or your own `ls`

#### Systems & embedded

Microcontrollers, bare metal and low-level code.

- [The Embedded Rust Book](https://doc.rust-lang.org/embedded-book)
- [Comprehensive Rust: Bare-metal day](https://google.github.io/comprehensive-rust/bare-metal.html)

#### Speed up Python

Write Rust extensions for Python code that's too slow.

- [Rust-Python Interoperability](https://rust-exercises.com/rust-python-interop/) (PyO3), free

- [ ] Pick one track. Only one.
- [ ] Build and publish one project on GitHub with a README, tests, and clean `clippy` output.
- [ ] Bonus: build the multithreaded web server from the book's final chapter.

6Ongoing

## Go deeper

For when you're comfortable and want to write Rust at a professional level.

- [Rust for Rustaceans](https://nostarch.com/rust-rustaceans)Paid

  By Jon Gjengset. The standard "what to read after the book": API design, unsafe, async internals, macros, no_std.
- [The Rustonomicon](https://doc.rust-lang.org/nomicon/index.html)Free

  Official guide to unsafe Rust and how the language works underneath.
- [The Rust Reference](https://doc.rust-lang.org/reference/index.html)Free

  More detailed than the book. Use it to settle "how exactly does this work" questions.
- [Rust Users Forum](https://users.rust-lang.org/)Free

  Where to ask when you're stuck. The community is genuinely friendly to beginners.

- [ ] Find a crate you use and fix a "good first issue" on its GitHub.

!Read this

## The compiler is your teacher

Every beginner fights the borrow checker. These are the errors you'll see most. Run `rustc --explain` with the code for a full explanation with examples, or check the [Compiler Error Index](https://doc.rust-lang.org/error-index.html).

`E0382`Using a value after it was moved. Borrow it with `&`, or `.clone()` it for now.

`E0502`Borrowing something as mutable while it's also borrowed as immutable. Shorten one borrow's scope.

`E0499`Two mutable borrows at once. Only one `&mut` may exist at a time.

`E0106`Missing lifetime specifier. Often a sign you should return an owned `String` instead of `&str`.

`rustc --explain E0382`

**Rule of thumb**Read the whole error message, top to bottom, before changing code. Clone freely while learning; optimize later.

Put together by **Abhishek** · abhish3k.xyz. Every link checked against its official source in October 2026. Stuck somewhere? Reply to the video and tell me which phase you're on.