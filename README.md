# Zsh History Sanitizer

## Overview
The **Zsh History Sanitizer** is a simple shell script designed to clean and sanitize your Zsh command history. By removing non-readable or corrupted entries, it ensures that your `.zsh_history` file remains tidy and secure, preventing the accidental exposure of sensitive commands.

## Features
- **Backup Creation**: Renames the current `.zsh_history` file to `.zsh_history_bad` for backup purposes.
- **Readability Enhancement**: Utilizes the `strings` command to extract readable entries and create a new `.zsh_history` file.
- **Instant Reload**: Immediately reloads the cleaned history into the current shell session.
- **Cleanup**: Removes the backup file after processing to save space.

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/zsh-history-sanitizer.git
   cd zsh-history-sanitizer

2. Make the script executable:
   ```bash
   chmod +x zsh_history_sanitizer.zsh

3. Run the script:
   ```bash
   ./zsh_history_sanitizer.zsh
