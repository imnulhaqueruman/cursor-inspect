# rg-paths.txt

Single build-machine path recovered from the Cursor-bundled `rg` binary.

Leaks the upstream `regex-automata` crate version used to compile ripgrep
(`0.4.13`) and the source file that produced one of the embedded panic
strings: `src/nfa/thompson/builder.rs`.

This is the only `runner/.cargo` path present in the ripgrep binary
compared to the dozens seen in the `crepectl` dump, which is consistent
with ripgrep being built with fewer custom / patched crates.

## Raw content

```text
/Users/runner/.cargo/registry/src/index.crates.io-1949cf8c6b5b557f/regex-automata-0.4.13/src/nfa/thompson/builder.rs
```
