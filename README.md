# Cora 🦀

[![License](https://img.shields.io/badge/License-GPL--3.0-blue)](https://www.gnu.org/licenses/gpl-3.0.html)
[![Made with](https://img.shields.io/badge/Made%20with-Rust-orange)](https://rust-lang.org)
[![Built for](https://img.shields.io/badge/Built%20for-Arch%20Based%20Distros-cyan)](https://archlinux.org)

Cora is a terminal tool for Arch-based distros that replaces complex pacman commands with simple human-readable ones. Instead of `sudo pacman -S pkg` you just type `cora install pkg`. Includes package management, mirror updates, system maintenance and more — built to make the terminal accessible for Linux beginners.

---

## Installation

### IF YOU DONT HAVE GIT MAKE SURE TO INSTALL IT HERES THE COMMAND

```bash
sudo pacman -S git
sudo pacman -Syu
```

### One line install

```bash
curl -s https://raw.githubusercontent.com/fusiontech21/Cora/main/install.sh | bash
```

### Manual install

```bash
git clone https://github.com/fusiontech21/Cora
cd Cora
cargo build --release
sudo cp target/release/cora /usr/local/bin/
```

### Requirements

- Rust + Cargo
- An Arch-based distro (Arch, CachyOS, Manjaro, EndeavourOS, etc.)

---

## Showcase

![showcase 1](imgs/Showcase1.png)
![showcase 2](imgs/Showcase2.png)
![showcase 3](imgs/Showcase3.png)

---

## Commands

| Command                 | What it does                                        |
| ----------------------- | --------------------------------------------------- |
| `cora install <pkg>`    | Install a package                                   |
| `cora remove <pkg>`     | Remove a package and its configs + orphaned deps    |
| `cora softremove <pkg>` | Remove just the package                             |
| `cora search <pkg>`     | Search for a package                                |
| `cora update`           | Update the entire system                            |
| `cora upgrade <pkg>`    | Upgrade a specific package                          |
| `cora downgrade <pkg>`  | Downgrade a package to an older cached version      |
| `cora info <pkg>`       | Show info about a package                           |
| `cora installed <pkg>`  | Check if a package is installed                     |
| `cora list`             | List packages you explicitly installed              |
| `cora listall`          | List every installed package including dependencies |
| `cora files <pkg>`      | Show all files owned by a package                   |
| `cora owner <file>`     | Show which package owns a file                      |
| `cora deps <pkg>`       | Show dependencies of a package                      |
| `cora stats`            | Show how many packages you have installed           |
| `cora log`              | Show pacman install history                         |
| `cora mirrors`          | List your mirrorlist with reflector                 |
| `cora unlock`           | Remove pacman lock file when pacman gets stuck      |
| `cora details`          | Show info about cora                                |

---

## License

This project is licensed under the **GPL-3.0** license. See [LICENSE](LICENSE) for details.

---

© 2026 fusiontech21 — All rights reserved
