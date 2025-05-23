# <div align="center">Aurora</div>

### <div align="center">Supercharge your terminal and Wayland experience with Aurora framework!</div>
<div align="center">
  <img alt="Static Badge" src="https://img.shields.io/badge/BASH-000000?style=for-the-badge&logo=gnubash&logoColor=000000&labelColor=ccddff">
  <img alt="Static Badge" src="https://img.shields.io/badge/MIT-000000?style=for-the-badge&logo=opensourceinitiative&logoColor=000000&labelColor=ccddff">
  <img alt="Static Badge" src="https://img.shields.io/badge/WAYLAND-000000?style=for-the-badge&logo=wayland&logoColor=000000&labelColor=ccddff">
  <img alt="Static Badge" src="https://img.shields.io/badge/TMUX-000000?style=for-the-badge&logo=tmux&logoColor=000000&labelColor=ccddff">
</div><br>

Meet Aurora – your new `.bashrc`, reimagined! It's a powerful, multi-functional utility built to supercharge your command-line environment. Automated compositor launching, intelligent terminal session management, and effortless customization, all within a lightweight, cross-platform package designed for power users and tinkerers alike.

### Key Features:
- **Smart Defaults**: Start with a rock-solid `.bashrc` foundation, including essential `PATH` settings and smart defaults.
- **Wayland Launching**: Log in via TTY, and Aurora instantly finds your installed [Wayland compositors](https://github.com/hlasitahudbabezzvuku/aurora?tab=readme-ov-file#supported-composiitors), letting you pick and launch your graphical session with a single keypress.
- **Tmux Integration**: Never lose your place again! Aurora intelligently manages `tmux` sessions within your graphical environment. It automatically reconnects you to existing sessions or creates fresh ones, bringing incredible persistence and powerful features (tabs, splits!) even to terminals that lack them natively.
- **Services**: A mechanism to launch and manage simple background tasks (like battery monitors) alongside your compositor session.
- **Customization**: Easily extend and customize your Bash environment! Simply drop your configuration `.sh` files into `~/.config/bash/`. Aurora automatically sources them in alphabetical order (use `10_`, `50_` prefixes), making customization clean and manageable.
- **Automatic Updates**: Enable automatic updates (requires `curl`) and always have the latest Aurora features and improvements delivered straight to your system, effortlessly.

### Get Started in Seconds:
1.  **Download**: Grab the [bashrc](https://github.com/hlasitahudbabezzvuku/aurora/blob/development/bashrc) file or clone the repository.
2.  **Backup**: Protect your current setup: `cp ~/.bashrc ~/.bashrc.bak`
3.  **Install**: Replace your `~/.bashrc` with `bashrc` for the complete experience.
4.  **Customize (Optional)**: Create `~/.config/bash/` and populate it with your personal scripts (e.g., `~/.config/bash/50_aliases.sh`, `~/.config/bash/90_exports.sh`).
5.  **Activate**: Launch a new tty and log in.

### Platform Support & Dependencies:
- **Minimal Dependencies**:
  - **Core Dependencies**:
    - `bash`
    - `kill`
    - `time`
    - `tty`
    - `tput`
  - **Optional Dependencies**:
    - `tmux`: Required for the Tmux Sessioning feature.
    - `notify-send`: Often used by background services for notifications.
    - `curl`: Required for the Automatic Updates feature.
- **OS Compatibility**: Designed from the ground up to be distribution and init-system agnostic. Runs beautifully on Linux, macOS, FreeBSD/OpenBSD, and Solaris.

### Supported Compositors:
| Compositor | Command |
| -------- | ------- |
| Cage | $ cage |
| DWL | $ dwl |
| Steamdeck Mode | $ gamescope -e -- steam -tenfoot |
| Hyprland | $ Hyprland |
| Plasma | $ startplasma-wayland |
| LabWC | $ labwc |
| Miracle | $ miracle-wm |
| niri | $ niri --session |
| Qtile | $ qtile start -b wayland |
| River | $ river |
| Sway | $ sway --unsupported-gpu |
| SwayFX | $ swayfx --unsupported-gpu |
| Wayfire | $ wayfire |
| Weston | $ weston |

### Join the Community:
- **Contribute**: Got ideas or code improvements? Open an [pull request](https://github.com/hlasitahudbabezzvuku/aurora/pulls).
- **Report Bugs**: Found a bug? Open an [issue](https://github.com/hlasitahudbabezzvuku/aurora/issues).

### License:
Aurora is released under the MIT licence. Check the [LICENSE](https://github.com/hlasitahudbabezzvuku/aurora/blob/development/LICENSE) file for the full details.
