# Clonk CLI

A command-line interface for interacting with the Clonk API.

## Installation

clone the repository and run `cargo install --path .` to install the CLI.

## Usage

### Login

```bash
clonk auth login
```

This will prompt you for your username and password, and then save the authentication cookies to a file in your home directory.

### Redeem

```bash
clonk redeem <api_name> [--input "input"]
```

This will redeem the specified API with the given input (if required).

### Repeating redeem

If (for some reason) you need to send some message repeatedly, you can use special parameters `--period` and `--count`:
```bash
clonk redeem <api_name> --period <ms> --count <n> [--input "input"]
```
