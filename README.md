# keskos-mirrorlist

`keskos-mirrorlist` packages the pacman mirror configuration for the KeskOS package repository.

## What this is

This repository builds the package that installs the curated mirror list consumed by the `[keskos]` pacman repo configuration.

## Role in KeskOS

Mirrorlist package.

## Package name

```txt
Package: keskos-mirrorlist
Repo: [keskos]
Architecture: any
```

## What it installs or provides

- Installs `/etc/pacman.d/keskos-mirrorlist`.
- Does not ship commands, services, or GUI launchers.

## Commands and launchers

- This package does not install standalone commands.

## Config, logs, and state

- `/etc/pacman.d/keskos-mirrorlist` is the primary file managed by the package.
- No logs or systemd units are created by the package.

## Dependencies

- No runtime dependencies are declared.
- Build with `makepkg -s --noconfirm`.

## Build

```bash
makepkg -s --noconfirm
```

## Packaging notes

- Keep mirror URLs and ordering here rather than scattering them across installer/app repos.
- The package name should remain stable so other repos can depend on it.

## Troubleshooting

- If pacman cannot reach the KeskOS repo, inspect `/etc/pacman.d/keskos-mirrorlist` and the matching repo include lines in pacman configuration.

## Docs website export notes

- Docs site usage: repo setup and mirror-configuration reference.
