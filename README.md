# pleme-take-derive

Per-field steal: pub fn take_<field>(&mut self) -> <Type>. Returns the current value, leaves default in place (via std::mem::take; requires <Type>: Default at the call site).

[![Build](https://github.com/pleme-io/pleme-take-derive/actions/workflows/auto-release.yml/badge.svg)](#)
[![crates.io](https://img.shields.io/crates/v/pleme-take-derive.svg)](https://crates.io/crates/pleme-take-derive)

## Install

```toml
[dependencies]
pleme-take-derive = "*"
```

## Generation

This crate is mechanically emitted by [`tatara-rust-ast`](https://github.com/pleme-io/tatara-rust-ast). The author surface is a typed `(defmacro …)` Spec — the proc-macro implementation, tests, Nix flake, caixa wrapper, and CI workflow are all generated. See the catalog at `catalog.json` in the parent registry.
