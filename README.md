# LPU WiFi Manager

This is a command-line tool for managing LPU WiFi connections, written in Rust. It's a rewrite of the original Bash script by [Ba3a-G](https://github.com/Ba3a-G). You can find the original repository [here](https://github.com/Ba3a-G/LPU-Wireless-Autologin). I thank Ba3a-G for their original work.

The tool provides several commands:

- `--help` or `-h`: Show the help message.
- `--version` or `-v`: Show the version of the program.
- `--account` or `-a`: Perform LPU login with the provided account ID.
- `--list` or `-l`: List all stored account IDs.

If no command is provided, the tool will prompt the user for an account ID and perform LPU login.

The tool checks if the user is connected to LPU WiFi before performing any operations. If the user is not connected to LPU WiFi, the tool will exit with an error message.

The tool stores LPU credentials in environment variables and writes them to a file. The file is updated every time the user stores new credentials.

## Installation

### Arch Linux

The tool is available on the AUR with the package name `llogin`. You can install it using `paru`, `yay` or your prefered AUR helper:

```Bash
paru -S llogin
```

or

```Bash
yay -S llogin
```

### Other Systems

The tool is also available on crates.io. You can install it using `cargo`:

```Bash
cargo install llogin
```

## Usage

After installation, you can run the tool using `llogin` command followed by the desired options.

## Original Bash Script

The original Bash script by [@Ba3a-G](https://github.com/Ba3a-G) is also included in this repository for those who prefer using it.
