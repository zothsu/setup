# Dotfiles & Setup Scripts

## Key Features

- Custom aliases and shell enhancements to boost terminal productivity
- Hardened Linux server setup routines (SSH, firewall, Fail2Ban)
- Docker- and VPN-friendly CLI configuration
- Modular structure for internal notes and machine-specific config
- Obsidian-flavored markdown in `.notes/` for documentation

## Technologies Used

- Linux (Ubuntu 24.04)
- Bash
- SSH
- Fail2Ban
- UFW
- Docker
- Git

## Directory Structure

```
.dotfiles/
├── .bash_aliases       # Aliases for quick command use
├── .notes/             # Personal markdown notes
└── gitignore.sh
```

## Setup Instructions

1. Clone the repository into your home directory:
   ```bash
   git clone git@github.com:***REMOVED***/dotfiles.git ~/.dotfiles
   ```

2. Symlink key files:
   ```bash
   ln -sf ~/.dotfiles/.bash_aliases ~/.bash_aliases
   ln -sf ~/.dotfiles/.bashrc ~/.bashrc
   source ~/.bashrc
   ```

3. Run the setup script (optional):
   ```bash
   ~/.dotfiles/setup.sh
   ```

## To-Do and Future Improvements

- [ ] Add SSH hardening script for `/etc/ssh/sshd_config`
- [ ] Create modular install scripts for workstation vs server environments
- [ ] Automate dotfiles deployment with GitHub and SSH key setup
- [ ] Move private keys and credentials to a `.secrets/` folder (excluded from Git)
- [ ] Add `.vimrc`, `.inputrc`, and completions for Docker, Git, and SSH

---

These dotfiles are designed for personal use on trusted systems. Sensitive content is either redacted or stored securely outside of version control.


