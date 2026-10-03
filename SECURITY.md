# Security policy

## Reporting a vulnerability

Please **don't open a public issue** for a security problem. Use GitHub's private reporting instead: open the
repository's **Security** tab and choose **Report a vulnerability**. Only the maintainers can see it.

Include what you found, how to reproduce it and which version (Invasor and, if it applies, the module) you used.
Invasor is maintained by one person in their free time: you'll get an answer as soon as possible, but not
necessarily the same day.

## What is covered

- **Invasor (the core)**: the service, the panel, the installer and the update mechanism.
- **The modules** in this organization: Artwork, Deckico, Patito, Pescao, GE-RR and Noty.
- **The release packages** published in each repository's Releases.

Only the **latest release** of each project is supported with fixes.

## Things worth knowing

- **A module is trusted code.** Its backend runs as your user and its UI runs inside Steam's window. Install only
  modules from people you trust. Invasor checks that a module zip is well formed; that doesn't make it safe.
- **Invasor never needs root.** It runs as a user service. A report that depends on running it as root is a
  different kind of problem.
- **Updates verify integrity, not authorship.** The core checks the SHA-256 published next to each release
  package. That catches a corrupt download; it doesn't protect against a compromised GitHub account.

## Not our vulnerabilities

Problems in the projects the modules work with (Steam, SteamGridDB, lsfg-vk, MAKO Renderer, GE-Proton…) belong to
those projects. Please don't report them to those projects as Invasor's.
