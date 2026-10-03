# Contributing to Invasor

Thanks for wanting to help. Invasor is a small project maintained by one person, so a short conversation before a
big change saves everybody time.

## Before you start

- **Found a bug or have an idea?** Open an issue in the repository it concerns (the core is `invasor`; each
  module has its own repository). Use the template: it asks for what is usually needed.
- **Security problem?** Don't open an issue: see the [security policy](SECURITY.md).
- **Bigger change?** Open an issue first and describe what you'd like to do.

## Setting up

The core and the module repositories live side by side, as the module tools expect. The
[`invasor-workspace`](https://github.com/Gamemode-Invasor/invasor-workspace) repository clones them all with one
command (`./bootstrap.sh`).

Core (`invasor`):
```sh
python3 -m unittest discover -s backend/tests -t backend   # backend, no Steam needed
(cd frontend && npm ci && npm run typecheck && npm test)   # frontend types and value helpers
python3 tools/check_module.py modules/demo modules/_example # the module contract
```
The backend uses only Python's standard library (3.9 or newer): please don't add dependencies.

Modules: build, check, test and pack with `python3 ../invasor/tools/pack_module.py <id>`. How to write one is in
[docs/MODULES.md](https://github.com/Gamemode-Invasor/invasor/blob/main/docs/MODULES.md).

## Sending a change

1. Fork the repository and create a branch from `main`.
2. Make the change, with tests for the Python code you add or fix.
3. Run the commands above. The same checks run automatically on every pull request.
4. Open a pull request saying what it does and why.

Commit messages are short and start with the area: `Settings: every section starts folded`.

## Licensing

Invasor and its modules are under the GPL-3.0-or-later. By sending a contribution you agree that it is
distributed under that license. The module template and the code examples in the module guide are MIT.
