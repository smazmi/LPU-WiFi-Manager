# 🛜 LPU WiFi Manager

<br>
<p align="center">
<img src="./assets/llogin.png" alt="Logo" width="300">
</p>
<br>
This is a command-line tool for managing LPU WiFi connections, written in Rust. It's a rewrite of the original Bash script by 
<a href="https://github.com/Ba3a-G">Ba3a-G</a>. You can find the original repository <a href="https://github.com/Ba3a-G/LPU-Wireless-Autologin">here</a>. I thank Ba3a-G for their original work.

The tool provides several commands:

- `--help` or `-h`: Show the help message.
- `--version` or `-v`: Show the version of the program.
- `--account` or `-a`: Perform LPU login with the provided account ID.
- `--list` or `-l`: List all stored account IDs.

If no command is provided, the tool will prompt the user for an account ID and perform LPU login.

The tool checks if the user is connected to LPU WiFi before performing any operations. If the user is not connected to LPU WiFi, the tool will exit with an error message.

The tool stores LPU credentials in environment variables and writes them to a file. The file is updated every time the user stores new credentials.

## 🛠️ Installation

### <img src="./assets/arch.png" alt="Arch" height="23" width="23"> Arch Linux

The tool is available on the [AUR](https://aur.archlinux.org/packages/llogin) with the package name `llogin`. You can install it using `paru`, `yay` or your prefered AUR helper:

```Bash
paru -S llogin
```

or

```Bash
yay -S llogin
```

> Note: I've also included the `PKGBUILD` file if you choose to run `makepkg` locally.

### <img src="./assets/ubuntu.png" alt="Ubuntu" height="23" width="23"> Ubuntu

The tool is also available on a Personal Package Archive (PPA) for Ubuntu users. You can add the PPA and install the tool using the following commands:

```Bash
sudo add-apt-repository ppa:smazmi/llogin
sudo apt update
sudo apt install llogin
```

### <img src="./assets/cargo.png" alt="Crates" height="23" width="23"> Other Systems

The tool is also available on [crates.io](https://crates.io/crates/llogin). You can install it using `cargo`:

```Bash
cargo install llogin
```

## 🚀 Usage

After installation, you can run the tool using `llogin` command followed by the desired options.

## 📝 Original Bash Script

The original Bash script by [@Ba3a-G](https://github.com/Ba3a-G) is also included in this repository for those who prefer using it.
